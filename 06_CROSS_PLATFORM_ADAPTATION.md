# 跨平台适配：ChatGPT / 深度研究代理（含部分 WorkBuddy 类产品）/ Codex / 其他 AI

这套系统的核心不是某一个平台，而是一组可迁移的工作流约束。

## 一、ChatGPT

### 最适合

- 定时运行
- 周期性推送
- Web 检索
- 结合支持的连接应用
- 邮件/通知
- 读取本系列历史进行去重（取决于权限）

### 推荐结构

一个任务，每周一/三/五运行，由星期切换模式。

### 优势

- 无需本地电脑保持在线
- 调度、搜索、推送可以放在一个任务中
- 符合条件的任务可以分享给他人

### 注意

分享任务链接时，完整任务指令、计划和时区会被看到。不要把私人邮箱、未公开研究数据等放进公开版。

---

## 二、WorkBuddy 类产品 / 深度研究代理

> “WorkBuddy”不是一个足够唯一的公开产品标识，不同服务可能使用相同或相近名称。本仓库**不提供也不声称提供某个特定 WorkBuddy 产品的官方集成**。以下内容只适用于“能够执行多步骤网页研究、文件处理或长任务的 Agent”这一通用能力类别。使用前请按你实际使用的平台文档核对。

### 最适合

- 专项深度检索
- 大量网页遍历
- 一次性盘点目标期刊近几年文章
- 批量拆解文献
- 制作证据台账
- 检查长时间窗的研究趋势

### 推荐优化

不要直接把巨型 Prompt 每次完整粘贴。

拆为：

1. `CORE_PROTOCOL`：证据规则、反证、去重、输出质量。
2. `PROFILE`：你的研究、目标期刊、关键词、成果池。
3. `TASK`：本次具体检索范围。
4. `OUTPUT_SCHEMA`：最终表格/报告格式。

### 推荐运行方式

- 日常定时：优先使用你已有的稳定调度器（例如符合条件的 ChatGPT Scheduled Tasks）
- 每月/每季度深度盘点：可交给支持长任务的深度研究 Agent
- 出现重大方法问题：可让深度研究 Agent 做专项审计

如果平台没有稳定的无人值守调度，不要把它伪装成自动任务。

---

## 三、Codex / Agent Skill

### 最适合

- 把工作流变成可版本管理的 Skill
- 维护多个配置文件
- 维护关键词、来源池、模板
- 做脚本化去重、元数据清洗
- 与 GitHub 仓库协作
- 长期迭代 Prompt / Skill

### 推荐目录

```text
research-growth-academic-intelligence/
├── SKILL.md
├── references/
│   ├── SOURCE_POLICY.md
│   └── PERSONALIZATION_SCHEMA.md
└── templates/
    └── OUTPUT_TEMPLATES.md
```

本套件已经提供这个最小结构。它是**可移植的 Skill 起点**，不是某个 Codex 版本已经安装好的插件，也不保证可直接拖入所有 ChatGPT 账户。当前 OpenAI 产品中，Skill 的可用性、安装和同步方式会因 ChatGPT、Codex、API、计划及工作空间设置而异。

### Skill 与自动化的区别

Skill 负责：

- 怎么做
- 什么顺序
- 什么质量标准
- 输出什么

调度器负责：

- 什么时候运行
- 多久运行一次

不要把两者混为一谈。

---

## 四、Claude / Gemini / 其他支持项目指令的 AI

如果支持：

- Project Instructions
- System Prompt
- Persistent Workspace
- Custom Agent

可以把：

- `03_CHATGPT_AUTOMATION_PROMPT_TEMPLATE.md`
- `04_PERSONALIZATION_WORKSHEET.md`
- `05_SOURCE_AND_EVIDENCE_POLICY.md`

组合使用。

如果不支持定时任务：

每周手动触发：

- “运行周一模式”
- “运行周三模式”
- “运行周五模式”

如果支持外部自动化平台，可让外部平台负责调度，AI 只负责执行研究协议。

---

## 五、不同使用习惯怎么改

### 轻量用户

只保留：

- 周三精读
- 周五周报

删除周一能力模块。

### 方法导向用户

提高：

- 周一频率
- 方法类期刊
- psychometrics / research methods / statistics 权重

降低新闻类内容。

### 纯文献跟踪用户

可以只运行周五，但仍保留：

- 去重
- Claim–Evidence
- Contradiction Search
- Outside the thesis
- 每月覆盖审计

### 博士申请用户

增加：

- 导师/项目
- funding
- summer school
- conference
- 招生/申请窗口

但不要让申请信息挤占核心研究内容。

### 企业研究 / 产品研究用户

增加：

- 技术报告
- benchmark
- 产业研究
- 产品文档
- 岗位技能信号

把“成果池”改为“项目/能力/职业素材池”。

---

## 六、不要跨平台照搬的部分

以下内容应按平台能力改写：

- 具体工具名
- 邮件连接方式
- 数据库登录能力
- 本地文件访问
- 定时任务语法
- Skill 安装路径
- 审批/权限逻辑

核心协议可迁移，工具调用细节不要假设。
