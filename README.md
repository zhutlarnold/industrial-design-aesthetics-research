# 工业设计美学 / Industrial Design Aesthetics

## 发给AI前选对文件 / Choose the right document

| 用途 / Purpose | 文件 / File | 使用方式 / How to use |
|---|---|---|
| 让豆包等普通AI执行分析 / Run analysis in ordinary chat | [完整TXT](universal-prompt.txt) · [完整Markdown](universal-prompt.md) | 上传可读取附件或复制全部正文；不是只发URL / Attach readable content or paste the entire text, not just its URL |
| 打开页面复制全文 / Copy the full prompt in a browser | [复制入口](docs/use-with-ai.html) | 你打开页面、复制，再粘贴到AI；页面内含全部规则 / Open, copy and paste; all rules are embedded |
| 分享项目及升学材料 / Project evidence | [中英文项目说明](PROJECT_OVERVIEW_ZH_EN.md) | 介绍目标、贡献和验证，不代替执行规则 / Purpose, contributions and validation, not operating rules |
| 原生Skill客户端 / Native skill client | [完整Skill文件夹](skills/industrial-design-aesthetics/) | 安装完整目录，按任务读取参考 / Install the directory and read relevant references |

AI报告读取超时、只看到文件名或没有读到末尾时，不应模拟“已按Skill执行”。改为提供全文；如果仍截断，分段粘贴，最后一段发完再开始任务。完整规则也不会为客户端增加联网、看图或文件导出工具。

If retrieval fails or text is truncated, supply the complete prompt directly; for chunked input, begin the task only after the final chunk. The prompt does not provide missing browsing, vision or export tools.

**完整Skill初版已提炼；当前使用入口修订版0.1.1，后续继续完善。** 核心方法：专业概念 → 白话解释 → 原图细节 → 关系分析 → 美感效果。以两篇迭代试稿为开发依据，不将结构检查等同外部模型或读者验收。

**Skill release 0.1.1 (chat-entry repair).** Explain the aesthetics of real industrial products using accessible art concepts and source imagery. Developed from two revised trials; structural validation does not establish reader comprehension or cross-model behaviour.

- [使用方法与11项功能提示词 / Usage and 11 function prompts](skills/industrial-design-aesthetics/README.md)
- [Skill指令 / Skill entrypoint](skills/industrial-design-aesthetics/SKILL.md)
- [普通AI完整单文件提示词 / Complete text-chat prompt](universal-prompt.md)
- [中英文项目说明与贡献证据 / Bilingual project statement](PROJECT_OVERVIEW_ZH_EN.md)
- [验证 / Validation](VALIDATION.md) · [更新记录 / Changelog](CHANGELOG.md)
- [下载Skill及Plugin / Download](https://github.com/zhutlarnold/industrial-design-aesthetics-research/releases/tag/v0.1.1-skill)

安装示例 / Installation prompt:

```text
使用 $skill-installer，从 https://github.com/zhutlarnold/industrial-design-aesthetics-research/tree/main/skills/industrial-design-aesthetics 安装这个Skill。
```

普通AI：复制universal-prompt.md全文或作为附件发送，附最新历史后给任务。Native clients should load the complete skill folder; ordinary chat can use the complete text prompt and attached history. See [official skill guidance](https://learn.chatgpt.com/docs/build-skills). GitHub sharing is not universal-directory publication.

三份内容保持独立：本方向解释美学原理；[科技参与艺术创作](https://github.com/zhutlarnold/tech-in-art-skill)解释技术成为艺术语言；[艺术批判工业科技](https://github.com/zhutlarnold/art-tech-critique-skill)分析社会批判与生活哲思。它们共用项目历史、素材限制和双语维护要求。

---

## 保留的案例与研究 / Preserved trials and research

# 生活中的工业设计：美学与功能

第三个内容方向的研究与双案例试稿，v0.2，2026-10-06。两篇案例已作为Skill初版的开发依据，保留供阅读与后续完善。

重点是让读者理解美学原理：**专业概念 → 一句白话 → 图片中的证据 → 关系分析 → 美感效果**。解释术语，但不把审美判断包装成普遍定律，不强加哲学反思。

| 阅读内容 | 链接 |
|---|---|
| 五种车灯的完整长文、5张原始图片 | [好看的车灯，究竟好看在哪里？](cases/01-volvo-ex90.md) |
| 榨汁器的完整长文、3张原始图片 | [这件小雕塑，居然是榨汁器](cases/02-juicy-salif.md) |
| 可以复制的较短正文 | [车灯](cases/01-volvo-ex90-post.txt) · [榨汁器](cases/02-juicy-salif-post.txt) |
| 同类 Skill、Similarity & Difference、源码阅读 | [研究报告](research/similarity-difference.md) |
| 车灯评选数据、统计口径与限制 | [证据表](research/headlight-evidence.md) |
| 第三个方向的方法草案 | [method-draft.md](research/method-draft.md) |
| 素材历史增量 | [material-history.json](research/material-history.json) |
| 更新与验证 | [CHANGELOG.md](CHANGELOG.md) · [VALIDATION.md](VALIDATION.md) |

**直接分享阅读入口：** https://zhutlarnold.github.io/industrial-design-aesthetics-research/

入口和每篇页面均可切换完整长文与较短图文版。较短正文保留较多解释，不承诺适配所有账号的字数限制；可配图片分页编辑。下载 [Releases](https://github.com/zhutlarnold/industrial-design-aesthetics-research/releases) 的 v0.2 ZIP，解压后打开 `docs/index.html` 即可离线阅读。保留 v0.1 发布包及 Git 历史，旧版案例文件名继续使用以避免旧链接失效。

车灯以2023年两个“年度颜值车灯”类别及2025年DVN行业投票为选材依据，再比较极星4、智己LS7、Audi A6 Avant e-tron、Opel Grandland和Volvo EX90；这些数据不能证明全球消费者公认的最好看排名。榨汁器按用户要求单件细读；榨汁器本身仍有同类产品。

采用有出处的原始外观图和设计档案，不用 AI 生成图片替代证据。新选4张图片检查已知项目历史；同一文章修订沿用1张Volvo与3张榨汁器图片，明确登记沿用原因。长短版共用文章身份，不能算4篇新案例。跨 AI 去重需要共享最新历史，本仓库不自动获得其他平台记录。交付试稿不代表已经在小红书发布。

下一步：使用Skill初版完成新任务，收集具体输出与反馈，在共同历史和GitHub中记录迭代。
