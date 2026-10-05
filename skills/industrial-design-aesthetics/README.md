# 工业设计美学 / Industrial Design Aesthetics

版本 / Version **0.1.0 · 初版 / Initial release**

## 中文说明

本Skill研究真实工业产品的美学与功能，让没有美术基础的读者也能看懂专业分析。核心顺序是“专业概念 → 一句白话 → 图片细节 → 关系分析 → 美感效果”。可分析单件产品，也可比较多个用途相近但造型不同的产品；默认输出解释充分的长文和较短图文版，不强制人生或伦理反思。

## English overview

This skill explains the aesthetics and function of real industrial products for readers without formal art training. It moves from an accurate art concept to a plain-language definition, visible image evidence, relationships between elements, and the resulting visual impression. It supports single-product readings and comparisons of differently designed peers. Full-length and shorter illustrated editions preserve the same claims; philosophical reflection is not a mandatory ending.

## 如何使用 / How to use

**原生Skill客户端 / Skill-capable clients:** 安装整个 `industrial-design-aesthetics` 文件夹，保留SKILL.md、references、scripts、assets和agents。只复制入口会缺少资料。支持Codex的环境可向安装器发送：

```text
使用 $skill-installer，从 https://github.com/zhutlarnold/industrial-design-aesthetics-research/tree/main/skills/industrial-design-aesthetics 安装这个Skill。
```

Then invoke `$industrial-design-aesthetics` with the task, desired language, product or topic, and latest shared history. Local discovery and installer support depend on the client; see [official guidance](https://learn.chatgpt.com/docs/build-skills). The plugin ZIP contains a portable manifest and this skill; GitHub distribution is not universal-directory approval.

**普通AI聊天 / Ordinary AI chat:** 从仓库下载 `universal-prompt.md`，上传该文件或复制其全文，并附最新共同历史；发送任务。它已包含方法参考正文，不要求AI能打开GitHub链接。普通聊天是提示词加载，不等同原生安装。需要联网才能完成新资料检索，需要图片理解才能核对画面；没有文件工具则交付文字、图片链接和历史增量，不假装已经生成文件。

For a text-only chat, attach or paste `universal-prompt.md` and the latest history, then describe the task. Browsing, vision, file export and persistence are host capabilities, not capabilities created by the prompt. The package does not need a paid API or credentials; the optional history helper requires Python3.10+ standard library.

## 功能与提示词 / Functions and prompts

以下对应自然语言任务范围，不是固定关键词开关；“只”限制范围，多个功能可以组合。

| 功能 / Function | 可复制提示词 / Example prompt | 结果 / Output |
|---|---|---|
| 1.选题与视觉筛选 / Topic selection | 使用 $industrial-design-aesthetics，先读历史，给我3个有清楚原图、适合解释美学原理的生活产品候选，先不写稿。 | 原图或链接、可分析原理、资料与历史差异 / Candidates, visual rationale and history differences |
| 2.单件细读 / Single-product reading | 使用 $industrial-design-aesthetics，只分析这件台灯的比例、正负形与明暗，先解释概念，再结合我给的图展开。 | 图像依据与美感分析 / Image-grounded formal analysis |
| 3.同类比较 / Peer comparison | 使用 $industrial-design-aesthetics，比较3—5种造型不同的车灯，用共同美学维度解释差别，不强制排第一。 | 共同维度表及充分解释 / Comparable dimensions and explanations |
| 4.专业概念白话讲解 / Accessible concepts | 使用 $industrial-design-aesthetics，只解释正负形，用这张产品图指给我看，不扩成完整案例。 | 简短准确定义＋可见细节 / Plain definition and visible examples |
| 5.审美数据核查 / Preference evidence | 使用 $industrial-design-aesthetics，查哪些车灯获得好看认可，列样本、指标、权重和缺口，区分纯审美投票与技术奖。 | 有边界的认可结论，不造榜单 / Bounded findings and data limits |
| 6.设计师意图 / Design intent | 使用 $industrial-design-aesthetics，只查这个产品的设计者访谈，将明确陈述、后期回顾与你的解读分开。 | 来源定位、可确认意图、缺口 / Sourced intent and uncertainty |
| 7.原图选择 / Source imagery | 使用 $industrial-design-aesthetics，只选原始配图，检查型号和历史复用，给图序、图注、出处和分析用途。 | 可取得的原图及清单 / Available source images and captions |
| 8.长短图文 / Long and short editions | 使用 $industrial-design-aesthetics，研究一件新产品，交付解释充分的长文和约900字较短图文版，配真实原图与依据。 | 两版正文、图片、来源、历史增量 / Both editions, images, evidence and history increment |
| 9.自然改稿 / Revision | 使用 $industrial-design-aesthetics，只改这份稿，让专业概念更容易理解、中文更自然，保留事实，不添哲思结尾。 | 针对性改稿与修改说明 / Scoped revision |
| 10.查重与登记 / Deduplication and history | 使用 $industrial-design-aesthetics，只检查这次选题、论点、图片在共同历史中是否用过，保留旧记录并给增量。 | 有范围的重复风险和登记 / Bounded duplicate checks and increment |
| 11.分享文档 / Shareable document | 使用 $industrial-design-aesthetics，将认可稿与原图做成可转发图文文档，检查页面；有已授权分享服务才上传。 | 环境支持的文件或验证过的分享链接 / Supported files or verified authorised share link |

English invocation example:

```text
Use $industrial-design-aesthetics to analyse a real household product. Explain the relevant art concepts in plain English, point to the image details, and show how their relationships shape its visual appeal. Deliver a full article and a shorter illustrated edition, with sources and a shared-history increment. Do not add a mandatory philosophical ending.
```

## 目录与记录 / Files and records

- `SKILL.md`：触发范围与工作指令 / scope and operating instructions.
- `references/`：形式分析、比较证据、写作交付、历史规则、两篇经验 / progressively loaded methods and trial lessons.
- `scripts/registry.py`：已知历史的结构检查与重复提示 / optional offline registry helper.
- `assets/registry.template.json`：新项目空表 / empty template, not proof of no prior work.
- `assets/example-history.json`：本方向公开案例快照 / partial example snapshot, not a live shared ledger.

新稿默认不复用已交付/已发布媒体；同稿修订或明确指定可沿用，必须保留关系与理由。三个角度共用最新历史，跨AI不会自动同步。

New articles normally use unused media. Revisions and explicitly requested reuse retain identity and reasons. Shared history must travel across clients; no automatic cross-AI synchronisation is claimed.

中英文项目说明、证据、贡献边界见仓库根目录 `PROJECT_OVERVIEW_ZH_EN.md`；更新见根目录CHANGELOG.md；验证范围见VALIDATION.md。两篇旧案例为开发依据，不代表自动化模型或读者效果已经验证。

[中英文项目说明 / Bilingual project statement](PROJECT_OVERVIEW_ZH_EN.md)：目标、功能、项目发起者贡献、AI参与与验证边界。 Purpose, capabilities, contribution, AI assistance and validation limits.
