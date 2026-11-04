---
layout: default
title: "Horizon Summary: 2026-11-04 (ZH)"
date: 2026-11-04
lang: zh
---

> 从 203 条内容中筛选出 12 条重要资讯。

---

**Agentic CRM 与竞品**
1. [Slack 披露智能体调用规模](#item-crm-vendors-1) ⭐️ 8.0/10
2. [Salesforce 拟收购 Cresta](#item-crm-vendors-2) ⭐️ 7.0/10
3. [Workday 推无头 AI 智能体平台](#item-crm-vendors-3) ⭐️ 7.0/10

**企业 AI 平台与运行时**
1. [Claude 接入 MLflow 追踪](#item-ai-platform-1) ⭐️ 8.0/10
2. [AgentCore 代理用户访问配置](#item-ai-platform-2) ⭐️ 8.0/10
3. [曙光云发布 OneBox 协作平台](#item-ai-platform-3) ⭐️ 6.0/10

**本体、语义层与知识图谱**
1. [Auto Ontology 发布报道](#item-ontology-1) ⭐️ 7.0/10
2. [Neo4j Kafka 连接器 v6](#item-ontology-2) ⭐️ 7.0/10

**AI 评测、治理与安全**
1. [NIST 智能体身份授权十原则](#item-governance-1) ⭐️ 7.0/10
2. [TRAI 拟要求电信商建立 AI 治理体系](#item-governance-2) ⭐️ 7.0/10

**分析师与研究**
1. [Gartner：2030 年开放模型占九成](#item-research-1) ⭐️ 7.0/10
2. [Gartner2027 技术趋势前瞻](#item-research-2) ⭐️ 7.0/10

---

## Agentic CRM 与竞品

<a id="item-crm-vendors-1"></a>
### [Slack 披露智能体调用规模](https://www.salesforce.com/news/stories/slack-stats/) ⭐️ 8.0/10

Salesforce 披露，智能体可通过 MCP 等开放标准，利用 Slack 中涉及 GitHub、Salesforce、Jira 等平台的业务上下文并实时执行操作；据其统计，Slack 每周处理 1.27 亿次 MCP 工具调用，调用量逐季翻倍。面向销售与运营协作，文中称 Rochester Electronics 已使用 Slackbot、可复用 Skills 和自定义工作流生成高管简报、准备客户会议、分析销售表现并推送 Salesforce 通知；Vercel 则在 Slack 中运行入站销售智能体，辅助线索筛选、研究和外联文案起草。上述规模与客户使用情况均为厂商披露，所给正文未说明调用统计口径，也未直接佐证原标题中“半数消息不再来自人类”的说法。

rss · Salesforce News · 11月3日 22:30

**「背景」** Slack 最初用于让工程团队在同一处协调代码、日志告警和团队沟通；Salesforce 将其当前定位延伸为人类与智能体协同工作的执行层。文中所述的 MCP 使智能体能够从 Slack 及 GitHub、Salesforce、Jira 等平台获取上下文并执行操作，说明协作工具正在从消息传递入口扩展为跨系统工作入口。

**「竞争启示」** 材料展示了一种将协作渠道作为智能体操作入口的设计：通过 MCP 连接业务上下文与执行动作，再以 Skills 和工作流承接可重复的销售、运营任务。对 CRM+AI 产品设计的具体参考是，将客户会议准备、线索筛选及业务通知嵌入团队已有的沟通渠道；不过，材料未披露权限控制、操作审批或审计机制，尚不足以评估其执行治理能力。

**标签**: `#Slack`, `#Salesforce`, `#MCP`, `#企业智能体`, `#协同执行平台`

---

<a id="item-crm-vendors-2"></a>
### [Salesforce 拟收购 Cresta](https://news.google.com/rss/articles/CBMifkFVX3lxTFBNbzYxbkJmb04tQ1lzT3pYZUNxNkVvcHlaa2hIcVQ4anRtVzVOQXA5bnBnTGRKaDFDQXNIN2JQSVNaTVVTUENxa25LTktYUGFIamlpUnVOUE5PR3o0Y29rR0Q4UDRaQWNXM0t1ckRId2tpazVVa09PakkzMW1CQQ?oc=5) ⭐️ 7.0/10

MarTech 的报道标题称，Salesforce 正在收购 AI 客服公司 Cresta；所附其他媒体标题将 Cresta 描述为语音 AI 或客户体验平台，并称 Salesforce 已同意收购。The Next Web 等媒体标题提及交易金额约为 27 亿美元，但所供材料仅含标题，无法确认正式交易条款、交割状态或完成时间。这一动向涉及企业语音客服场景，材料尚未提供与 Salesforce 产品的整合方案、能力上线安排或客户使用情况。

rss · GN 竞品 CRM EN · 11月3日 15:22

**「背景」** 所附报道标题将 Cresta 描述为语音 AI 或 AI 客户体验平台，因此这笔拟议收购涉及的具体方向是语音客服与客户体验。各标题分别使用“拟收购”“同意收购”等表述，现有材料不足以确认交易已经完成，也未说明 Cresta 将如何整合进 Salesforce 的产品体系。

**标签**: `#Salesforce`, `#Cresta`, `#AI客服`, `#企业并购`, `#CRM竞品格局`

---

<a id="item-crm-vendors-3"></a>
### [Workday 推无头 AI 智能体平台](https://news.google.com/rss/articles/CBMiqgFBVV95cUxNRFZCd1hLZjhVTzM0aF9ZbzRGUFlBUUJCb0EwenRpVGJtSXFiYnQyc1E5ajZtYU53X0Fucy1WVWFRLXhWUkQ1Mk5INngwTDhWT1RGNVBkdzFPeXQtQWRXSzF0VnJrQ1REcWhIelFDWEFidjNGV0xoNVRQZUVmNk91RFA5WXZSelZqeDg1OUQ4bEZkQ29UcmpTRW50QXAyOHQ5Y0dPM3ROQU5lQQ?oc=5) ⭐️ 7.0/10

据 Small Business Trends 的报道标题，Workday 推出面向人力资源与财务场景的无头式 AI 智能体平台，并以提升安全性为宣传重点。所给材料仅含聚合标题，未披露平台正式名称、具体能力、安全机制、价格及可用范围，因此尚无法确认哪些能力已经上线，也无法验证其安全性改善。

rss · GN 竞品 企业套件 EN · 11月3日 15:11

**「背景」** 与所给标题相对应的报道补充称，Workday 的 Trusted Agent Platform 已采用“无头”模式，客户可构建并运行处理人力资源和财务数据的智能体，而不必让用户登录 Workday；该报道还提到平台附带规则机制。另有报道将这一发布与 Workday 的 Data Cloud、Data Connect 及 Live Data Query 能力扩展联系起来，但所给来源未提供更具体的可用范围或安全实现细节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.enterprisetimes.co.uk/2026/10/16/workday-unveils-autopilot-agents-a-headless-agent-platform-and-new-decision-tools-at-rising-2026/">Workday Unveils Autopilot Agents , a Headless Agent Platform and...</a></li>
<li><a href="https://www.dhrmap.com/column/workday/workday-launches-agentic-ai-to-transform-enterprise-execution-systems">Workday Launches Agentic AI to Transform Enterprise Execution...</a></li>

</ul>
</details>

**标签**: `#Workday`, `#AI智能体平台`, `#无头架构`, `#人力资源与财务`, `#智能体安全`

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [Claude 接入 MLflow 追踪](https://www.databricks.com/blog/claude-platform-now-supports-native-opentelemetry-observability-databricks-mlflow) ⭐️ 8.0/10

Databricks 宣布，Databricks MLflow 现已成为 Claude Platform 原生 OpenTelemetry 导出的受支持目的地，覆盖 Anthropic SDK、Messages API 和 Managed Agents。追踪数据通过 Zerobus Ingest 写入与 MLflow 实验关联的 Unity Catalog 表，开发者可查看模型请求、工具调用、耗时、错误及评估信息，用于调试智能体、定位重复故障和评估版本改动；输入输出内容只有在选择“full”内容模式时才会采集。该集成适合需要统一追踪、故障排查、质量评估和访问治理的企业智能体平台，材料未披露价格、权限配置细节、成本或实际落地数据。

rss · Databricks Blog · 11月3日 21:00

**「背景」** OpenTelemetry 是用于采集和导出服务信号的开放标准，Claude 的原生埋点会把模型请求和工具调用记录为多个 span，并通过 OpenTelemetry Protocol 导出。MLflow Tracing 基于 OpenTelemetry，相关追踪可在实验页面中查看，也可通过 SQL 查询 Unity Catalog 中的数据。

**「平台启示」** 该集成体现了“统一追踪协议、实验管理与数据治理”分层：Claude 负责生成原生执行追踪，Zerobus 承担高吞吐摄取，MLflow 负责调试与评估，Unity Catalog 负责表级数据访问控制。对 CRM+AI 平台而言，可将模型调用、工具调用和评估结果纳入同一条可治理的执行链路，同时把敏感输入输出采集设计为明确的选择项。

**标签**: `#智能体可观测性`, `#OpenTelemetry`, `#Databricks MLflow`, `#Claude Platform`, `#智能体评估`

---

<a id="item-ai-platform-2"></a>
### [AgentCore 代理用户访问配置](https://aws.amazon.com/blogs/machine-learning/servicenow-on-behalf-of-token-exchange-with-bedrock-agentcore-gateway/) ⭐️ 8.0/10

AWS 发布技术文章，演示如何在 Amazon Bedrock AgentCore Gateway 的目标配置中设置 Microsoft Entra ID 的代理用户（OBO）令牌交换，让 AI 智能体保留发起用户身份并调用 ServiceNow REST API。按文中流程，网关在每次请求时将传入令牌交换为面向 ServiceNow API 连接器的新令牌；ServiceNow 将其中的 preferred\_username 声明映射到已有用户，并按该用户权限处理调用。该方案适用于需要用户级授权与审计的企业智能体 API 集成；文章提供的是配置示例，未提供规模化部署数据或定价信息。

rss · AWS Machine Learning Blog · 11月3日 16:47

**「背景」** 代理用户调用企业 API 时，需要同时保留用户身份，并让令牌的受众与下游 API 匹配；本文中，智能体传入令牌的受众是智能体应用，而 ServiceNow 要求受众为其 API 连接器。OBO 流程通过 Entra ID 验证委托授权并签发新令牌，方案需要两个 Entra 应用注册，以及 ServiceNow 侧关联 Entra ID 的入站 OAuth 集成。

**「平台启示」** 该示例将令牌交换放在网关目标配置中，由网关处理下游令牌获取，ServiceNow 继续依据映射用户执行权限检查。对 CRM+AI 平台设计的参考点是：工具调用网关可以集中处理身份委托，但接入时仍需明确每个下游系统的令牌受众、用户映射与权限规则。

**标签**: `#Bedrock AgentCore`, `#AgentCore Gateway`, `#身份传播`, `#OAuth/OBO`, `#企业 API 权限`

---

<a id="item-ai-platform-3"></a>
### [曙光云发布 OneBox 协作平台](https://news.google.com/rss/articles/CBMiXkFVX3lxTE9ELXZoNGJlZks3R1NHcW5Pd0h0LWVnbVh1czlNeENCeDM4N3ItMVBMN2pOQmROT0ZIdlBnV3UwQ2ppb2xrTWY0YksySkRtMGdzSDJic0Q4M1dzdGxmcVE?oc=5) ⭐️ 6.0/10

据 36 氪经 Google News 聚合的条目标题，曙光云发布了 OneBox 智能体协作平台。现有材料仅包含标题与来源，未披露智能体协作机制、编排与运行时能力、权限治理、部署方式、价格及可用范围，也未提供客户案例，暂无法判断其适用的具体企业场景或是否已开放使用。

rss · 36氪（经 Google News） · 11月3日 07:57

**「背景」** 现有材料仅包含 36 氪的聚合标题，未提供曙光云此前的智能体产品布局或 OneBox 的技术说明，尚无法确认该平台与其既有产品的关系。标题中的“智能体协作”也未明确是指多个智能体之间的任务协同，还是人与智能体之间的协作。

**标签**: `#曙光云`, `#OneBox`, `#智能体平台`, `#智能体协作`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [Auto Ontology 发布报道](https://news.google.com/rss/articles/CBMiiwFBVV95cUxOV3Q5anhDc2NrVHlOR0diZjN0U0RRNGM5WFJMRzZrRTdsQ0U5WjBtdlZ2bXJYOEd1akpDZkozeUFONXotYWlFSWJteFdBS2FIeFlYdi14SjBsV3FTcjNjN2JRRGo2cDMyckpyblZROUhMRzM1dVJmOE1lN0hJTXl1RFl3R1IyMjZ1VEpF?oc=5) ⭐️ 7.0/10

据 news.lavx.hu 的 RSS 标题报道，NVIDIA 发布了面向智能体上下文层的 Auto Ontology。该消息涉及企业智能体的上下文组织与本体建模方向，但现有材料仅包含标题和链接，未披露具体能力、版本、价格、可用范围或客户案例。目前无法据此确认其是否已正式可用，也无法判断其对 CRM 等企业场景的具体支持。

rss · GN 本体与语义层 EN · 11月3日 08:07

**「背景」** 这里的语义层用于把企业元数据组织成智能体可使用的上下文，并让智能体依据经过认证的业务定义编写 SQL，从而为自然语言查询提供统一的业务口径。NVIDIA 另有公开的 auto-ontology-eval 仓库，用于对 Text-to-SQL 智能体进行数据集基准测试并评分，可为理解这一方向的查询评估方式提供参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/11/01/nvidia-auto-ontology-open-source-semantic-layer-ai-agents/">NVIDIA Releases Auto Ontology : An Open Semantic Layer That...</a></li>
<li><a href="https://github.com/NVIDIA/auto-ontology-eval">GitHub - NVIDIA / auto - ontology -eval: LLM-powered Text-to-SQL...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Auto Ontology`, `#智能体上下文层`, `#本体建模`, `#语义层`

---

<a id="item-ontology-2"></a>
### [Neo4j Kafka 连接器 v6](https://neo4j.com/blog/developer/neo4j-connector-for-apache-kafka-and-confluent-v6/) ⭐️ 7.0/10

Neo4j 发布面向 Apache Kafka 和 Confluent 的 Connector v6，新增统一的节点与关系 CDC 事件模式、OIDC 认证，以及由连接器自动处理的 Exactly-once 约束；厂商称其在配置、可靠性和安全性方面有所简化或提升。CDC 可用于 Neo4j Aura Virtual Dedicated Cloud、Business Critical 和 Neo4j Enterprise，托管式 Neo4j Sink Connector 支持 Confluent Cloud 在 AWS、Azure 和 Google Cloud 上的私有端点。v6 还可用于基于 CDC 的自托管数据库迁移至 Aura，以及权限同步、治理告警和实体解析等事件驱动知识图谱场景；升级前需确认 Java 17、Kafka Connect 4.3、Confluent Platform 8.3 或更高版本，并更新旧版事件解析和配置项。

rss · Neo4j Blog · 11月3日 01:39

**「背景」** Kafka 与 Confluent 是 Neo4j 用于实时变更流和数据迁移的集成路径；v6 相比 5.x 的关键变化包括平台最低版本提高，以及节点和关系 CDC 事件从两种消息形状合并为一种统一模式。对于仍使用 neo4j.query.force-maps-as-struct 的部署，需要改用 neo4j.query.map-encoding。

**「建模启示」** 统一 CDC 事件模式可减少下游流处理、回写其他图数据库或落库数仓时的分支解析逻辑；同时，OIDC 与自动维护 Exactly-once 约束显示，实时知识图谱集成不仅需要事件建模，也需要将身份认证和交付语义纳入连接器治理。上述能力与收益为 Neo4j 官方材料所述，具体迁移效果仍取决于现有消费者和平台版本。

**标签**: `#Neo4j`, `#Kafka与Confluent`, `#变更数据捕获（CDC）`, `#事件驱动知识图谱`, `#实时数据集成`

---

## AI 评测、治理与安全

<a id="item-governance-1"></a>
### [NIST 智能体身份授权十原则](https://news.google.com/rss/articles/CBMipAFBVV95cUxOajBtOEdwR3ZtWjgwc3hYRHZiUFIza1R3TFVIUnVhZlZ0YUoxOENuMThxemlJZG9rWEdZSkx5OEJaNkdrVjN0U0FpZlNoOTNYOXByLVJ1Y21DZ3I2a0dlU3liSUlGOFNzal9WeGoxcnR0OVpZUzAtZG1TSGEyMTBBbGdMMF96ZDBDSFdKTXQzeXpwQTdId2xfYWlsd2p3VkQwb3ZsWg?oc=5) ⭐️ 7.0/10

据 Biometric Update 报道标题，美国国家标准与技术研究院（NIST）提出了面向 AI 智能体身份与授权的十项原则，涉及企业部署智能体时的身份识别与权限治理议题。现有材料仅包含标题及来源，未提供原则正文，无法确认其正式发布状态、文件性质、具体要求及适用范围；企业可将其作为后续核查的治理线索，目前尚不足以据此制定 CRM+AI 智能体的权限控制方案。

rss · GN 智能体治理与评测 EN · 11月3日 16:52

**「背景」** Biometric Update 是关注生物识别行业的媒体，其网站列出了这则关于 NIST 智能体身份与授权十项原则的报道。目前提供的材料仅有标题与网站摘要，缺少 NIST 原始文件和原则正文，因此尚无法确认其属于正式标准、草案还是研究建议，也无法核实具体要求与适用范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.biometricupdate.com/">Biometric Update | Biometrics News, Market Research &amp; Companies</a></li>

</ul>
</details>

**标签**: `#NIST`, `#智能体身份`, `#授权与权限治理`, `#AI 安全`, `#治理框架`

---

<a id="item-governance-2"></a>
### [TRAI 拟要求电信商建立 AI 治理体系](https://news.google.com/rss/articles/CBMiWEFVX3lxTE5mZ1JQc2RBWENKdHhxMHhFLXI4QTlJNEt3X2NUSUZ6NXo1VHdJTWtVdW44Qmh0TkpsLXR3ZUxSdzJ6VHdxZ0E0SGhpbUlTU2pCRzBDdmIyMGI?oc=5) ⭐️ 7.0/10

据维度网报道标题，印度电信监管机构 TRAI 拟要求电信运营商建立 AI 治理体系，该消息涉及拟议要求，尚不能视为已生效规则。现有材料仅包含标题，未披露治理体系的具体要求、适用范围或实施时间，电信企业及面向该行业的 CRM+AI 产品团队仍需依据后续规则判断具体合规义务。

rss · GN AI 治理与安全 中文 · 11月3日 08:49

**「背景」** TRAI 是印度电信领域的监管机构，负责推动和监管电信服务发展。此次信息仅表明其拟要求电信运营商建立 AI 治理体系，具体适用范围、治理要求和实施时间尚未披露，因此目前应视为监管方向而非已生效规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telecom_Regulatory_Authority_of_India">Telecom Regulatory Authority of India - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI治理`, `#电信监管`, `#合规监管`, `#问责与审计`, `#企业AI平台`

---

## 分析师与研究

<a id="item-research-1"></a>
### [Gartner：2030 年开放模型占九成](https://news.google.com/rss/articles/CBMikAFBVV95cUxNaTZsTFpDOWNrMWdSYTFHVURrWEtUOHgxclFfRUVpT0FEeG8tcml0Sk44NE1XbzdkUHpTWk9xbTBOMzFiS0dnbklPa2xqUEhSaGVNUHZVYzA5dW9IdWRPQWc4eXU5eXFxOXcwVFVNYkN6WlQ1TEk0TjBlanpOblJ3QzZ1bXJzRVV6OU55TDIyNWg?oc=5) ⭐️ 7.0/10

Dataconomy 报道称，Gartner 预测到 2030 年，开放模型将运行 90%的企业 AI 智能体工作流。该信息仅给出了预测结论，未披露原始报告、预测口径、数据依据或具体模型范围，因此不能据此判断当前企业采用率或实际性能。对 CRM 与企业 AI 平台而言，这一预测主要涉及智能体工作流的长期模型选型、部署方式和开放生态兼容性。

rss · GN 分析师 EN · 11月3日 08:48

**「背景」** 企业 AI 智能体系统将模型的推理能力与实际操作结合，使其能够执行任务；相关评测覆盖工具调用、浏览器研究和多步骤计算机操作。理解本条预测时需留意统计口径：所给报道标题分别使用“工作流”和“智能体步骤”，当前材料不足以确认二者是否指同一统计单位。

**「研究启示」** 在缺少更多依据的情况下，可将该预测作为长期架构规划的观察信号，而不是现状判断：企业平台可关注模型可替换性、开放权重模型的部署接口与治理机制，以降低未来模型切换的集成成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://benchlm.ai/agentic">Best LLMs for Agentic — October 2026 Leaderboard | BenchLM. ai</a></li>
<li><a href="https://www.moveworks.com/us/en/resources/blog/the-rise-of-agentic-systems-how-they-work">Agentic Systems: The Rise of Agentic AI -powered Automation</a></li>

</ul>
</details>

**标签**: `#Gartner`, `#开放模型`, `#企业AI智能体`, `#Agentic AI`, `#平台架构预测`

---

<a id="item-research-2"></a>
### [Gartner2027 技术趋势前瞻](https://news.google.com/rss/articles/CBMiTEFVX3lxTFAteEJWS2lQaXh2MTJHRlBoOUVpRjE2SWFYYlVlN2VrWTl3cVZPRkFxcmpNbU8tZGh6amlMd2N0T0tBUEdmLUIxRTRfS3o?oc=5) ⭐️ 7.0/10

据凤凰网科技报道标题，Gartner 发布了 2027 年十大技术趋势，其中“非文本 AI”被列为第一，“Harness”被视为未来 1 至 3 年的重点方向。所给材料仅包含标题和来源，未提供完整趋势清单、两项概念的定义、排序依据或 Gartner 原始报告，因此尚无法判断其具体能力边界与成熟度。对企业 AI 平台及 CRM+AI 产品规划而言，这条资讯可作为后续研究线索，但不足以据此确定应用场景或技术选型。

rss · GN 分析师 中文 · 11月3日 11:27

**「背景」** Gartner 此前已发布过上一版《Top Strategic Technology Trends for 2026》，相关页面将其定位为面向企业技术战略的趋势与框架内容；本条报道则聚焦 2027 年趋势，并特别提到非文本 AI 与 Harness。由于现有材料未提供 2027 年趋势的完整定义、研究方法或数据，暂不能进一步核实这两个术语的具体范围及排名依据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gartner.com/en/articles/top-technology-trends-2026">Top Strategic Technology Trends for 2026 | Gartner</a></li>

</ul>
</details>

**标签**: `#Gartner`, `#技术趋势`, `#非文本AI`, `#Harness`, `#企业AI平台`

---