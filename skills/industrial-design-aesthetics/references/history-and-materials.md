# 共同历史与素材限制 / Shared history and media reuse

三种角度都使用同一项目总表，不因换Skill而重新开始。优先用户指定表；否则当前项目case-research-state/registry.json。没有总表时说明覆盖缺口，才用 [空模板](../assets/registry.template.json) 建新项目表。包内 [双案例历史快照](../assets/example-history.json) 只覆盖公开的本方向案例，不是最新总表，不是两个艺术Skill的全部历史。调用其他AI前附最新总表，返回后合并增量。

## 分开判断的三类重复

- 产品身份：型号、年份、别名、概念/量产/配置。旧产品有新问题可以深化，保留同一产品ID；同一产品同一主张仅换话术不算新文章。
- 论点：核心问题、结论、形式关系、比较对象与用途。换产品或换栏目可能仍重复旧解释；脚本词项相似只提示风险，不自动判定抄袭率。
- 媒体：源URL、原资产标识、来源页、原文件SHA-256、derived_from、可疑近似图。引用同一文献不等于复用同一图片。

已交付/已发布文章用过的媒体默认不能分配给新稿；裁切、镜像、压缩、改名、加字、同一视频片段等派生物仍按原媒体处理。仅改变URL尺寸参数不会自动变新。脚本给image_reuse预警时，先停止分配，确认原身份再更换；看图检查不同URL的近似素材，不能只等SHA相等。

同文章改稿、长短版和用户明确要求复用可沿用，记录同一analysis_id、版本、旧用途、新用途与reuse_reason。不得把复用图计为新增。用于新文章的深度比较并不自动豁免媒体限制，除非用户指定复用。

## 登记约定

schema_version为1；collections为cases、sources、searches、claims、images。

案例含id、title、kind（此方向通常product）、artist（可为实际设计师/团队，未知null）、year（未知null）、aliases、stage及publication。按文章ID在analyses记录skill_name、question、takeaway、stage、delivery_version等。长短版共用文章ID；比较中的参考产品不自动算独立文章。

主张type分fact、artist_intent、interpretation、unverified。事实与意图需source_ids；解释需指向有证据的前提主张；未确认不标publishable。来源按规范URL复用ID，已知同一家族使用evidence_family_id，避免转载当独立证据。

图片含case_id、source_url、source_page、asset_id、sha256、original_sha256、derived_from、edits与used_in；每篇用途说明status、role、delivery_files、reuse_reason。拿不到字节指纹就null并说明，不编哈希。发布状态只在有实际发布证据时记published_confirmed，交付或认可都不等于发布。

## 可选离线辅助

Python3.10+标准库，无账号、联网、收费API或第三方依赖。命令相对Skill根目录执行；路径用用户的项目路径替换。

```text
python scripts/registry.py init --registry ./project/registry.json --seed assets/registry.template.json
python scripts/registry.py check --registry ./project/registry.json
python scripts/registry.py assess --registry ./project/registry.json --candidate ./project/candidate.json
python scripts/registry.py merge --registry ./project/registry.json --entry ./project/increment.json --operation add
python scripts/registry.py merge --registry ./project/registry.json --entry ./project/revision.json --operation update
```

init不覆盖存在文件；assess只读。候选使用完整case对象，或{case:完整对象,sources:[],images:[],claims:[]}；仅提产品名不是有效输入。新增使用add，同一ID修订使用update；不能用add覆盖旧记录。写入有备份、并发锁和原子替换。保留旧版analyses.versions等记录，不用当前文本抹除原文；先试合并并校验引用。

脚本只做结构、已知身份/版本、来源族、文件与URL、词项重合提示；不识别全部视觉变体，也不验证作者真实想法、审美偏好或全网原创性。没有Python则同规则人工登记，返回增量由用户维护总表。缺历史必须留范围说明，不能跳过查重并宣称完成。
