# 跨平台适配指南

> 适用于 ChatGPT、Codex / Skill、WorkBuddy 类产品、Claude、Gemini，以及其他支持项目指令、Agent 或长任务的 AI。
>
> **核心原则：不要让用户自己来回复制很多文件和链接。能让 AI 直接读取仓库，就把仓库地址一次性写进指令里。**

仓库地址：

```text
https://github.com/YiboCheng2000/research-growth-academic-intelligence-system
```

---

# 先选你的平台

| 你使用什么 | 推荐方式 |
|---|---|
| **ChatGPT** | 让 ChatGPT 读取仓库 → 逐问逐答配置 → 生成最终 Prompt → 创建 Scheduled Task |
| **Codex / Skill** | 让 Codex 读取仓库 → 使用 `skill/` 目录 → 完成个性化 → 按你的环境安装/调用 |
| **WorkBuddy / 深度研究代理** | 让 Agent 读取仓库 → 把周五学术情报和专项深度检索作为长任务运行 |
| **Claude / Gemini / 其他 AI** | 读取仓库或上传核心文件 → 生成个性化配置 → 手动或借助平台自动化运行 |

---

## 一、ChatGPT 用户

## 最省事：直接复制下面这段

```text
我想使用这个 GitHub 项目：

https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

请先读取这个仓库中的：
- README.md
- 00_BEGINNER_SETUP.md
- 02_QUICK_START_CHATGPT.md
- 03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md
- 04_PERSONALIZATION_WORKSHEET.md
- 05_SOURCE_AND_EVIDENCE_POLICY.md

不要直接生成最终提示词。

请一次只问我一个问题，帮我完成个性化配置。
我不懂时给我2—3个简单例子或选项。
不要替我编造研究信息。

全部问完后：
1. 先给我配置摘要；
2. 区分“我的明确选择”和“你的建议”；
3. 等我确认；
4. 自动填好最终 Prompt；
5. 检查是否还有 {{...}}；
6. 再告诉我如何创建 Scheduled Task；
7. 如果当前环境支持直接创建，获得我的明确同意后再执行。
```

## 推荐结构

一个任务，每周一 / 周三 / 周五运行，由星期切换模式：

- 周一：方法与能力
- 周三：研究与发表精读
- 周五：学术情报周报

如果需要邮件、历史查重或其他连接应用，先测试权限，再依赖自动运行。

---

## 二、Codex / Skill 用户

## 先说明：Skill 和定时任务不是一回事

**Skill 负责：**

- 怎么做；
- 什么顺序；
- 什么质量标准；
- 输出什么。

**调度器负责：**

- 什么时候运行；
- 多久运行一次。

本仓库已经提供：

```text
skill/
├── SKILL.md
├── references/
│   ├── PERSONALIZATION_SCHEMA.md
│   └── SOURCE_POLICY.md
└── templates/
    └── OUTPUT_TEMPLATES.md
```

## 直接复制给 Codex

```text
请读取这个 GitHub 仓库：

https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

我要把其中的“研究成长与学术情报系统”用于 Codex / Skill 工作流。

请重点读取：
- skill/SKILL.md
- skill/references/PERSONALIZATION_SCHEMA.md
- skill/references/SOURCE_POLICY.md
- skill/templates/OUTPUT_TEMPLATES.md
- 00_BEGINNER_SETUP.md

然后完成以下工作：

1. 先判断我当前的 Codex 环境是否支持直接使用或安装这个 Skill；
2. 不要假装安装成功；
3. 如果需要本地复制、克隆仓库或放入某个 Skill 目录，请告诉我具体步骤；
4. 在真正安装或改文件前，先一次只问我一个问题，完成个性化配置；
5. 如果我不懂某个字段，给我2—3个例子；
6. 不要替我编造研究信息；
7. 学术生态按我的学科决定，不机械要求中英文50:50；
8. 保留证据核验、反证搜索、去重、信息茧房审计等核心规则；
9. 最后给我一份“已个性化的 Skill 配置摘要”；
10. 等我确认后，再执行你当前环境允许的安装、编辑或调用操作。

如果你无法直接访问 GitHub，请告诉我最少需要下载并上传哪些文件。
```

## Codex 最适合做什么？

- 维护 Skill 版本；
- 管理关键词、来源池和模板；
- 做脚本化去重与元数据清洗；
- 与 GitHub 协作；
- 长期迭代工作流。

---

## 三、WorkBuddy / 深度研究代理

> “WorkBuddy”可能对应不同产品。本仓库不声称和某个具体 WorkBuddy 产品存在官方集成。这里指能够执行多步骤网页研究、文件处理或长任务的 AI Agent。

## 直接复制给你的 WorkBuddy / 深度研究 Agent

```text
请读取这个 GitHub 仓库：

https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

我要把它适配成适合你当前平台能力的研究成长与学术情报工作流。

请重点读取：
- README.md
- 00_BEGINNER_SETUP.md
- 03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md
- 04_PERSONALIZATION_WORKSHEET.md
- 05_SOURCE_AND_EVIDENCE_POLICY.md
- 06_CROSS_PLATFORM_ADAPTATION.md
- 07_GATE6_AUDIT_PROTOCOL.md

请先判断你具备哪些能力：
- 长时间网页检索
- 文件读取
- 数据库访问
- 浏览器操作
- 定时运行
- 邮件/通知
- 历史结果查重

不要假装拥有你没有的能力。

然后：
1. 一次只问我一个问题完成个性化；
2. 帮我判断哪些模块适合自动运行，哪些适合手动触发；
3. 优先把周五学术情报或专项深度检索作为长任务；
4. 保留 Claim–Evidence Gate、Contradiction Search、去重、来源覆盖透明；
5. 学术生态按我的学科和研究问题配置；
6. 最后给我一份适合当前平台的执行方案；
7. 等我确认后再创建或修改工作流。
```

## 适合交给深度研究 Agent 的任务

- 专项深度检索；
- 目标期刊多年盘点；
- 批量拆解文献；
- 制作证据台账；
- 检查长期研究趋势；
- 对某个方法问题做专项审计。

---

## 四、Claude / Gemini / 其他 AI

## 如果你的 AI 能读取 GitHub

直接复制：

```text
请读取这个 GitHub 仓库：

https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

请先阅读 README.md 和 00_BEGINNER_SETUP.md，
再判断你当前平台支持哪些能力。

如果你支持项目指令、持久工作区、Agent、定时器或连接应用，
请把仓库中的工作流适配到这些能力；
如果不支持，就保留为手动触发的周一 / 周三 / 周五模式。

请先逐问逐答完成我的个性化配置，
不要替我编造研究信息，
最后再生成可直接使用的版本。
```

## 如果你的 AI 不能读取 GitHub

上传这四个文件即可开始：

- `03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md`
- `04_PERSONALIZATION_WORKSHEET.md`
- `05_SOURCE_AND_EVIDENCE_POLICY.md`
- `06_CROSS_PLATFORM_ADAPTATION.md`

然后告诉它：

```text
这些文件来自：
https://github.com/YiboCheng2000/research-growth-academic-intelligence-system

请基于我上传的文件完成个性化配置。
缺少必要信息时先问我，不要自行补写。
```

---

## 五、不同使用习惯怎么改

## 轻量用户

可以只保留：

- 周三精读；
- 周五周报。

## 方法导向用户

提高：

- 周一方法学习权重；
- 方法类期刊；
- 测量、统计、研究设计内容。

## 纯文献跟踪用户

可以只运行周五，但仍保留：

- 去重；
- Claim–Evidence Gate；
- Contradiction Search；
- Outside the thesis；
- 每月覆盖审计。

## 博士申请用户

可以增加：

- 导师 / 项目；
- funding；
- summer school；
- conference；
- 申请窗口。

但不要让申请信息挤占核心研究内容。

## 企业研究 / 产品研究用户

可以增加：

- 技术报告；
- benchmark；
- 产业研究；
- 产品文档；
- 岗位技能信号。

把“成果池”改成“项目 / 能力 / 职业素材池”。

---

## 六、跨平台时不要照搬什么？

以下内容必须按平台能力改：

- 工具名称；
- 邮件连接方式；
- 数据库登录能力；
- 本地文件访问；
- 定时任务语法；
- Skill 安装路径；
- 审批和权限逻辑。

**核心协议可以迁移，工具调用细节不能假设。**
