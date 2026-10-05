# 设计参考与公开项目

本系统借鉴的是公开项目的**公开工作流思想与产品设计模式**，不是代码复制，也没有将这些项目的源代码、Prompt 文件或资产直接 vendoring 到本仓库。引用项目不代表它们认可、赞助或参与了本项目。

上游许可证仅用于帮助读者理解各项目自身的许可状态；如果你以后直接复制任何上游代码或受版权保护的文本，应重新核对该项目当时的许可证和归属要求。

## 1. Future-House / PaperQA2

GitHub:
https://github.com/Future-House/paper-qa

上游许可证（核对日期：2026-10-05）：Apache-2.0

借鉴：

- Paper Search
- Gather Evidence
- Generate Answer
- 元数据意识
- 证据排序
- 引用支撑
- 科学文献问答中的 grounded response

迁移到本系统后：

- Candidate Discovery
- Evidence Retrieval
- Claim–Evidence Gate

## 2. Stanford STORM / Co-STORM

GitHub:
https://github.com/stanford-oval/storm

上游许可证（核对日期：2026-10-05）：MIT

借鉴：

- Perspective-Guided Question Asking
- 多视角信息搜集
- 主动发现遗漏问题
- 人与 AI 共同知识整理

迁移后：

- Perspective Expansion
- Outside the thesis
- 每月信息覆盖审计

## 3. ArxivDigest

GitHub:
https://github.com/AutoLLM/ArxivDigest

上游许可证（核对日期：2026-10-05）：MIT

借鉴：

- 根据自然语言研究兴趣做个性化相关性排序
- 定期 digest
- 邮件交付

迁移后：

- 个性化多维相关性筛选
- 周报邮件
- 用户明确反馈校准

## 4. paper-search-mcp

GitHub:
https://github.com/openags/paper-search-mcp

上游许可证（核对日期：2026-10-05）：MIT

借鉴：

- 多来源并行检索
- 去重
- 来源能力透明
- discovery 与 full-text retrieval 分开
- canonical metadata 思维

迁移后：

- DOI/题名/作者年份去重
- 发现源和证据源分离
- 来源覆盖情况报告

## 5. ASReview

GitHub:
https://github.com/asreview/asreview

上游许可证（核对日期：2026-10-05）：Apache-2.0

借鉴：

- human-in-the-loop
- 用户标签参与筛选
- 不把 AI 当成最终 oracle

迁移后：

- 只根据用户明确反馈调整推荐权重
- 沉默不等于掌握
- 未完成不等于能力不足

## 6. Academic Research Skills

GitHub:
https://github.com/Imbad0202/academic-research-skills

上游许可证（核对日期：2026-10-05）：CC BY-NC 4.0

Codex 版本:
https://github.com/Imbad0202/academic-research-skills-codex

借鉴：

- human-in-the-loop
- integrity gate
- source provenance
- citation / claim support
- 质量检查

迁移后：

- Claim–Evidence Gate
- 证据访问状态
- 最终自检

## 7. Awesome AI Literature Review

GitHub:
https://github.com/brycewang-stanford/lit-review-agent-tools

上游许可证（核对日期：2026-10-05）：CC0-1.0

借鉴：

- search
- screen
- extract
- read
- synthesize
- cite-check
- write / review

迁移后：

把“文献检索”拆成多个可审计阶段，而不是一个黑箱 Prompt。

---

## OpenAI 官方资料（用于部署）

Scheduled Tasks:
https://help.openai.com/en/articles/10291617-scheduled-tasks-in-chatgpt

Sharing Scheduled Tasks:
https://help.openai.com/en/articles/7925741-sharing-conversations-and-scheduled-tasks-in-chatgpt

Skills in ChatGPT:
https://help.openai.com/en/articles/20001066-skills-in-chatgpt

Agent Skills API guide:
https://developers.openai.com/api/docs/guides/tools-skills

Plugin Skills concept:
https://developers.openai.com/plugins/concepts/skills

说明：

产品能力可能变化。部署时请以当时的官方文档为准。
