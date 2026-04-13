# Seedance Viral Forge

Reusable AI video prompt skills for builders who need Chinese short-video scripts that can be copied into Seedance 2.0 and published fast.

Seedance Viral Forge 是一个面向即梦 / Seedance 2.0 的 AI 视频脚本仓库，重点不是“写好看的提示词”，而是产出能直接生成、发布、测数据的中文脚本。

## What This Project Does

This repository helps users generate structured Chinese AI video scripts for three real short-video jobs:

- product-selling videos
- merchant lead-gen dance videos
- trend-driven traffic videos

Instead of treating prompt writing like vague inspiration, this repo turns it into reusable skills with clear inputs, default flows, output formats, and safety boundaries.

## Why This Matters

Most AI video prompt collections fail in production for the same reasons:

- they produce pretty wording instead of usable scripts
- they do not ask for the minimum missing inputs
- they mix default chat output with automatic file writing
- they ignore how Seedance handles memory, physical detail, and motion continuity

This repo is designed for the opposite. It favors direct-to-generation scripts, conservative defaults, and repeatable operator behavior.

## What You Get

| Part | What it does |
|------|---------------|
| `通用场景/SKILL.md` | Generates product-selling scripts for Douyin / 即梦 workflows |
| `跳舞/SKILL.md` | Generates merchant dance lead-gen scripts built around scene + character attraction |
| `热梗/SKILL.md` | Generates trend-driven traffic prompts for short viral clips |
| `shared/SEEDANCE_BASELINE.md` | Shared production rules for all three skills |
| `docs/` | GitHub Pages landing pages for search and AI discovery |
| `archive/` | Old drafts and non-production material |

## Quick Start

### 1. Pick the right skill

- Product selling: [`通用场景/SKILL.md`](./通用场景/SKILL.md)
- Merchant scene traffic: [`跳舞/SKILL.md`](./跳舞/SKILL.md)
- Trend traffic: [`热梗/SKILL.md`](./热梗/SKILL.md)

### 2. Give the minimum usable input

For `通用场景`:

- product name
- category
- 1-3 selling points
- ideally what it looks like and how it is used

For `跳舞`:

- merchant type
- the most filmable part of the venue
- what the offer / package sells

For `热梗`:

- a specific trend
- or just `/热梗` and let the skill propose directions

### 3. Follow the default flow

1. The skill extracts what is missing.
2. It returns 3 direction cards.
3. The user chooses A, B, C, or asks for all.
4. The skill outputs the final script in Chinese.

## Use Cases

### How to generate Seedance 2.0 product video scripts in Chinese

Use [`通用场景/SKILL.md`](./通用场景/SKILL.md) when you need short product-selling scripts with a clear reveal, simple shot logic, and natural CTA placement.

### How to create merchant dance promo prompts for 即梦

Use [`跳舞/SKILL.md`](./跳舞/SKILL.md) when the goal is local lead-gen: grab attention with character energy, then move viewers toward the venue or offer.

### How to turn current trends into AI short-video prompts

Use [`热梗/SKILL.md`](./热梗/SKILL.md) when you want traffic-first scripts built around hot topics, visual absurdity, and proven viral patterns.

### How to design reusable skills for AI video prompt workflows

Use [`shared/SEEDANCE_BASELINE.md`](./shared/SEEDANCE_BASELINE.md) plus the three production skills to study how prompt work can be structured into reusable operational protocols instead of one-off prompt dumps.

## Core Principles

- Copyable into Seedance first
- Chinese-only production output
- Ask for the minimum missing detail, not a giant intake form
- Default to conversation output, not file writing
- Repeat physical details because the model does not remember reliably
- Prefer one-shot or very few scene changes

## Documentation

- Docs home: `https://11yuxuanyang.github.io/seedance-viral-forge/`
- How to write Seedance product-selling prompts: [`docs/seedance-product-video-prompts.html`](./docs/seedance-product-video-prompts.html)
- How to make 即梦 merchant dance videos: [`docs/jimeng-merchant-dance-video-scripts.html`](./docs/jimeng-merchant-dance-video-scripts.html)
- How to make trend-based AI short videos: [`docs/ai-trend-video-prompts.html`](./docs/ai-trend-video-prompts.html)
- How this repo structures reusable AI video skills: [`docs/reusable-ai-video-skill-design.html`](./docs/reusable-ai-video-skill-design.html)

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=11Yuxuanyang/seedance-viral-forge&type=Date)](https://www.star-history.com/#11Yuxuanyang/seedance-viral-forge&Date)

## Repository Structure

```text
ai-video/
├── README.md
├── AGENTS.md
├── llms.txt
├── CITATION.cff
├── CLAUDE.md
├── shared/
│   └── SEEDANCE_BASELINE.md
├── docs/
│   ├── index.html
│   ├── styles.css
│   ├── llms.txt
│   ├── robots.txt
│   ├── sitemap.xml
│   └── plans/
├── 通用场景/
│   └── SKILL.md
├── 跳舞/
│   └── SKILL.md
├── 热梗/
│   └── SKILL.md
└── archive/
```

## Best Entry Points

- [`README.md`](./README.md)
- [`AGENTS.md`](./AGENTS.md)
- [`llms.txt`](./llms.txt)
- [`shared/SEEDANCE_BASELINE.md`](./shared/SEEDANCE_BASELINE.md)
- [`通用场景/SKILL.md`](./通用场景/SKILL.md)
- [`跳舞/SKILL.md`](./跳舞/SKILL.md)
- [`热梗/SKILL.md`](./热梗/SKILL.md)

## Keywords This Repository Covers

- Seedance 2.0 prompts
- 即梦提示词
- AI video script skills
- Chinese short-video prompts
- Douyin AI product video script
- merchant dance promo prompt
- viral trend AI video prompt
- reusable `SKILL.md` design

## License

MIT. See [LICENSE](./LICENSE).
