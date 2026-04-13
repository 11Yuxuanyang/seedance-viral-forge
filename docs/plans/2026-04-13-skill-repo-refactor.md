# Skill Repo Refactor Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** 把仓库收口为一套生产版 skill 结构，统一协议、入口文档和维护规则。

**Architecture:** 保留根目录三个生产版 skill 作为唯一真相；新增共享规范文档和 README；把旧的嵌套快照移入 `archive/`，避免双份维护。

**Tech Stack:** Markdown, Codex skills, Seedance prompt conventions

---

### Task 1: 统一仓库入口

**Files:**
- Create: `README.md`
- Modify: `CLAUDE.md`

**Step 1:** 明确生产目录和维护规则  
**Step 2:** 写仓库入口说明和最小输入要求  
**Step 3:** 把旧的 `.claude/skills` 说法移除  
**Step 4:** 复查目录结构描述是否一致

### Task 2: 抽共通基线规则

**Files:**
- Create: `shared/SEEDANCE_BASELINE.md`

**Step 1:** 提炼三个 skill 的共通约束  
**Step 2:** 写成可维护的基线文档  
**Step 3:** 让各 skill 只保留差异化策略

### Task 3: 重写三个生产版 Skill

**Files:**
- Modify: `通用场景/SKILL.md`
- Modify: `跳舞/SKILL.md`
- Modify: `热梗/SKILL.md`

**Step 1:** 统一 front matter  
**Step 2:** 统一默认模式、批量模式、保存策略  
**Step 3:** 修复触发词、输出协议和默认行为冲突  
**Step 4:** 删除会让模型漂移的冗余长说明

### Task 4: 归档旧快照

**Files:**
- Move: `ai-video-skills/**` -> `archive/legacy-repo-snapshot/**`

**Step 1:** 保留历史内容，但移出生产目录  
**Step 2:** 确认 README 与 CLAUDE 不再引用旧路径

### Task 5: 验证

**Files:**
- Verify: repo tree and file content

**Step 1:** 检查顶层目录是否只剩一套生产版  
**Step 2:** 检查三个 skill 是否都声明默认不自动保存  
**Step 3:** 检查 `热梗` invocation 与正文是否一致  
**Step 4:** 用 `git diff --stat` 做最终核对

