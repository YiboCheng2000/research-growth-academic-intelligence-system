# 来源与证据政策

> **只想把这套证据规则加入你现有的 AI 工作流？直接复制：**

```text
请读取这个仓库：
https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

请把 05_SOURCE_AND_EVIDENCE_POLICY.md
作为我后续学术检索与文献总结的强制质量规则。

不要因为其他提示词更长就忽略这些规则。
如果你的工具无法访问某个来源，明确报告覆盖限制。
如果只有摘要，不要写成已读全文。
```

这份文件可以单独交给任何 AI 作为“学术检索质量规则”。

## 1. 发现源不等于证据源

可以用于发现：

- Google Scholar
- Crossref
- OpenAlex
- Semantic Scholar
- 搜索引擎
- 数据库检索页
- 期刊目录
- 官方公众号 / 社交媒体

涉及研究结论时，优先回到：

- 论文正文
- 出版商 / 期刊官网
- DOI 页面
- 正式预印本
- 高校 / 学会 / 官方机构页面

搜索摘要不能替代正文。

## 2. 证据访问状态

所有关键研究至少标记一种：

- 【正文已核】
- 【仅摘要】
- 【仅元数据】
- 【推测】

如果只能获得摘要，不得声称已核实 Methods、Results 或 Discussion 的全文细节。

## 3. Claim–Evidence Gate

最终输出中的每个重要结论都要问：

> 这句话是否真的由当前证据支持？

尤其警惕：

- 修改成功 → 学习
- 相关 → 因果
- 态度 → 能力
- 同任务表现 → 迁移
- 短期变化 → 长期习得
- 公众号摘要 → 作者正式结论
- 单一研究 → 整个领域共识

## 4. 去重

优先：

DOI → 正式题名 → 作者+年份 → 高相似标题。

同一研究的：

- preprint
- accepted manuscript
- Online First
- 正式卷期

原则上归并为一个 canonical record。

## 5. 反证搜索

每轮核心检索至少尝试：

- null results
- no effect
- negative effect
- replication
- methodological criticism
- measurement problem
- boundary condition
- overreliance
- transfer failure

没有反证时如实说没有，不能为了形式完整制造“对立观点”。

## 6. 来源覆盖必须透明

不同学科的来源结构可以不同。

可能包括：

- 中文 / 本地数据库与期刊；
- 国际 / 英文数据库与期刊；
- 其他语言或地区来源；
- 学会、会议、出版社、预印本平台、官方项目页面。

如果 CNKI、Google Scholar、出版社、公众号、会议网站或任何关键来源无法稳定访问：

- 明确写覆盖限制；
- 不要声称“已经完整检索”；
- 尽量用同等级的一手或正式来源补充；
- 不要为了“中英文平衡”而机械加入与研究问题无关的来源。

学术生态的目标是**相关覆盖**，不是固定语言比例。

## 7. 期刊层级

必须区分不同体系：

- JIF / JCR
- CSSCI
- CSSCI扩展版
- 北大核心
- AMI
- 专业领域核心目录

不同体系不得合并成一个未经定义的“A/B/C等级”。

## 8. 宁缺毋滥

允许：

- 本周 0 篇
- 本周无会议
- 本周无直接反证
- 本周 CNKI 未完整覆盖

不允许：

- 为了凑数塞旧文献
- 为了好看虚构覆盖
- 为了输出完整把摘要写成全文
