# 第三个方向：生活中的工业设计——美学与功能

研究日期：2026-10-05。状态：公开同类检索、选定源文件阅读、两篇初步案例已制作；完整 Skill 尚未生成。

## 查重结论与检索范围

工业设计分析已经有直接同类，不能宣称这个方向“市面上没有”。本轮检索 Google 可见的公开 GitHub、Skill 目录及链接来源，关键词包括 `"SKILL.md" "industrial design"`、`"SKILL.md" "design critique"`、`"SKILL.md" "design history"`、`industrial-design aesthetic analysis` 和此前讨论的 `Arts & Design Tutor`。选取六个实际能读到源文件、在任务或方法上相关的项目，不根据目录宣传页或单个星数认定流行程度。

没有找到完全覆盖本项目下述组合的已读入口：生活中真实产品的案例选材，具体形式与功能分析，来源支持的设计意图，自然中文图文，生活思考，以及跨文章素材限制。但这只是这六个项目、这些已读文件的比较结果，不是全市场独创性证明。没有对私有项目、付费内容、所有语言及全部公开仓库做穷尽检索。

## Similarity & Difference

| 公开项目与源文件 | Similarity：实际重合 | Difference：与我们的任务不同 | 可取之处及本次转化 |
|---|---|---|---|
| [Industrial Design Portfolio](https://github.com/truman-t3/industrial-design-portfolio-skill/blob/653fbd3c4b070c72cbd21a3253aa9300940835d8/SKILL.md) | 实体产品案例、形态与材料分析、图文证据、叙事编排；最接近我们的研究与交付环节 | 面向求职、申请、客户评审的本人作品集，以横向 HTML 多页介绍个人贡献；可使用明确标注的生成图 | 学习证据和意图分开、每篇有独立论点；改成对既有设计的第三方中文案例分析 |
| [Buro industrial-designer](https://github.com/getburo/buro-free/blob/86cd7e849bee7b04b159644afdb6a9abd0f4a7c8/skills/industrial-designer/SKILL.md) | 产品轮廓、操作线索、人机关系、功能与寿命 | 输出设计规格与改进意见；功能主义取向强，要求删去没有实用作用的装饰；不是社交案例写作 | 学习追问“这个形状怎么被使用”；保留情感、符号与装饰的讨论空间 |
| [Product Designer](https://github.com/shawnlix/claude-product-designer-skill/blob/76c2b29194674a4dc936d44894dd14045ea6521b/SKILL.md) | 机制、材料、形态、持久记录、真实参考的保存 | 指导从简报、草图到渲染的新产品创作，依赖可选图像生成；不是分析已有产品 | 学习先核对机制、把决策写进文件；不采用生成草图和原型流程 |
| [Arts & Design Tutor](https://github.com/24kchengYe/human-skill-tree/blob/be589ddd04c945cd64642702ed7f6cfbd2466e03/app/content/skills/02-arts-design-tutor/SKILL.md) | 观察、形式分析、解释、评价；视觉证据与历史背景 | 教学、练习、复习和作品集训练；覆盖艺术与平面设计，不专门输出工业设计发布稿 | 从能指给读者看的线、体块、颜色和空隙开始，再讨论意义；不带教学练习 |
| [Anthropic design-critique](https://github.com/anthropics/knowledge-work-plugins/blob/8444efcd48f7012f09797778a36a33e73d0861f4/design/skills/design-critique/SKILL.md) | 第一眼、视觉层次、使用目标、具体理由 | 主要面向界面与 Figma，输出问题及修改建议；不研究实物设计史 | 把第一眼吸引与正文解释对齐，不能拿界面触控指标替代实体产品判断 |
| [Content Research Writer](https://github.com/ComposioHQ/awesome-claude-skills/blob/be2a406907dbc61b73e6827ded415c96139d13a2/content-research-writer/SKILL.md) | 检索、引用、开头、提纲、反复修稿、作者语气 | 通用内容写作；已读入口没有实体产品版本与设计意图的专门约束 | 把证据资料与读者正文分开，开头落到具体物件；不采用示例中未经验证的数据 |

相似是工作范围和方法的定性比较，不是抄袭率。描述、分析、论证、引用等通行方法本身不构成我们独有的方法。

## 阅读到了什么源文件

已阅读上述六个项目的 `SKILL.md`，以及相关参考文件：

- Portfolio：`references/industrial-design-evidence.md`、`references/story-architecture.md`、`references/checklist.md`。
- Portfolio 可执行源代码：`scripts/validate_portfolio.py`、`scripts/validate_manifest.py`。
- Buro：`skills/industrial-designer/references/canon.md`。
- Product Designer：`references/heuristics.md`、`assets/brief-template.md`。
- 能找到的根目录许可证。精确提交、路径和文件指纹见 [source-index.json](source-index.json)。

前四个最早抽样项目的选定 Skill 目录内，没有发现相邻的 `.py/.js/.ts/.sh` 实现文件；主要分析方法就在 Markdown 指令中。不能把阅读提示词说成研究了不存在的算法。

Portfolio 的两份验证脚本是结构检查：一份检查占位符、图像说明、版式、HTML 与清单对应等；另一份检查证据、作者、项目与页面引用的字段关系。它们不能验证设计师真的这样想、性能数据是否真实，也不能证明读者喜欢文章。本次阅读代码，没有运行上游 Skill 或把其作品集专用验证器用于我们的文章。

Buro 指令提到 `buro:cmf`，但此次公开仓库的递归文件列表中没有对应文件。不能声称读过该模块；本轮材料与表面方法来自另外两个实际读取的工业设计项目。

## 我们独立整理的试跑方法

每篇先回答一个具体问题，用能看到的细节带读者往下走。

1. **选物件与选图**：读者在生活里能接触，第一张真实照片清楚且有吸引力，后续图片有不同证据作用。照片的吸引力是编辑判断，不能保证浏览量。
2. **看外形**：指出线条、比例、体块、空隙、材料或光。每个“美”“稳”“轻”的判断都要有能对照图片的原因。
3. **查用途和机制**：这个部件做什么，身体怎样与它接触，材料或技术怎样影响外形。看图不能证明效率、安全、耐用或维修成本。
4. **找设计意图**：引用参与者访谈、官方档案；区分原始陈述、后期回看及我们的解释。品牌声明只证明它这样介绍产品，不自动证明效果。
5. **讨论取舍**：保留不同合理评价。简洁、功能、装饰、情感不预设一个永远获胜；不强迫每篇都批判工业危害。
6. **连回日常**：提一个与物件和论点相连、允许不同答案的生活问题，少用“科技与人性的边界”等脱离案例的套话。
7. **查历史并交付**：检查作品、论点与实际媒体分别是否重复；同稿格式版本共用文章身份，图片交付即登记；缺历史则说明范围。

这是本次试稿的工作方法，不是已打包、已行为验证的完整 Skill。

## 两篇试稿覆盖的差别

| 项目 | 核心问题 | 主论点 | 图片作用 | 历史状态 |
|---|---|---|---|---|
| [Volvo EX90](../cases/01-volvo-ex90.md) | 灯光和机械运动如何让机器显得亲近？ | 灯组在履行照明任务时，也借身体动作表达身份与迎接 | 实物近照、团队设计图、实物协作场景 | 以前提过并写过文字样稿的“雷神之锤”专题，本次明确为深化；新选图 |
| [Juicy Salif](../cases/02-juicy-salif.md) | 雕塑外形带来的喜欢，如何与工具用途相处？ | 使用之外的交谈与欣赏有价值，使用取舍也仍值得讨论 | 雕塑般的实物、使用情境、原始草图 | 本任务已知历史内的新选题；新选图 |

两篇用不同机制、不同形式分析与不同生活问题来试跑。它们能帮助判断方法是否适合栏目，不能仅凭两篇推断所有选题都能跑通。

## 如何降低内容和素材重复

共用本项目历史位置 `case-research-state/registry.json`，交付记录同时进入本研究仓库的 [material-history.json](material-history.json)。公开文件只包含此次案例的增量，不发布全部私人项目记录。

新稿默认不用已交付或已发布的媒体。改文件名、压缩、裁切、镜像、加字及同一视频片段，不能自动算新素材。引用同一个资料网页不等于复用图片。旧题深化允许采用新媒体并登记新论点；同稿修订或用户明确要求复用可沿用，记录关系和原因。跨 AI 要附最新共同历史，两个项目不会自动同步云端状态。

当前能查同源 URL、原媒体标识和文件指纹，近似素材还需看原图。历史论点缺口、其他 AI 未提供的媒体、未知的发布状态不能被当作“确认没用过”。

## 不照搬的内容

Buro 的根许可写明保留所有权利；本仓库只发布自己的比较与写作，不复制它的指令文本。Arts Tutor 所在 `app/` 路径与根许可证对 `skills/` 的双许可说明有适用范围差别，不擅自当成 MIT。Content Research Writer 在本次根文件列表中未找到许可证。两个新查到的工业设计项目为 MIT，Anthropic 为 Apache-2.0；即使允许复制，也不需要把整份提示词搬来作为自己的内容。

研究借鉴可以有清楚出处；创新性结论仍需要更广泛检索和独立测试。下一步是根据你对这两篇的反馈修稿，达到满意标准后再提炼完整 Skill、提示词功能表和验证用例。
