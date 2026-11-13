---
layout: default
title: "Horizon Summary: 2026-11-13 (ZH)"
date: 2026-11-13
lang: zh
---

> 从 37 条内容中筛选出 7 条重要资讯。

---

**Agentic CRM 与竞品**
1. [Salesforce 预测 AI 影响假日消费](#item-crm-vendors-1) ⭐️ 6.0/10

**企业 AI 平台与运行时**
1. [Natera 构建实验室运维智能体](#item-ai-platform-1) ⭐️ 8.0/10
2. [Bedrock 按身份管控支出](#item-ai-platform-2) ⭐️ 8.0/10

**本体、语义层与知识图谱**
1. [Neo4j CDC 编排智能体](#item-ontology-1) ⭐️ 7.0/10
2. [Neo4j 推出 Relate 与黑客松](#item-ontology-2) ⭐️ 6.0/10

**行业 AI 落地**
1. [昆腾动力物流机器人进展](#item-industry-1) ⭐️ 6.0/10
2. [Amplitude 用 Wave 闭环交付](#item-industry-2) ⭐️ 6.0/10

---

## Agentic CRM 与竞品

<a id="item-crm-vendors-1"></a>
### [Salesforce 预测 AI 影响假日消费](https://www.salesforce.com/news/stories/ai-first-holiday/) ⭐️ 6.0/10

Salesforce 基于美国、英国、加拿大和澳大利亚逾 2500 名消费者的调查称，近 20%的受访者已将 AI 作为购物起点，74%信任其推荐，30%的 AI 购物用户会借此发现新品牌。该公司预计，2026 年 AI 将影响 758 亿美元的 Cyber Week 支出，较 2025 年增长 13%，并影响超过五分之一的假日订单；来自 AI 工具的电商引流同比增长 104%。目前个人智能体主要用于比价、分析商品参数与评论及发现商品，仅 19%的个人智能体用户曾让其执行结账，73%的消费者不愿向其提供支付信息。对零售企业而言，这些数据适用于商品发现、导购和站外 AI 引流场景，但支付授权、隐私保护和错误推荐仍是关键限制。

rss · Salesforce News · 11月12日 18:00

**「背景」** 这组数据来自 Salesforce 对美国、英国、加拿大和澳大利亚逾 2,500 名消费者的自有调研；其中 2026 年 Cyber Week 支出及订单影响等数字属于预测，并非已经发生的交易结果。原文区分了消费者使用的个人 AI Agent 与零售商在电商网站部署的购物 Agent：前者目前主要用于比价、评论分析和商品发现，多数受访者仍不愿授权其代为付款。

**「竞争启示」** 材料显示，消费者对“辅助决策”和“代为交易”的信任程度存在明显分层，因此零售智能体可将商品检索、比较和推荐与支付执行拆分设计，并为后者配置明确的额度、专用支付方式和授权边界。Salesforce 还称，接触品牌购物智能体的订单平均客单价高 8%、商品件数多 23%，但这些是厂商披露的相关性数据，不能据此单独认定智能体带来了增长。

**标签**: `#Salesforce`, `#零售AI`, `#消费者购物行为`, `#AI推荐`, `#市场趋势`

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [Natera 构建实验室运维智能体](https://aws.amazon.com/blogs/machine-learning/how-natera-designed-an-agentic-ai-system-for-lab-ops-with-amazon-bedrock-agentcore/) ⭐️ 8.0/10

Natera 与 AWS 基于 Amazon Bedrock AgentCore 构建了实验室运维智能体系统 SWARM，用于处理每天超过 65 张、来自三个 Jira 队列的设备支持工单。该系统采用共享技能库的双智能体架构：swarm-agent 在工程师查看工单前自动生成结构化诊断报告，swarm-hive 支持工程师实时交互、上传图片并探索其他排障路径；底层按事件、智能体、上下文及可观测与交付四层组织，并集成 Jira、Confluence、EventBridge 和 SQS。AWS 案例称，SWARM 将平均 17.4 小时的首次响应时间缩短约 130 倍，并实现 96.2%的工单自动覆盖率；这些数据是厂商披露的落地结果。该方案适用于设备停机会影响生产流程、且故障知识分散在专家经验、厂商手册和历史工单中的实验室及企业运维场景。

rss · AWS Machine Learning Blog · 11月12日 21:47

**「背景」** 10 月 29 日的 Horizon 日报曾介绍 AWS 面向多业务团队的 AgentCore 企业平台蓝图，涵盖运行时、身份、记忆、策略、评估和多账户治理，但当时未提供客户落地数据。本次 Natera 案例则将 AgentCore 用于具体的实验室运维流程，并披露了 SWARM 的双智能体、共享技能库及 Jira 工单集成实践。

**「平台启示」** SWARM 将自动预处理与人工交互拆分为两个运行时，同时复用同一技能库和上下文层，这种分层方式可以减少不同交互入口之间的诊断逻辑重复。通过事件队列接入工单，并把厂商手册、历史工单和运营数据统一纳入上下文，也为高并发处理、知识持续更新及诊断过程追踪提供了明确的架构边界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/machine-learning/building-an-agentic-ai-platform-on-amazon-bedrock-agentcore/">2026-10-29 — AgentCore 企业平台蓝图</a></li>

</ul>
</details>

**标签**: `#Amazon Bedrock AgentCore`, `#企业智能体`, `#智能体运行时`, `#知识管理`, `#运维自动化`

---

<a id="item-ai-platform-2"></a>
### [Bedrock 按身份管控支出](https://aws.amazon.com/blogs/machine-learning/tokenomics-at-scale-track-and-cap-amazon-bedrock-spend-per-iam-principal-with-cur-2-0-and-aws-budgets/) ⭐️ 8.0/10

AWS 发布了一套面向 Amazon Bedrock 的原生成本治理方案：Bedrock 自动记录每次推理请求对应的 IAM 用户或角色，共享角色则可在代入角色时通过会话标签细分到用户。企业可在 Cost Explorer 查看按身份或标签归集的费用，或将 CUR 2.0 导出至 Amazon S3 并用 Athena 进行明细分析；随后可按 Bedrock 服务及特定身份或标签创建 AWS Budget，并在越过阈值时通过预算操作附加 Deny IAM 策略。该方案适合需要按员工、团队或应用核算并限制生成式 AI 支出的企业，但所给正文不完整，无法确认预算执行时效、全部配置限制及价格。

rss · AWS Machine Learning Blog · 11月12日 19:29

**「背景」** AWS 此前介绍过 Jamf 使用 IAM Identity Center、Bedrock 模型调用日志、Athena 和 Lambda 构建的近实时支出执行闭环；该方案控制更及时，但需要自行编写、运行和维护代码。此次方案转向 AWS 原生账单与预算能力，以减少常见场景的应用开发工作。

**「平台启示」** 该方案将 AI 成本治理拆成“身份归因、费用报告、权限执行”三层，并复用 IAM 标签把访问身份与账单维度连接起来。对采用共享模型网关或共享角色的企业，只有在角色会话中持续传递用户级标签，才能避免成本只能归集到统一角色。

**标签**: `#Amazon Bedrock`, `#AI成本治理`, `#CUR 2.0`, `#AWS Budgets`, `#IAM权限`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [Neo4j CDC 编排智能体](https://neo4j.com/blog/developer/change-data-capture-to-orchestrate-agents/) ⭐️ 7.0/10

Neo4j 官方博客介绍用 Change Data Capture（CDC）把图数据库中的已提交变更转成有序事件流：例如筛选 Task 的 status 更新，在任务从 PENDING 变为 ACTIVE 时触发后续智能体。文章称该模式将任务状态、智能体交接、治理决策和审计信息关联在同一图中，并可在 Cypher 中查询失败事件；但所给正文未展示完整实现，也没有提供可验证的落地效果。CDC 适用于智能体工作状态已存于 Neo4j、需要按状态变更驱动交接并保留可查询审计轨迹的企业工作流；该能力仅适用于 AuraDB Business Critical，以及自托管 Neo4j Graph Database Enterprise 或 Infinigraph Editions。

rss · Neo4j Blog · 11月12日 09:47

**「背景」** Neo4j 的 CDC 文档说明，\`db.cdc.query\` 可根据给定的变更标识查询数据库后续发生的变更；本文将这一能力用于读取任务状态变更，以驱动智能体交接。

**「建模启示」** 该方案把业务状态写入作为事件源，并通过 CDC 读取有序变更，再由工作进程触发智能体；这可供需要减少状态库与独立事件审计系统之间同步的架构评估。文章同时指出，失败事件可以作为图节点关联任务与处理失败的智能体，让排查与运行状态处于同一查询环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neo4j.com/docs/cdc/current/procedures/">Use CDC to query changes (procedures) - Change Data Capture</a></li>

</ul>
</details>

**标签**: `#Neo4j`, `#Change Data Capture`, `#多智能体编排`, `#知识图谱`, `#审计追踪`

---

<a id="item-ontology-2"></a>
### [Neo4j 推出 Relate 与黑客松](https://neo4j.com/blog/graph-database/announcing-the-relate-by-neo4j-hackathon-2026-build-ai-agents-on-an-embedded-graph-database/) ⭐️ 6.0/10

Neo4j 宣布在 NODES 2026 推出开源嵌入式数据库 Relate，并于 11 月 11 日在 Devpost 启动为期一个月的线上黑客松，征集利用关联上下文构建的 AI 智能体、应用或工具。Relate 以库的形式运行在应用内部，无需部署服务器，支持内存、目录或单文件图存储，可通过 Rust、Python、命令行及浏览器 WebAssembly 使用，并提供本地关系遍历、向量搜索、返回行数受限的 JSON 查询结果和多智能体共享事务更新。厂商将其定位为面向智能体的上下文与记忆组件，适用于缺陷追踪、多智能体任务协同和知识库探索；比赛设三个获奖名额，奖品硬件总价值超过 6000 美元。

rss · Neo4j Blog · 11月12日 01:55

**「背景」** 嵌入式数据库与应用运行在同一进程内，可减少独立数据库服务的部署和网络调用成本。Relate 进一步用图结构表达事实之间的关系，并允许智能体通过 Cypher 查询这些关联，但原文未提供性能基准、生产部署案例或长期运维与治理细节。

**「建模启示」** 对 CRM+AI 平台而言，可按会话、沙箱或用户建立可销毁的单文件关系图，把客户、人员、事件、任务和证据建模为连接事实；受限行数的结构化结果与可纠正错误信息，也体现了为智能体工具调用控制上下文规模和失败恢复路径的设计思路。

**标签**: `#Neo4j`, `#嵌入式图数据库`, `#AI 智能体`, `#上下文引擎`, `#开源项目`

---

## 行业 AI 落地

<a id="item-industry-1"></a>
### [昆腾动力物流机器人进展](https://www.qbitai.com/2026/11/509281.html) ⭐️ 6.0/10

昆腾动力称，其机器人已在跨境物流称重、量方场景完成产品市场匹配（PMF）验证，并出现客户复购；公司计划于 12 月底发布新一代构型机器人。现有材料未披露客户名称、部署规模、产品价格或作业效果数据，相关信息适用于关注物流仓储自动化的企业评估场景需求与交付进展，但尚不足以判断规模化交付情况。

rss · 量子位 · 11月12日 01:45

**「背景」** 物流仓储中的跨境称重量方，是机器人可切入的具体作业场景；现有材料称昆腾动力已在这些场景完成产品市场匹配验证并出现客户复购，但未提供客户名称、部署规模或效果数据。

**标签**: `#具身智能`, `#物流机器人`, `#跨境物流`, `#产品市场匹配`, `#客户复购`

---

<a id="item-industry-2"></a>
### [Amplitude 用 Wave 闭环交付](https://openai.com/business/customer-stories/amplitude) ⭐️ 6.0/10

OpenAI 客户案例称，Amplitude 主要基于 OpenAI 模型构建了主动式产品智能体 Wave，用于识别产品改进机会、借助编码智能体协助团队交付变更，并衡量上线后的影响，形成从需求发现到效果评估的闭环。案例标题宣称产品改进可在 1 至 2 天内交付，但现有材料未提供时间口径、效果基线、模型配置或可复核数据；该方案适用于软件企业的产品规划、研发协作和上线效果分析场景。

rss · OpenAI News · 11月12日 20:00

**「背景」** Amplitude 将 Wave 定位为主动式产品智能体：它识别待开发的产品改进机会，协助团队通过编码智能体交付变更，并衡量上线效果。

**「行业启示」** Wave 将产品行为分析、需求识别、编码执行和效果衡量串联起来，体现了产品智能体可通过调用专业编码智能体完成跨环节协作。对企业 AI 平台而言，这种分工方式可作为设计“分析智能体负责判断、执行智能体负责变更、指标系统负责验证”架构的参考。

**标签**: `#产品智能体`, `#编码智能体`, `#产品分析`, `#研发提效`, `#OpenAI`

---