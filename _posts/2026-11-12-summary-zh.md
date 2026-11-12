---
layout: default
title: "Horizon Summary: 2026-11-12 (ZH)"
date: 2026-11-12
lang: zh
---

> 从 38 条内容中筛选出 8 条重要资讯。

---

**Agentic CRM 与竞品**
1. [Salesforce 披露研发智能体](#item-crm-vendors-1) ⭐️ 8.0/10

**企业 AI 平台与运行时**
1. [Databricks 发布新版 Genie](#item-ai-platform-1) ⭐️ 8.0/10
2. [Genie 公布企业数据评测结果](#item-ai-platform-2) ⭐️ 8.0/10
3. [aiXcoder 开源上下文压缩模型](#item-ai-platform-3) ⭐️ 7.0/10

**本体、语义层与知识图谱**
1. [Neo4j 推出 Relate 嵌入式图数据库](#item-ontology-1) ⭐️ 8.0/10

**Agent 协议与开发生态**
1. [MCP 规范改为半年发布一次](#item-protocols-1) ⭐️ 7.0/10

**分析师与研究**
1. [清华、伯克利据称开源 RUA 框架](#item-research-1) ⭐️ 7.0/10
2. [GEAR：模块化智能体自改进框架](#item-research-2) ⭐️ 7.0/10

---

## Agentic CRM 与竞品

<a id="item-crm-vendors-1"></a>
### [Salesforce 披露研发智能体](https://www.salesforce.com/news/stories/agents-that-improve-ai-models/) ⭐️ 8.0/10

Salesforce AI Research 披露 SFR-AutoR&amp;D 研发智能体系统：在给定目标、待优化系统和计算预算后，自主提出假设、修改代码，并通过与基线对照的实验验证改进。Salesforce 称，该系统已用于改进 Data Cloud 检索所用的生产模型 SFR-Embedding V3，并以开源模型 EmbeddingGemma 2 为基础生成 SFR-Embedding v4，后者的质量与延迟均有改善，但所提供正文未给出具体指标。厂商还称，该系统自主完成嵌入模型改进周期约需 80 小时；这类内部应用面向企业检索模型和底层软件的研发迭代，材料未说明系统是否对外开放或提供可购买的产品能力。

rss · Salesforce News · 11月11日 16:00

**「背景」** 嵌入模型将文本转换为数值表示，用于从企业数据中检索相关记录、文档或历史工单。Salesforce 在原文中说明，Agentforce 基于客户自有数据回答问题时，会通过 Data Cloud 检索信息，而 SFR-Embedding V3 正是这一检索环节使用的模型，因此此次研发智能体优化的对象涉及企业问答的数据检索基础能力。

**「竞争启示」** SFR-AutoR&amp;D 将代码优化与模型训练探索分工给 AutoR&amp;D-Engineer 和 TrainForge，并由 AutoInfra 统一承载共享 GPU 上的实验；其中 TrainForge 使用不参与训练的留出基准评估候选方案，体现了执行、算力调度与评估相分离的设计。对企业 AI 平台而言，可参考的是把研发智能体的改动纳入基线对照与证据门槛；不过，材料未披露具体安全验证方法，不能据此认定其已具备完整的生产发布治理机制。

**标签**: `#Salesforce`, `#研发智能体`, `#自主模型优化`, `#Data Cloud`, `#嵌入模型`

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [Databricks 发布新版 Genie](https://www.databricks.com/blog/new-genie-autonomous-ai-complex-enterprise-work) ⭐️ 8.0/10

Databricks 宣布推出新版 Genie，将其定位为持续处理长期企业任务的自主 AI 协作者；据厂商介绍，它可按计划或事件触发任务，跟踪进展、追补缺失输入，并在需要时请求人工批准，用户可通过 Genie One、邮件、Slack 和 Microsoft Teams 与其交互。Genie Ontology 提供业务定义、指标和关系等上下文，Genie Search 跨湖仓及已连接的业务系统检索信息，Unity Gateway 与 Unity Catalog 则用于权限和策略治理，其中 Unity Gateway 支持工具访问控制、行动追踪和支出限制。厂商列举的场景包括保险理赔风险监测、营销活动表现调查及预算调整提案，但所给材料未说明新版的具体可用范围、定价或客户验证；文中“数千家客户在生产中使用 Genie”的说法不能直接视为新版自治能力的落地证明。

rss · Databricks Blog · 11月11日 16:00

**「背景」** 2026 年 11 月 10 日的 Horizon 日报曾报道，Genie One 通过 Sendoso MCP Server 将自然语言数据分析与赠礼操作连接起来，流程包含用户预览、批准及执行后追踪，展示了其从数据问答延伸至业务操作的用法。本次 Databricks 则将 Genie 定位进一步扩展为持续处理长期任务的自主协作者，宣称可跟踪进展、追索缺失输入并随新信息采取行动，同时保留人工监督与必要审批；这比此前的单项工具调用流程覆盖了更长的任务周期。

**「平台启示」** Genie 的设计将业务语义、跨系统检索与执行治理分开处理，并将任务的自主执行范围和人工审批要求交由用户在组织规则内设定。对 CRM+AI 产品而言，可参考这种分层方式，把客户与收入指标定义、信息访问权限，以及营销预算调整等行动的审批要求分别建模，避免将“能检索信息”等同于“获准采取行动”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.databricks.com/blog/turn-buying-signals-pipeline-sendoso-gifts-genie-one">2026-11-10 — Genie One 接入 Sendoso</a></li>

</ul>
</details>

**标签**: `#Databricks Genie`, `#企业智能体`, `#长任务执行`, `#业务本体与检索`, `#工具权限与成本治理`

---

<a id="item-ai-platform-2"></a>
### [Genie 公布企业数据评测结果](https://www.databricks.com/blog/genie-genie-ontology-delivers-16-accuracy-less-half-tokens) ⭐️ 8.0/10

Databricks 报告称，在与 Turing 合作构建的企业数据智能体评测中，使用 Genie Ontology 的 Genie 通过率为 91%，两款未具名的前沿智能体分别为 45% 和 58%，且 Genie 的 token 消耗不足对比智能体的一半。评测以虚构的英国能源供应商 Calderwick Energy 为背景，在同一个真实运行的 Databricks 工作区中对每项任务分别运行各智能体 5 次，数据包含数百张表，最大表约有 1.2 亿行，并纳入笔记本、仪表板、已保存的 SQL 查询和文档等分析资产。Genie Ontology 被厂商定位为企业上下文层，可自动提取、组织这些资产中的业务知识，为需要结合收入定义、报表规则或业务例外进行分析的企业问答提供上下文。上述结果属于厂商报告，所给正文已截断，未提供对手名称、任务总量、完整评分规则及配置，也未交代相关能力的版本、价格或可用范围，因此不足以独立复核或推广至其他场景。

rss · Databricks Blog · 11月11日 15:00

**「背景」** Databricks 表示，此前对 Genie 与 Genie Ontology 的评测使用了专有数据集；本次评测改用可分享的任务及配套分析资产，以便其他团队运行同一评测。与主要围绕表和数据管道的既有数据智能体评测不同，本次基准还纳入了 notebook、dashboard、已保存 SQL 查询、文档及其他资产，用于检验智能体能否发现并使用分散的企业业务知识。

**「平台启示」** 这项评测提示，企业数据问答的上下文建模不宜只覆盖表结构，还应纳入仪表板 SQL、笔记本和文档中的业务定义与计算规则；CRM+AI 产品可据此检查其指标口径和业务例外是否进入可检索的上下文层。由于本次对比同时涉及智能体、各自的运行框架和上下文获取方式，现有材料无法将准确率及 token 消耗差异单独归因于 Genie Ontology。

**标签**: `#Databricks Genie`, `#Genie Ontology`, `#企业上下文层`, `#数据智能体评测`, `#Token 成本`

---

<a id="item-ai-platform-3"></a>
### [aiXcoder 开源上下文压缩模型](https://www.jiqizhixin.com/articles/2026-11-11-11) ⭐️ 7.0/10

据所给报道，aiXcoder 开源了 aiXcompact-4B 模型，用于编程 Agent 的上下文压缩，并提供了 GitHub 仓库地址 github.com/aixcoder-plugin/aiXcompact-4B。该模型面向复杂、长执行链路的编程任务，旨在降低上下文带来的 Token 消耗与推理成本。报道标题宣称推理成本降低 78%，但所给正文不完整，未提供评测条件、成本计算口径或独立验证，不能据此认定企业部署可获得同等收益。

rss · 机器之心 · 11月11日 07:35

**「背景」** 原文将编程 Agent 任务复杂化、执行链路拉长带来的 Token 开销增长，作为 aiXcompact-4B 面向上下文压缩的背景，其关注点是 Agent 运行过程中的成本控制。现有正文片段未提供压缩机制、评测条件或任务效果数据，因此标题所称“推理成本直降 78%”仍应视为待核验的效果主张，不能直接作为企业部署的成本预期。

**「平台启示」** 将上下文压缩交给专用模型，为企业 Agent 运行时提供了一种独立优化上下文成本的方案。评估其用于编程 Agent 或 CRM+AI 长链路任务时，需要同时检验压缩后的信息保留程度、任务完成质量，以及计入压缩模型开销后的端到端成本；现有材料尚不足以判断这些权衡。

**标签**: `#Agent上下文压缩`, `#推理成本优化`, `#开源模型`, `#编程Agent`, `#Agent运行时`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [Neo4j 推出 Relate 嵌入式图数据库](https://neo4j.com/blog/news/meet-relate-by-neo4j-an-embedded-database-for-ai-agents/) ⭐️ 8.0/10

Neo4j 在 NODES 2026 宣布推出开源嵌入式图数据库 Relate，定位是让 AI 智能体在本地进程内保存文档、文件、消息、工单、笔记、决策和行动及其关系。Relate 可作为 Python、JavaScript、Rust、Java、Go 或 Swift 应用库运行，也可通过 CLI、WebAssembly 或 MCP 接入；厂商称其无需部署服务器，并提供面向智能体的紧凑输出、行数限制和版本化命令参考。材料还展示了 Claude Code 使用 Relate 为 Google Agent Development Kit 的 24 个直接依赖创建一次性图实例，以分析传递依赖中的安全通告和未维护软件；但当前材料未提供查询接口细节、持久化机制、性能验证或实际客户落地信息。

rss · Neo4j Blog · 11月11日 12:00

**「背景」** 公告将 Relate 的定位放在智能体本地存储这一场景：文档、工单、消息、笔记和行动不仅需要保存，还需要保留引用、决策依据等关联。这里的“嵌入式”指数据库随应用启动和停止，无需单独部署数据库服务器；这与公告所对比的服务器式数据库，以及用 Python 字典或 JSON 文件保存数据的方式有所不同。

**「建模启示」** Relate 将智能体数据存储从仅保存事实的字典或 JSON 文件扩展到同时保存关系，适合用于上下文关联、引用追踪、决策溯源和隔离的临时分析任务。其进程内部署、应用库、CLI 与 MCP 接入方式表明，企业 AI 平台可以把关系数据能力作为智能体运行时的可嵌入组件；不过材料尚不足以判断其在生产级持久化、性能和治理方面的适用范围。

**标签**: `#Neo4j`, `#嵌入式图数据库`, `#智能体上下文`, `#知识图谱`, `#决策追踪`

---

## Agent 协议与开发生态

<a id="item-protocols-1"></a>
### [MCP 规范改为半年发布一次](https://blog.modelcontextprotocol.io/posts/mcp-release-cycle/) ⭐️ 7.0/10

MCP 官方宣布规范将按半年周期发布，通常安排在 3 月和 9 月的最后一个星期二，并将同时公布提案截止日期和 SDK 测试版日期。下一次发布目标为 2027 年 3 月 30 日，计划版本为 2027-03-30；尚未准备好的提案将转入后续版本，不会推迟整个规范发布。官方还设立发布经理角色，协调提案评审和 SDK 实施；这一安排可供企业规划 MCP 客户端、服务端的适配与测试。

rss · MCP Blog · 11月11日 09:00

**「背景」** MCP 规范变更需要提案作者、工作组和多个 SDK 的维护者协同评审、实现与测试；客户端和服务端开发者也依赖 SDK 尝试新能力并反馈。此前，社区需要从会议记录和 GitHub 讨论中拼凑相关时间安排。

**「集成启示」** 固定发布窗口与延期处理机制，为企业安排协议适配和测试提供了时间依据；由于单项提案可能延期，集成计划仍应以实际发布内容为准。官方称常规周期将在发布前八个月启动规划，与上一周期最后两个月重叠，可作为协调规范和 SDK 工作的参考。

**标签**: `#MCP`, `#规范发布周期`, `#协议治理`, `#SDK 生态`, `#企业集成`

---

## 分析师与研究

<a id="item-research-1"></a>
### [清华、伯克利据称开源 RUA 框架](https://www.jiqizhixin.com/articles/2026-11-11-16) ⭐️ 7.0/10

机器之心的文章标题称，清华与伯克利开源了面向 Agentic Robotics 的统一 RUA 框架，研究方向涉及具身智能与机器人智能体架构。但所提供的正文仅有开头片段，未展示 RUA 的架构、开源地址、许可协议或评测结果，尚无法据此确认其具体能力与可用范围。对探索机器人任务执行与智能体编排的企业团队，这是一条可进一步核查的研究线索；现有材料不足以判断其对企业 AI 平台或 CRM+AI 场景的直接适用性。

rss · 机器之心 · 11月11日 11:58

**「背景」** 原文以“机器人自己的 Computer Use 时刻”作类比，将物理机器人控制及完成未经专项训练的任务，作为讨论 Agentic Robotics 的切入点。当前正文摘录尚未展开 RUA 框架的架构、任务范围及评测方法，因此还无法判断这里的“统一”具体覆盖哪些能力，也无法确认其与文中提及的模型控制能力之间的技术关系。

**标签**: `#具身智能`, `#Agentic Robotics`, `#智能体框架`, `#开源研究`, `#机器人控制`

---

<a id="item-research-2"></a>
### [GEAR：模块化智能体自改进框架](https://www.jiqizhixin.com/articles/2026-11-11-8) ⭐️ 7.0/10

机器之心介绍了面向递归自我改进（RSI）的 GEAR 框架，其目标是让研究者像使用 Scikit-learn 一样，以模块化方式构建、比较和复用 RSI 算法。框架将采样、候选评测、多样性管理等算法模块与并行推理等评测基础设施组织起来，适用于智能体持续优化算法的研究与评测。材料提到基于 GEPA（Genetic-Pareto）算法改进的实验，但正文截断，未提供完整结果、对照设置或性能数据，因此无法据此判断改进幅度及企业部署效果。

rss · 机器之心 · 11月11日 06:31

**「背景」** 原文提到的 GEPA（Genetic-Pareto）是一种提示词优化方法，通过对试错过程进行自然语言反思来提炼高层规则，其优化对象是提示词，不应直接等同于底层模型权重的自我更新。已有 Hermes Agent Self-Evolution 项目结合 DSPy 与 GEPA，探索对智能体技能、工具描述、系统提示词和代码进行演化优化，为理解 GEAR 所组织的自我改进流程提供了具体参照。

**「研究启示」** GEAR 将算法模块与评测基础设施分开组织，为企业智能体平台提供了一个可参考的设计点：将采样、候选评测和多样性管理做成可替换组件，并复用并行推理设施来比较优化策略。不过，这种研究框架的模块化设计本身并不代表已具备生产环境所需的治理与安全保障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/NousResearch/hermes-agent-self-evolution">GitHub - NousResearch/hermes- agent - self -evolution: Evolutionary...</a></li>
<li><a href="https://arxiv.org/abs/2507.19457">[2507.19457] GEPA : Reflective Prompt Evolution Can Outperform...</a></li>

</ul>
</details>

**标签**: `#Agent 自我进化`, `#RSI 框架`, `#智能体评测`, `#模块化架构`, `#GEPA`

---