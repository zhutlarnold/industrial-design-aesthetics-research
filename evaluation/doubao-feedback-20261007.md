# 豆包使用反馈与修复 / Doubao entry feedback

2026-10-07 (Asia/Shanghai)，Skill 0.1.1。依据用户截图，不公开个人账户、截图或无关聊天。

## 观察 / Observed

- 用户发送的是`PROJECT_OVERVIEW_ZH_EN.md`的GitHub文件页。该文件是项目说明，不含完整执行规则。
- 豆包回复“原始raw地址网络读取超时”，并按仓库名和文件名模拟生成项目概述。此处只是客户端自述，没有请求日志，不能确定真实网络故障位置。
- 问题既涉及读取失败，也涉及入口用途不清，以及失败后生成替代内容。模拟内容不等于按真实Skill运行。

The supplied document was a project statement. Doubao reported a raw-fetch timeout, then simulated an overview from metadata. The screenshot does not identify the network root cause or show that the skill was loaded.

## 当前连接核查 / Current-path checks

同日从Codex使用本机现有代理读取GitHub文件页、raw项目说明、raw完整提示词和Pages完整提示词，4个地址均HTTP200。3份文本与当时本地版本（0.1.0）一致。这证明此路径中文件存在且未损坏，不证明豆包服务端可读取，更不能解释豆包具体为什么超时。网页工具另一次读取返回cache miss，也不能据此认定仓库失效。

Four URLs returned HTTP200 through the current Codex/local-proxy path. Text matched the then-current 0.1.0 source. This is not a test of Doubao's fetcher; its network root cause remains unconfirmed.

## 已做修复 / Patch

区分项目说明和执行入口；增加完整TXT和自带全文的复制页面；SKILL.md及通用提示词要求读取失败时报告缺口，不凭元数据模拟Skill。保留既有专业美学方法、11项功能和原案例。使用真实正文可绕过对AI抓取GitHub的依赖，但不能修复平台工具、上下文截断或确保模型一定遵循规则。

The patch distinguishes document roles, embeds a full copyable prompt, adds an identical TXT attachment, and specifies an honest missing-input response. It does not repair the platform's fetcher or guarantee compliance.

## 待验证 / Pending

用户在豆包粘贴全文或上传可读取TXT后，要求先报告加载情况；检查是否实际读到核心方法、素材规则及结尾，而非只复述文件名。随后再给真实任务验证执行。此次尚未在豆包重新试跑，不将文件、浏览器或打包检查称作跨模型行为验收。

The revised prompt has not yet been rerun in Doubao. Copy-page and packaging checks establish delivery integrity only; a real loading and task test remains necessary.
