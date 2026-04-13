# ai-video-skills

面向 Seedance 2.0 / 即梦 的短视频脚本技能仓库。目标不是写“好看的提示词”，而是产出能直接拿去生成、发布、测数据的中文脚本。

## 生产版 Skills

| Skill | 触发词 | 用途 |
|------|------|------|
| `通用场景` | `/通用场景` | 产品带货脚本 |
| `跳舞` | `/跳舞` | 商家场景引流脚本 |
| `热梗` | `/热梗` | 热点流量脚本 |

## 仓库原则

- 单一真相：生产版 skill 只保留在仓库根目录的三个文件夹里
- 默认先输出到对话，不自动写文件；只有用户明确要求时才保存
- 共通规范集中写在 [shared/SEEDANCE_BASELINE.md](/Users/yuxuanyang/ai-video/shared/SEEDANCE_BASELINE.md)
- 历史草稿和旧快照不参与当前维护，统一放到 `archive/`

## 典型工作流

1. 用户给输入
2. Skill 先给 3 个方案卡或 1 个角度矩阵
3. 用户选择
4. Skill 输出最终脚本
5. 用户再决定是否保存成 `.md`

## 最小输入要求

### 通用场景

- 产品名
- 产品是什么
- 1-3 个卖点
- 最好补一句“长什么样、怎么用”

### 跳舞

- 商家类型
- 商家最值得拍的点
- 团购/套餐卖什么
- 想要小姐姐、帅哥，还是不限

### 热梗

- 直接给热点
- 或只输入 `/热梗`，让 skill 先查最近热点再给方案

## 目录结构

```text
ai-video/
├── README.md
├── CLAUDE.md
├── shared/
│   └── SEEDANCE_BASELINE.md
├── docs/
│   └── plans/
├── 通用场景/
│   └── SKILL.md
├── 跳舞/
│   └── SKILL.md
├── 热梗/
│   └── SKILL.md
└── archive/
```

## 维护规则

- 改共通约束，先改 `shared/SEEDANCE_BASELINE.md`
- 改调用协议，再改对应的 `SKILL.md`
- 不要再引入第二套平行目录
- 需要实验新 skill，就放到 `archive/experiments/` 或单独分支，不要混进生产版

