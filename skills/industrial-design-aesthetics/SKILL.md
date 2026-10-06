---
name: industrial-design-aesthetics
description: Explain the aesthetics of real industrial products through accurate art concepts, accessible language, source images, and evidence. Use for single-product readings, comparisons of differently designed peers, design-intent checks, illustrated long/short articles, and material deduplication. Focus on understanding form and function rather than mandatory ethical reflection or creating new products.
---

# 工业设计美学 / Industrial Design Aesthetics

让普通读者对着真实产品图看懂美感：**专业概念 → 一句白话 → 指认细节 → 分析关系 → 说明视觉效果**。版本0.1.1，源于车灯比较与Juicy Salif两篇试稿的迭代。默认中文，用户可指定英文或双语。使用与功能提示词见 [README](README.md)。

## 0. 识别执行入口 / Identify the operating entry

`PROJECT_OVERVIEW_ZH_EN.md`介绍项目目标、贡献和验证状态，不是完整执行提示词。原生Skill需要入口及任务所需参考；普通聊天使用完整`universal-prompt.md`或内容相同的TXT正文。URL、文件名、网页摘要和项目说明不能替代尚未读取的执行规则。

用户要求按此Skill执行时，先确认实际收到规则正文。只有链接且读取失败，就说明尚未加载，并请提供完整提示词正文或可读取附件；不要按仓库名、文件名模拟Skill、项目内容、研究或输出。收到完整规则后直接执行已给任务，无需额外确认。若仅收到部分，指出缺失范围；可做用户明确允许且不依赖缺失规则的工作，并标明所依据的材料。

首次加载或用户检查加载情况时，简短概括实际读到的核心方法与限制，帮助发现发错文件或截断；这不是权限确认。工具是否可联网、看图、导出文件或维护历史需按实际环境判断，不能因为提示词声明这些任务就假装具备工具。

The bilingual project statement is documentation, not the full operating prompt. A URL or filename does not establish that instructions were read. If a task depends on this skill and retrieval fails, report the missing instructions and request readable text or an attachment instead of inventing a substitute. Once the rules are available, proceed with the authorized task. Disclose partial input and actual host capabilities; a short first-load recap is a diagnostic, not an approval gate.

## 1. 选择功能与范围

按请求选题、单件细读、同类比较、术语解释、数据核查、意图研究、选图、长短文、修改、查重或分享文档；用户说“只……”就只做该项。完整案例才组合研究、分析、原图与交付。没有指定对象时先给少量有原图、资料可查且具有不同形式关系的候选，不凭知名度、参数或漂亮标题选题。

主线是生活中工业产品的美学与功能。艺术批判工业科技、技术参与艺术创作属于相邻角度，不能机械移入它们的伦理结尾、互动实验或技术秀。用户明确指定跨角度时尊重其范围。

## 2. 先读共同历史并核对身份

先读取用户指定的共同历史；未指定时查当前项目 `case-research-state/registry.json`。参照 [历史与素材](references/history-and-materials.md)，逐项比较产品型号/年份/配置、别名、旧文核心问题、论点、图片来源与指纹。不同栏目共用身份，长短版及同稿修订共用文章ID。

新文章默认不使用已交付或已发布文章用过的图片、截图、视频及同源变体；改名、裁切、压缩、镜像或加字不是新素材。发现匹配先更换素材。同稿修订或用户明确要求复用，可登记原因后沿用，不重复索要确认。历史缺失标明覆盖范围，不宣称“从未用过”。交付时维护历史，不能以空表或本包样例替换已有总表。

## 3. 取得图片、资料与比较依据

研究或比较时读 [证据与比较](references/research-and-comparison.md)。先确认具体型号和原图版本，实际看图再记录轮廓、比例、空间、颜色、明暗、表面与部件安排。品牌外观渲染、产品实拍、设计草图分开标注；不能把概念车当量产款或把草图当结构实测。

有多个用途可比且造型不同的同类，通常选3—5个做共同维度比较；单件细读不意味着没有同类。不要求每篇比较，也不强制选唯一赢家。图片机位、光线不同，不能当作控制变量实验。

“最好看”“最受欢迎”需要可核对的偏好数据，说明样本、时间、指标及缺失字段。纯审美调查、综合设计奖、技术奖、销量分别处理；缺数据就用明确的编辑选材理由，不编排名。先读实际来源，不把品牌获奖通稿和主办方记录当独立两次投票。

## 4. 从美术概念解释美感

分析时读 [形式分析](references/analysis-method.md)。按物件选择最有用的概念，不堆一串定义。首次使用术语就给准确的短解释，紧接着指出图中哪条线、哪个空处、哪些明暗正在起作用；再说明这些元素如何相处，形成何种视觉印象。完整案例至少展开三项具体形式关系，简短单项请求按其范围作答。

例如比例是局部之间及局部与整体的大小关系；腿细长、主体悬起、下方留空，才是物件显得轻巧的依据。“轻巧”不证明实际重量小或稳定性好。对称、曲线、黄金比例、简洁都不是普遍优美定律。

把技术、材料和用途放回具体形状：部件为何在这里，身体怎样使用，工艺怎样影响可见形式。设计师访谈支持其陈述的意图，原图支持观察，本文解释另行标注；性能、安全或耐用结论需要对应证据。找不到作者意图仍可分析形式，不能补造心理或采访。

## 5. 写作与原图交付

写稿、改稿、配图或制作分享文档时读 [写作与交付](references/writing-and-delivery.md)。从具体物件进入，解释有专业依据但用自然中文；减少空泛的高级感、科技感、套话、连续反问与生硬总结。结尾帮助读者再看懂一次产品，不强制人生哲思、内疚或伦理讨论。生活类比服务于理解，不虚构使用经历。

完整案例默认给解释充分的长文与较短图文版，短版保留相同核心事实与原理；约900字可作短版编辑起点，按用户要求及可确认的平台限制调整，不能冒充普遍字数上限。来源附录、图片清单与发布正文分开。

用有出处的原始产品图片，不用生成图替代事实证据。选图看主体辨识度、美感和细节可读性，其他图补充分析所需视角而非凑张数。图注核对产品、版本、来源及已知摄影署名。实际取得、查看和检查图片后才称交付图片包；仅有链接就交付链接及缺口。已授权直接使用无需额外逐图确认，但不声称未经核实的授权事实。

分享文档可采用Markdown或图文HTML，环境支持时采用Word/PDF；检查图片、正文、图注及实际页面。保存到用户指定位置，无指定则当前项目交付目录；本机地址不算公开链接。使用Skill不意味着授权发布社交账号或上传外部服务，依当前任务授权执行。

## 6. 验收、登记与阶段提醒

具体复盘见 [两篇经验](references/two-case-lessons.md)。交付前核对：读者能否从图中指认每项原理，比较维度是否一致，意图与解读是否分开，两版是否一致，原图是否匹配型号及历史，结尾是否解释美感。不要承诺全部读者都“没有AI感”或一定有流量。

Python3.10+可用时运行 `scripts/registry.py` 做登记结构与已知历史的重复预警；它不判断美感、事实真伪或全网语义独创性。无代码执行时按同一规则人工维护，交付增量供用户并入共同历史。

研究、已交付、用户认可与平台发布分别记载；没有发布证据保持unknown。每步简述结果、依据与下一步。历史示例不是最新云端状态；跨AI需携带最新总表。
