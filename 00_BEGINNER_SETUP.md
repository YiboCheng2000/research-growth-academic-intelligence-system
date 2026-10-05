# 00｜零基础配置指南

> **第一次使用？不要先改 Prompt。**
>
> 你只需要把本页的一段指令复制给你的 **AI / AI Agent**。  
> 让它先了解你，再自动完成配置。

## 30 秒看懂

| 第一步 | 第二步 | 第三步 |
|---|---|---|
| **复制下面的通用指令** | **AI 一次只问一个问题** | **确认配置后再部署** |
| 不用自己找仓库链接 | 不懂就让 AI 给例子 | 不要一上来修改大段模板 |

---

## A｜最推荐：只复制这一段

如果你的 AI 能读取 GitHub，**只复制下面整个代码块即可**。仓库地址已经写好了。

```text
我想使用这个 GitHub 项目：

https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

项目名称：
Research Growth & Academic Intelligence System

请先判断你是否能直接读取这个 GitHub 仓库。

如果可以，请重点阅读：
- README.md
- 00_BEGINNER_SETUP.md
- 03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md
- 04_PERSONALIZATION_WORKSHEET.md
- 05_SOURCE_AND_EVIDENCE_POLICY.md
- 06_CROSS_PLATFORM_ADAPTATION.md

不要立刻生成最终提示词。

请把配置过程当成一次简短访谈：
1. 一次只问我一个问题；
2. 用普通中文解释，不要默认我懂 Prompt、研究方法或数据库；
3. 我不知道怎么回答时，给我 2—3 个具体例子或选项；
4. 不要替我编造研究信息；
5. 你可以提出建议，但必须标记“建议，待我确认”。

你至少需要问清楚：
A. 我现在是什么阶段；
B. 我当前最重要的研究 / 学习任务；
C. 当前研究题目、核心问题或长期关注主题；
D. 哪些内容已经基本确定，不希望被每周新信息随意改变；
E. 我未来可能形成哪些独立成果、能力或职业方向；
F. 我的学科应该重点覆盖什么学术生态：
   - 中文 / 本地来源优先
   - 中文与国际双轨
   - 国际 / 英文来源优先
   - 其他语言 / 地区来源
   - 或由你根据我的学科提出建议
G. 我应该重点追踪哪些数据库、期刊、学会、会议和官方渠道；
H. 我最担心形成哪一种信息茧房；
I. 我未来最想补哪些方法、统计、AI 或数据能力；
J. 我每周最多愿意投入多少时间；
K. 我希望通过什么方式收到结果；
L. 我当前使用的平台是否支持定时任务、文件、浏览器、邮件或其他连接能力。

特别规则：
- 不要默认所有学科都需要同样比例的中文和英文来源；
- 不要为了“平衡”机械追求 50:50；
- 按我的学科和研究问题决定来源结构；
- 如果还需要其他语言或地区来源，也要纳入；
- 不要删除证据核验、反证搜索、去重、信息茧房审计等核心质量规则。

全部问题问完后：
第一步：给我一份“个性化配置摘要”；
第二步：区分“我的明确选择”和“你的建议”；
第三步：等我确认；
第四步：自动把配置填入 03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md；
第五步：检查最终版本中是否还残留任何 {{...}}；
第六步：根据我实际使用的平台给出部署方式；
第七步：如果平台支持自动创建任务，在获得我的明确同意后再创建。

如果你不能读取 GitHub：
直接告诉我最少需要上传哪些文件，不要假装已经读取。

现在请不要输出大段说明，先从第一个配置问题开始。
```

---

<details>
<summary><strong>B｜如果你的 AI 不能读取 GitHub，点这里</strong></summary>

先下载并上传：

1. `03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md`
2. `04_PERSONALIZATION_WORKSHEET.md`
3. `05_SOURCE_AND_EVIDENCE_POLICY.md`
4. `06_CROSS_PLATFORM_ADAPTATION.md`

然后只复制：

```text
我已经上传了“Research Growth & Academic Intelligence System”的核心配置文件。

原始仓库：
https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

请根据我上传的文件完成个性化配置。

一次只问我一个问题；
我不懂时给我例子或选项；
不要替我编造研究信息。

全部问题问完后：
1. 先给我配置摘要；
2. 区分“我的明确选择”和“你的建议”；
3. 等我确认；
4. 自动填好模板；
5. 检查是否还有 {{...}}；
6. 根据我使用的平台给出部署方式。
```

</details>

---

## C｜你到底需要自定义什么？

| **需要换成你自己的** | **新手先不要动** |
|---|---|
| 当前论文 / 项目 / 长期研究主题 | 发现源 ≠ 证据源 |
| 已稳定的研究边界 | 主张—证据核验（Claim–Evidence Gate） |
| 后续成果 / 能力 / 职业方向 | 反证搜索（Contradiction Search） |
| 学术生态与来源池 | 证据状态（Evidence Status） |
| 方法、统计、AI、数据能力池 | 文献去重 |
| 每周时间预算 | 研究外拓（Outside the thesis） |
| 邮件 / 通知 / 手动运行方式 | 每月信息覆盖审计 |
| 当前 AI 平台能力 | “相关 ≠ 因果”“宁缺毋滥”等边界规则 |

> **先改“你是谁”，不要先改“系统怎么保证质量”。**

---

<details>
<summary><strong>D｜什么是 {{...}} 占位符？点这里看例子</strong></summary>

模板里可能写：

```text
当前研究主题：
{{当前研究题目/问题}}
```

假设你的研究是：

```text
大学生使用生成式人工智能写作反馈的采纳行为
```

最终应变成：

```text
当前研究主题：
大学生使用生成式人工智能写作反馈的采纳行为
```

再例如：

```text
统一时区：{{时区}}
```

可以变成：

```text
统一时区：Asia/Shanghai
```

**但新手不用自己逐个替换。让 AI 自动做。**

</details>

---

<details>
<summary><strong>E｜不知道该关注中文、英文还是其他学术生态？点这里</strong></summary>

不要机械追求“中英文各一半”。

### 示例 1｜国际中文教育 / 中国本土教育议题

可能适合：

**中文 / 本地 + 国际 / 英文双轨**

因为中文期刊、国内学会、会议，以及国际 SLA / CALL / writing research 都可能重要。

### 示例 2｜计算机科学 / AI / NLP

可能适合：

**国际 / 英文来源优先**

重点可能是：

- arXiv
- ACL Anthology
- 顶级会议
- 期刊
- benchmark
- technical report

中文来源可以是补充，不必强制占一半。

### 示例 3｜区域研究 / 小语种研究

可能适合：

**中文 + 英文 + 目标地区语言**

因此真正的问题不是：

> “中文和英文各占多少？”

而是：

> **“你的学科需要覆盖哪些语言、地区和学术共同体？”**

</details>

---

## F｜配置完成后怎么部署？

| 你使用的平台 | 下一步 |
|---|---|
| **ChatGPT** | [ChatGPT 快速部署指南](02_QUICK_START_CHATGPT.md) |
| **Codex / Skill** | [中文 Skill 配置页](skill/SKILL.md) |
| **WorkBuddy / 深度研究代理** | [跨平台适配指南](06_CROSS_PLATFORM_ADAPTATION.md) |
| **Claude / Gemini / 其他 AI** | [跨平台适配指南](06_CROSS_PLATFORM_ADAPTATION.md) |

---

## G｜运行后不要立刻重构

建议先运行 **2–4 周**，再看真实问题。

之后直接使用：

**→ [Gate 6｜真实运行审计](07_GATE6_AUDIT_PROTOCOL.md)**

检查：

- 是否重复；
- 是否把摘要当全文；
- 学术生态是否真的覆盖；
- 是否总是推支持当前观点的研究；
- 输出是否太长；
- 是否真正帮助研究和成果转化。

---

## H｜如果你现在只想马上开始

最后再给你一份最短指令：

```text
我完全不会配置这个项目：

https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

如果你能读取 GitHub，请先阅读 README.md 和 00_BEGINNER_SETUP.md；
如果不能，请告诉我最少需要上传哪些文件。

然后一次只问我一个问题。
我不懂时给我例子或选项。
不要替我编造信息。

最后先让我确认个性化配置，
再帮我生成可直接使用的最终版本。
```

**你不需要先学会写 Prompt，才能使用这套系统。**
