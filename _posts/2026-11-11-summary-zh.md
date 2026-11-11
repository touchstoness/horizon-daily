---
layout: default
title: "Horizon Summary: 2026-11-11 (ZH)"
date: 2026-11-11
lang: zh
---

> 从 29 条内容中筛选出 9 条重要资讯。

---

**Agentic CRM 与竞品**
1. [Sales Cloud 公布智能体调研](#item-crm-vendors-1) ⭐️ 6.0/10
2. [Missionforce 招募方案获采购资格](#item-crm-vendors-2) ⭐️ 6.0/10
3. [ChatGPT 介绍企业信息管理](#item-crm-vendors-3) ⭐️ 6.0/10

**企业 AI 平台与运行时**
1. [AgentCore 依赖监控方案](#item-ai-platform-1) ⭐️ 8.0/10
2. [Unity Catalog 指标接入 Power BI](#item-ai-platform-2) ⭐️ 7.0/10
3. [openJiuwen 宣称首发 TTSE 框架](#item-ai-platform-3) ⭐️ 6.0/10

**本体、语义层与知识图谱**
1. [AuraDB 高内存实例正式商用](#item-ontology-1) ⭐️ 8.0/10
2. [Neo4j 示范本体知识层](#item-ontology-2) ⭐️ 7.0/10

**AI 评测、治理与安全**
1. [WorkflowArena 编排基准发布](#item-governance-1) ⭐️ 6.0/10

---

## Agentic CRM 与竞品

<a id="item-crm-vendors-1"></a>
### [Sales Cloud 公布智能体调研](https://www.salesforce.com/news/stories/how-ai-agents-improve-crm-data-accuracy/) ⭐️ 6.0/10

Salesforce 发布《The ROI Report: Sales Cloud Agents》，对 24 家正在使用 Sales Cloud AI 销售智能体的客户开展 ROI 调研，称智能体承担 CRM 更新等行政任务后，销售人员平均每周节省 6 小时。63% 的受访客户表示 CRM 数据更准确、完整，57% 的受访销售负责人认为智能体有助于在不增加员工人数的情况下提升收入。材料描述的应用包括潜客开发、客户研究、销售管道管理，以及将对话和客户研究自动记录到 Salesforce，适用于希望减少销售行政负担、补全商机信息的企业。上述收益来自厂商组织的客户调研，所给材料未披露详细统计方法、具体功能配置或独立验证，不能据此认定所有部署均能取得同等效果。

rss · Salesforce News · 11月10日 17:00

**「背景」** 销售预测和商机管道管理依赖销售人员及时录入客户互动与交易进展；原文指出，人工更新容易造成关键信息延迟、缺失或不可靠，Sales Cloud 智能体则通过自动记录对话和客户研究信息来补充 CRM 数据。本次 ROI 报告依据 Salesforce 对 24 家已使用其销售智能体的客户所做的调查，反映的是受访客户报告的体验，所给材料未披露对照组、统计方法或独立验证。

**「竞争启示」** 材料将自动记录对话和客户研究与 CRM 数据完整性、管道可见性联系起来，为 CRM+AI 产品提供了一个具体设计参考：让智能体执行销售任务时同步回写业务上下文。评估此类能力时，可同时衡量销售人员节省的时间和 CRM 数据质量；本次调研提供了这两类指标的客户反馈，但尚不足以证明其因果关系。

**标签**: `#Salesforce`, `#Sales Cloud`, `#销售智能体`, `#CRM数据质量`, `#ROI调研`

---

<a id="item-crm-vendors-2"></a>
### [Missionforce 招募方案获采购资格](https://www.salesforce.com/news/press-releases/2026/11/10/missionforce-achieves-awardable-status/) ⭐️ 6.0/10

Salesforce 宣布，Missionforce National Security 人员招募方案在美国首席数字与人工智能办公室（CDAO）的 Tradewinds Solutions Marketplace 获得“Awardable”资格，相关国防组织可通过该市场直接获取其招募解决方案。该方案面向军事人员招募与留任，Salesforce 称其获得影响级别 5（IL5）授权，并具备招募活动生成、候选人资格核验和人员流失风险分析等能力。公告未披露价格、实施规模或可复核的实际成效。

rss · Salesforce News · 11月10日 14:00

**「背景」** Tradewinds Solutions Marketplace 是 CDAO 用于加速政府采购和采用人工智能、机器学习及数据分析等技术的渠道，平台会评估面向政府任务的技术方案。“Awardable”表示方案具备通过该市场被采购的资格，并不代表已经获得采购合同；Empower AI 等供应商也已取得这一资格，因此本次公告应理解为 Salesforce 招募方案的采购渠道进展。

**「竞争启示」** 该方案将现有系统和人员数据接入、招募全流程分析与自动化相结合，并强调对智能体操作保留人工监督。对面向敏感场景的 CRM+AI 产品而言，这提供了一种将数据集成、业务流程和治理要求共同设计的参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.executivebiz.com/articles/empower-ai-ida-awardable-tradewinds">Empower AI Earns Awardable Status on Tradewinds Marketplace</a></li>
<li><a href="https://www.min.io/blog/why-awardable-matters-for-solutions-powering-government-agencies">Why “ Awardable ” Matters for Solutions Powering Government Agencies</a></li>

</ul>
</details>

**标签**: `#Salesforce`, `#Missionforce`, `#政府CRM`, `#人才招募`, `#AI采购市场`

---

<a id="item-crm-vendors-3"></a>
### [ChatGPT 介绍企业信息管理](https://openai.com/index/introducing-businesses-chatgpt) ⭐️ 6.0/10

OpenAI 介绍了 Businesses in ChatGPT，称企业可在 ChatGPT 中管理自身业务信息、了解企业信息的展示情况，并推动用户从表达兴趣转向采取行动。这些能力面向企业信息维护、品牌展示分析和潜在客户触达场景，但所提供的材料未说明具体操作方式、开放范围、价格或上线状态，也未披露是否支持线索采集及 CRM 集成。

rss · OpenAI News · 11月10日 10:00

**「背景」** OpenAI 官方介绍将 Businesses in ChatGPT 标注为测试版（beta），并称 ChatGPT 每周有 12 亿用户，以此说明企业在该平台触达用户的潜在范围。该数字是平台整体的周用户规模，不能据此判断参与企业实际获得的曝光或转化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-businesses-chatgpt/">Introducing Businesses in ChatGPT | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#企业信息管理`, `#客户转化`

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [AgentCore 依赖监控方案](https://aws.amazon.com/blogs/machine-learning/build-a-daily-dependency-watcher-with-langgraph-and-amazon-bedrock-agentcore-web-search/) ⭐️ 8.0/10

AWS 宣布 Amazon Bedrock AgentCore Web Search API 已可用，并展示如何结合 LangGraph 构建每日依赖监控智能体，为安全团队检查 npm、PyPI 和容器基础镜像的最新风险信息。该 API 使用 AWS 凭证签名调用，返回包含标题、URL、发布日期和相关摘录的搜索结果，支持域名包含或排除及发布日期范围限制；AWS 表示，查询由 Amazon 自营网页索引处理，不会发送给第三方搜索引擎。示例并行运行三个研究分支，每个分支最多搜索四次，再校验发现与引用来源是否一致、过滤时间窗口外的信息，并通过 LangGraph 存储记录已报告内容以避免重复。方案还演示在 AgentCore Runtime 上运行，并通过 AgentCore Gateway 向多个团队提供访问；AWS 报告其测试中三个分支并行耗时 36 秒，串行耗时 99 秒，这属于该示例的测试结果。

rss · AWS Machine Learning Blog · 11月10日 23:34

**「背景」** 依赖项监控需要及时发现新发布的安全公告和版本变化，而模型的训练数据无法覆盖发布后的动态。示例中，LangGraph 负责并行编排各软件生态的检索任务，AgentCore Web Search API 则返回带有网址、发布日期和相关摘录的网页结果，供工作流核对发现并生成引用。

**「平台启示」** 该方案将搜索词选择和发现撰写交给模型，同时把时间窗口、来源屏蔽列表、搜索预算及结果校验保留在代码中，为企业智能体提供了明确的控制边界。对于需要持续跟踪外部信息的 CRM+AI 功能，可参考其来源约束、引用校验和历史去重机制；通过 AgentCore Gateway 配置统一来源策略，也能让多个智能体及 MCP 客户端共享管理员设定的来源规则。

**标签**: `#Amazon Bedrock AgentCore`, `#LangGraph`, `#智能体工具调用`, `#企业级网页搜索`, `#来源治理`

---

<a id="item-ai-platform-2"></a>
### [Unity Catalog 指标接入 Power BI](https://www.databricks.com/blog/unity-catalog-metric-views-now-power-bi-one-unified-governed-semantic-layer-all-your-reporting) ⭐️ 7.0/10

Databricks 宣布推出 Publish to Power BI，可将 Unity Catalog 指标视图直接发布为 Power BI 语义模型，让企业集中定义收入、利润率和活跃客户数等 KPI，并用于报表与 AI 应用。每个指标视图映射为模型中的一张表，维度映射为列，度量映射为 DAX 度量；Power BI 查询指标视图，视图中定义的联接仍在 Databricks 执行。用户可从 Catalog Explorer 按需发布，也可在 Lakeflow Job 中加入 Power BI 任务，在指标定义更新后重新发布，适用于销售收入核对、营销渠道及区域 ROAS 分析等场景。正文将这些发布方式描述为当前能力，但未交代具体可用范围和权限传递机制；指标视图物化带来的性能优化则属于后续预告。

rss · Databricks Blog · 11月10日 18:45

**「背景」** Unity Catalog 指标视图是位于 Databricks Lakehouse 之上的治理型语义层，用于集中定义业务指标、维度及关联关系，并供 AI/BI Dashboards 和 Genie 等应用使用。Databricks 称，企业过去常在多个 Power BI 工作区和语义模型中重复维护 DAX 指标与表关系，容易造成同一 KPI 的定义分散和报表口径漂移。

**「平台启示」** 这一集成将 KPI 定义和联接逻辑集中在 Unity Catalog，将报表制作保留在 Power BI，为 CRM 报表与 AI 分析共享业务口径提供了具体的分层方式。指标变更后通过 Lakeflow Job 重新发布的机制也表明，统一口径需要维护从指标定义到下游语义模型的同步流程；设计类似平台时，应将这一步纳入生产数据管道。

**标签**: `#Databricks Unity Catalog`, `#Power BI 语义模型`, `#指标视图`, `#KPI 治理`, `#企业 AI 语义层`

---

<a id="item-ai-platform-3"></a>
### [openJiuwen 宣称首发 TTSE 框架](https://www.qbitai.com/2026/11/508998.html) ⭐️ 6.0/10

该条目标题宣称 openJiuwen 首发 TTSE 经验学习框架，指向利用任务经验推动 Agent 持续改进的方向。所提供正文仅有“让每一次任务，都成为下一次进步的起点”一句宣传语，未说明学习机制、发布状态、可用范围或效果验证。对于需要积累任务经验、持续优化 Agent 的企业团队，这可作为后续关注的产品线索，但现有材料不足以判断其运行时集成方式及实际适用性。

rss · 量子位 · 11月10日 07:56

**「背景」** openJiuwen 官网将其定位为面向生产级 AI Agent 构建的平台。此次条目所称的 TTSE 经验学习框架与 Agent 持续改进有关，但所给正文仅有宣传语，尚不足以确认其学习机制、与平台的集成方式或可用状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openjiuwen.com/en/">openJiuwen</a></li>

</ul>
</details>

**标签**: `#openJiuwen`, `#TTSE`, `#Agent自演进`, `#经验学习`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [AuraDB 高内存实例正式商用](https://neo4j.com/blog/graph-database/auradb-high-memory-instances-with-up-to-2tb-of-ram-now-generally-available/) ⭐️ 8.0/10

Neo4j 宣布，AuraDB Business Critical 和 Virtual Dedicated Cloud 套餐的 High Memory 实例现已在 AWS 和 Google Cloud 正式可用，最高内存分别为 2,048 GB 和 1,952 GB。两项套餐在 AWS、Google Cloud 和 Azure 上的存储上限也从 2 TB 提升至 5 TB，适用于内存至少为 192 GB 的实例，并受 1:16 的内存与存储比例限制。高内存实例面向采用预付费条款的客户开放，启用前需确认所在区域的云资源容量，公告未给出具体单价或性能基准。此次扩容适用于大型知识图谱、GraphRAG、反欺诈及客户 360 图谱，也为大型自管 Neo4j 部署迁入托管服务提供了容量选择。

rss · Neo4j Blog · 11月10日 12:51

**「背景」** 据公告，高内存实例已于今年早些时候在 Google Cloud 推出，此次新增 AWS 正式可用；此前用户可自行创建的实例内存上限为 512 GB。图查询需要沿关系遍历并检索关联上下文，Neo4j 将此次扩容的价值归结为让频繁访问的节点、关系和索引尽量驻留内存，但未提供量化性能对比。

**「建模启示」** AuraDB 允许在创建或调整实例时分别设置内存和存储：内存按 GB·小时计费，包含按 1:2 内存与存储比例配置的磁盘容量，额外存储另按 GB·小时计费。对知识图谱和 CRM 客户 360 的容量规划，这提供了将查询工作集所需内存与历史数据所需存储分别估算的依据，但仍需遵守实例容量及比例限制。

**标签**: `#Neo4j AuraDB`, `#托管图数据库`, `#高内存实例`, `#知识图谱扩容`, `#客户360`

---

<a id="item-ontology-2"></a>
### [Neo4j 示范本体知识层](https://neo4j.com/blog/graph-database/build-a-knowledge-layer-map-your-data-with-an-ontology/) ⭐️ 7.0/10

Neo4j 官方博客以虚构的企业贷款审批为例，提出用本体图为跨数据库 AI 智能体建立知识层，使其在查询前识别数据源、实体及其业务关系，而不必把全部语义写入提示词或为每个数据源定制工具。示例采用 DataProduct 和 SchemaEntity 两类节点、通用 RELATES 关系，以及 RESOLVES、SUPPLEMENTS、GOVERNS、CITES 四类数据源关系，覆盖银行交易、KYC、商业计划、贷款政策和历史决策等信息。文章属于配有 knowledge-layer-demo GitHub 代码的方案教程，并非新产品能力发布；案例明确为虚构，正文未提供客户落地或效果验证。

rss · Neo4j Blog · 11月10日 14:00

**「背景」** 在传统业务应用中，字段的含义往往写在应用代码里，业务人员也能凭经验理解；跨库智能体查询时，单看字段名往往无法判断它代表什么、该去哪个系统找相关信息。本体图为此提供了一份可查询的业务地图，把各系统中的业务对象及其关系显式记录下来，例如标明哪套贷款政策约束哪类银行业务。

**「建模启示」** 对 CRM+AI 平台而言，可以将“数据源级关系”与“源内业务实体关系”分层建模：前者帮助智能体判断应查询、补充或遵循哪个系统，后者描述客户、贷款等对象如何关联。用通用关系类型承载具体关系名称，也有助于在数据源变化时减少对统一语义层结构的硬编码。

**标签**: `#本体建模`, `#知识层`, `#智能体上下文`, `#Neo4j`, `#跨数据库语义`

---

## AI 评测、治理与安全

<a id="item-governance-1"></a>
### [WorkflowArena 编排基准发布](https://www.jiqizhixin.com/articles/2026-11-10-9) ⭐️ 6.0/10

Einsia AI 发布多智能体编排基准 WorkflowArena，用于关注模型自主组织和调度子智能体的能力，包括任务拆解、上下文分配、中间结果校验与最终结果整合。材料未披露基准任务、评分方法、测试结果、价格或开放范围，因此目前无法复核其评测有效性及模型表现。标题将其称为“行业首个”，但这是厂商或报道方的主张；该基准面向企业智能体平台的编排能力评估与上线前质量门禁场景。

rss · 机器之心 · 11月10日 10:33

**「背景」** 多智能体编排关注模型能否在运行时完成任务拆解、子智能体调度、上下文分配、中间结果校验和最终整合；材料称 Claude Code、Codex 等框架已支持模型拉起子智能体或生成可执行工作流。与预先由工程师固定协作结构的方式相比，这类能力把部分编排决策交给模型动态完成，因此需要专门评测其调度与整合质量。

**「治理启示」** 企业评测多智能体系统时，可将编排过程拆分为任务分解、上下文授权、中间校验和结果汇总等环节，分别设置可观测指标与质量门禁，而不是只评价最终答案。WorkflowArena 是否提供了足以落地这类分层评测的方法，仍需等待完整技术材料。

**标签**: `#多智能体评测`, `#WorkflowArena`, `#智能体编排`, `#质量门禁`

---