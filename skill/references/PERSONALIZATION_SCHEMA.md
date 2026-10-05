# 个性化配置字段

> 给 Skill / Agent 使用的最小个性化结构。

如果使用者不懂这些字段，可以直接复制下面这段给 AI：

```text
请读取这个仓库：
https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

请根据 skill/references/PERSONALIZATION_SCHEMA.md
一次只问我一个问题，帮我完成个性化配置。

我不懂时请给我例子或选项。
不要替我编造信息。
全部问完后先给我配置摘要，等我确认。
```

## 必填字段

| 字段 | 含义 |
|---|---|
| `user_stage` | 用户当前阶段 |
| `current_project` | 当前论文、项目或长期任务 |
| `core_research_chain` | 核心研究问题、变量或逻辑链 |
| `frozen_boundaries` | 已稳定、不应轻易改动的边界 |
| `review_triggers` | 哪些新证据出现时才需要复核 |
| `output_pool_A` | 候选成果方向 A |
| `output_pool_B` | 候选成果方向 B |
| `academic_ecosystem_strategy` | 学术生态策略 |
| `local_or_chinese_sources` | 中文 / 本地来源 |
| `international_or_english_sources` | 国际 / 英文来源 |
| `other_language_or_region_sources` | 其他语言 / 地区来源 |
| `adjacent_fields` | 邻近领域 / 防信息茧房方向 |
| `contradiction_keywords` | 反证关键词 |
| `methods_capability_pool` | 方法与能力学习池 |
| `weekly_time_budget` | 每周时间预算 |
| `output_language` | 输出语言 |
| `delivery_channel` | 邮件、通知、手动运行等交付方式 |
| `history_dedup_allowed` | 是否允许查历史做去重 |
| `explicit_feedback_rules` | 哪些用户反馈可以改变后续权重 |

## 推荐约束

- 长期成果池：原则上不超过 3 个
- 每周核心研究：0–5 项
- Outside the thesis：0–1 项
- 每周行动：最多 1 项
- 周三精读：每次 1 篇
- 不机械要求中文 / 英文 50:50
