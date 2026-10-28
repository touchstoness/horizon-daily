---
layout: default
title: "Horizon Summary: 2026-10-28 (ZH)"
date: 2026-10-28
lang: zh
---

> 从 231 条内容中筛选出 12 条重要资讯。

---

**Agentic CRM 与竞品**
1. [Agent Fabric 新增评测与成本控制](#item-crm-vendors-1) ⭐️ 8.0/10
2. [钉钉 DWS 适配鸿蒙 PC 并开源](#item-crm-vendors-2) ⭐️ 8.0/10
3. [Oracle 发布 AI 规划与语义层](#item-crm-vendors-3) ⭐️ 7.0/10
4. [Zoho 连接工作应用支撑智能体 AI](#item-crm-vendors-4) ⭐️ 6.0/10
5. [OpenAI 与 Oracle 扩展合作](#item-crm-vendors-5) ⭐️ 6.0/10

**企业 AI 平台与运行时**
1. [ai\_extract 文档抽取评测流程](#item-ai-platform-1) ⭐️ 8.0/10
2. [Google Cloud 推出 IAM Helper](#item-ai-platform-2) ⭐️ 8.0/10
3. [腾讯上线 WorkBuddy 开放平台](#item-ai-platform-3) ⭐️ 6.0/10
4. [科大讯飞首发星辰 TaaS](#item-ai-platform-4) ⭐️ 6.0/10

**本体、语义层与知识图谱**
1. [Oracle 扩展 AI Lakehouse](#item-ontology-1) ⭐️ 7.0/10

**AI 评测、治理与安全**
1. [IBM Agent Identity 正式可用](#item-governance-1) ⭐️ 7.0/10
2. [欧盟 AI 法案首项协调标准发布](#item-governance-2) ⭐️ 7.0/10

---

## Agentic CRM 与竞品

<a id="item-crm-vendors-1"></a>
### [Agent Fabric 新增评测与成本控制](https://www.salesforce.com/news/stories/agent-fabric-catch-failures-control-ai-costs/) ⭐️ 8.0/10

Salesforce 宣布为跨平台智能体控制平面 Agent Fabric 增加 Agent Evals、API Evals 和高级成本控制：前者可在部署前生成测试，并在生产环境按质量阈值持续评测智能体、LLM 和 MCP 服务器；API Evals 则从 API 规范生成测试，以发现功能或性能变化。质量不达标时，平台可按预设策略告警、触发审批或通过 Agent Kill Switch 下线智能体；FinOps Dashboard 与 Model Wallet 提供统一支出视图和预算硬上限，在超出预算前停止请求。Salesforce 称 Agent Fabric 日均处理超过 12 亿次请求，成本优化策略在测试场景中可通过语义缓存、载荷压缩和响应裁剪将 Token 用量最多降低 75%，但未公布定价、正式可用范围或外部客户验证；ASICS Digital 表示正在参与 Agent Evals Beta。该组合适用于同时运行多平台智能体、需要持续控制客服质量、API 依赖风险和 AI 预算的企业。

rss · Salesforce News · 10月27日 13:00

**「背景」** Agent Fabric 是 Salesforce 用于跨平台管理和治理 AI 智能体的控制平面。此次扩展针对智能体上线后的持续运营问题：底层模型、API 和成本结构变化可能导致质量下降或支出增加，而问题发现、责任人通知与限制智能体运行此前往往分属不同流程。

**「竞争启示」** Agent Fabric 将“评测发现问题”与“自动干预和预算阻断”置于同一控制平面，并允许企业按政策加入审批，体现了企业智能体治理从监控看板向可执行闭环演进的产品设计。对 CRM+AI 平台而言，可参考按质量阈值、API 变更和预算上限分别设置检测信号与处置动作，但实际效果仍取决于评测机制和策略配置等尚未披露的细节。

**标签**: `#Salesforce`, `#Agent Fabric`, `#智能体治理`, `#自动化评测`, `#成本控制`

---

<a id="item-crm-vendors-2"></a>
### [钉钉 DWS 适配鸿蒙 PC 并开源](https://www.jiqizhixin.com/articles/2026-10-27-7) ⭐️ 8.0/10

钉钉开放平台近日宣布，DingTalk Workspace CLI（DWS）已完成鸿蒙 PC 适配并正式开源，将钉钉办公能力封装为标准化命令行接口。按钉钉披露，DWS 涵盖 25 项业务模块和 1000 多条命令，覆盖群聊、会议听记、待办、AI 表格、文档、日历、通讯录及审批等场景，可用于企业智能体接入和调用办公系统能力。现有材料未提供开源仓库、权限治理机制、实际客户案例或可复核的应用效果。

rss · 机器之心 · 10月27日 03:26

**「背景」** CLI 可将办公系统能力转化为可脚本化调用的命令，使外部 Agent 能把群聊、审批、日历等功能作为工具接入，而不必仅依赖图形界面操作。此次 DWS 所称的“开放办公能力”，即将钉钉既有业务模块统一封装为这类接口；现有材料尚未披露权限治理、具体技术实现及实际客户案例。

**「竞争启示」** DWS 采用标准化 CLI 作为智能体与办公应用之间的工具接口，体现了一种将群聊、审批等业务模块统一封装为可调用命令的集成方式。对 CRM+AI 平台而言，这种工具层设计可作为开放业务动作的参考，但企业落地仍需进一步评估身份认证、权限继承、审计和高风险操作确认机制。

**标签**: `#钉钉`, `#DingTalk Workspace CLI`, `#企业智能体`, `#鸿蒙PC`, `#办公能力开放`

---

<a id="item-crm-vendors-3"></a>
### [Oracle 发布 AI 规划与语义层](https://news.google.com/rss/articles/CBMi2gFBVV95cUxNUERrSVJ0ZXVCWF9NTnpuaHdVNi1nV1hCcUhBdzR1dE51SDh2YjJuN3NCMmlzbWxWTnpFMmIxeWgtRTQzdlAzWUdnalpEN2ZFUExTZUhJOTlwLTF6TUliaFNFT1p5d1BOc3Z4cVFJQ09yaWJoTDdfU1ZOWm9vaG1heXJzalpnSFZER211LTZ2b1dQMTg1YktlVDc0RGx5Sy0tc2lHeV8zRVc1TTRBM3ZQU2F5c0F1cGFQa2lqVDRVMGxLQjI2bnhWbjFBeDlmdm42c1owUEI1d1gtUQ?oc=5) ⭐️ 7.0/10

据 Tech Times 标题信息，Oracle 宣布了 AI 规划引擎和语义层，目标是减少 AI 智能体对企业业务数据的误读。现有材料未披露具体产品归属、技术实现、版本、价格、客户案例或可用范围，也无法确认相关能力是否已经正式上线。该方向主要面向需要智能体理解统一业务口径并据此制定任务计划的企业数据分析、CRM 及业务自动化场景；降低误读属于厂商提出的目标，实际效果仍待验证。

rss · GN 竞品 数据与平台 EN · 10月27日 05:50

**「背景」** 从概念上看，语义层用于以统一的业务口径组织底层数据，规划引擎则负责将智能体目标拆解为执行步骤；二者结合，针对的是企业智能体因指标定义或数据关系理解不一致而产生错误的问题。当前材料只有报道标题，尚未说明 Oracle 此前对应能力、具体产品归属及技术实现。

**标签**: `#Oracle`, `#AI智能体`, `#语义层`, `#规划引擎`, `#企业数据`

---

<a id="item-crm-vendors-4"></a>
### [Zoho 连接工作应用支撑智能体 AI](https://news.google.com/rss/articles/CBMilwFBVV95cUxNeWdRREs2N0gwZHAzM2g0N2FJQXRSNWJ2dnhJZWpIMTIwNUNSbFBoekRTd2lFSFM3LVBza3QxdFhTQmRrZ0ZTOW1yRUR3QXl4UjkzRkdJeldaeXJVTUhDQ1hZMW1URUZNV0Y3eUNRWVJiS19ZanZrQlZEYkFFZnNYbTRUYkVyUHZzNFNZTWp1M3VTU3hkRElN?oc=5) ⭐️ 6.0/10

《首尔经济日报》的标题信息显示，Zoho 正尝试连接分散的企业工作应用，为其智能体 AI 能力提供跨应用基础。这一方向适用于需要智能体跨 CRM 及其他业务系统获取信息、衔接流程的企业场景，但现有材料未披露具体产品名称、技术架构、上线状态、定价、可用范围或客户案例。

rss · GN 竞品 CRM 二 EN · 10月27日 00:41

**「背景」** 跨应用连接可为企业智能体提供统一的业务上下文，并支持其在多个工作系统之间调用数据与执行流程。当前材料仅有聚合标题，尚无法确认 Zoho 采用的具体产品、集成架构、发布状态及开放范围。

**「竞争启示」** 该信息体现的产品思路是先打通分散应用，再承载智能体的跨系统任务执行；对 CRM+AI 平台而言，应用连接和业务上下文整合可能是智能体能力落地的基础层。

**标签**: `#Zoho`, `#Agentic AI`, `#应用集成`, `#企业AI平台`

---

<a id="item-crm-vendors-5"></a>
### [OpenAI 与 Oracle 扩展合作](https://openai.com/index/oracle-apps-in-chatgpt) ⭐️ 6.0/10

OpenAI 宣布扩大与 Oracle 的合作，计划把 Oracle 业务应用和 AI 智能体引入 ChatGPT，并以 OpenAI 技术支持 Oracle 的新产品。现有材料未披露具体应用清单、集成架构、能力边界、上线时间、价格或客户案例，因此这些内容仍属于合作计划，而非已确认上线的功能。该合作面向需要通过 ChatGPT 访问企业业务应用、调用智能体处理运营任务的企业场景。

rss · OpenAI News · 10月27日 07:00

**「背景」** OpenAI 将此次合作扩展概括为三个方向：在 ChatGPT 中使用 Oracle 应用、为 Oracle 产品引入 AI，以及通过 Oracle Marketplace 获取 OpenAI 服务。现有材料未披露具体应用清单、集成架构或上线时间，因此尚无法判断这些方向中哪些已正式可用。

**「竞争启示」** 这一合作体现了将通用对话入口与既有企业应用、业务智能体连接的产品路径；对 CRM+AI 平台而言，应用接入范围、身份与权限治理以及智能体调用边界将是后续需要观察的关键设计点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/oracle-apps-in-chatgpt/">OpenAI expands partnership with Oracle to bring its apps to ChatGPT</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Oracle`, `#ChatGPT`, `#企业应用集成`, `#AI智能体`

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [ai\_extract 文档抽取评测流程](https://www.databricks.com/blog/spot-fixes-measured-gains-improving-document-extraction-accuracy-aiextract-and-mlflow-prompt) ⭐️ 8.0/10

Databricks 介绍了一套企业文档抽取优化流程：使用 ai\_extract 生成结构化字段，以 MLflow Prompt Registry 对提示词和 JSON Schema 进行版本管理，并将人工审核结果整理为真值集，用于评估改动和发现回归。其项目需要从数十种 PDF 布局中抽取约 40 个字段；一次 Schema 调整虽使 revision 字段的错误数大致减半，却让全部字段的总错误数增加 9%，说明单字段修补不能替代全局评测。该流程适用于订单等版式多样、需要人工复核并向下游系统发布结构化数据的场景；Databricks 还称 Genie Code 可构建包含解析、分类、抽取、引用与置信度的 Lakeflow 作业，并自动执行评测和迭代优化，但正文未提供可复核的整体准确率增益。

rss · Databricks Blog · 10月27日 18:00

**「背景」** ai\_extract 以解析后的文档、JSON Schema 和可选的全局指令为输入，将文档转换为结构化字段；Schema 可通过枚举、数值类型等约束限定输出。该案例原有流程已覆盖 Lakeflow 数据处理、人工审核和审批结果回流，但审核数据尚未整理为可复用评测集，提示词与 Schema 也直接嵌入管道代码，修改时需要重新部署。

**「平台启示」** 可将文档抽取拆分为数据管道、提示词与 Schema 配置、人工真值集及晋级评测四层：配置通过 Registry 独立版本化，审核结果经 CDC 回流形成可复用评测集，再以全字段、跨版式指标作为上线门槛。这种设计能减少修改配置必须重新部署代码的问题，也能识别局部改善引发的系统级回归。

**标签**: `#Databricks`, `#MLflow Prompt Registry`, `#文档抽取`, `#LLM评测`, `#提示词版本管理`

---

<a id="item-ai-platform-2"></a>
### [Google Cloud 推出 IAM Helper](https://cloud.google.com/blog/products/identity-security/scale-agents-securely-with-iam-helper-agent-skills-and-mcp-tools/) ⭐️ 8.0/10

Google Cloud 宣布推出 IAM Helper，将 IAM 工作流封装为采用开放 Agent Skills 标准的技能和 MCP Tools，供代码助手、部署流水线及自定义智能体调用，并衔接 Policy Intelligence 和 Privileged Access Manager 等现有能力。其技能覆盖权限故障诊断、临时特权访问申请、策略模拟与策略生成等流程，适配 Gemini CLI、Gemini Cloud Assist、ADK、Claude Code 和 Cursor；只读诊断与策略变更相互分离，策略变更会依据可定制风险等级暂停并等待人工确认。该产品面向云资源配置、Terraform 编写、微服务部署和 CI/CD 权限故障处理等企业场景；Google Cloud 称其有助于维持最小权限并降低管理开销，但文中场景属于示例，未提供客户验证数据，也未说明价格和具体可用范围。

rss · Google Cloud AI Blog · 10月27日 16:00

**「背景」** IAM Helper 被定位为 Google Cloud IAM 之上的智能体原生编排与接口层，而非替代底层权限引擎；它衔接 Policy Intelligence、Privileged Access Manager 等能力，并将多步骤 IAM 流程封装为智能体可调用的 Agent Skills 和 MCP Tools。其 Skills 采用开放的 Agent Skills 标准，可供 Gemini CLI、Gemini Cloud Assist、ADK、Claude Code 和 Cursor 等常见智能体环境使用。

**「平台启示」** IAM Helper 采用“智能体接口与编排层—既有 IAM 决策引擎”的分层方式，让模型负责发起工作流，而将策略评估、模拟和执行交给云端后端。对企业智能体平台而言，将只读发现、风险分级和需人工确认的写操作明确拆分，可作为工具调用权限治理的一种具体设计参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/products/identity-security/scale-agents-securely-with-iam-helper-agent-skills-and-mcp-tools">Scale agents securely with IAM Helper Agent Skills and MCP Tools</a></li>

</ul>
</details>

**标签**: `#Google Cloud`, `#智能体权限治理`, `#IAM`, `#MCP Tools`, `#Agent Skills`

---

<a id="item-ai-platform-3"></a>
### [腾讯上线 WorkBuddy 开放平台](https://news.google.com/rss/articles/CBMiTkFVX3lxTFAyTEpIWk0wMks4WmFWLXk5a2pocmJRdTN0dEVGOWs2SDh0ME5LcHlTQklJbVdzdjQxTk9zRGExY0kwbEpfdWIwZkN0UlRNZw?oc=5) ⭐️ 6.0/10

据 36 氪标题信息，腾讯已上线 WorkBuddy 开放平台，旨在把 Agent 能力延伸至更多工作场景。现有材料未披露平台的智能体构建与编排、工具调用、权限治理、运行时、定价、开放范围及客户案例，因此其具体适用的企业流程和实际落地效果尚无法确认。

rss · 36氪（经 Google News） · 10月27日 19:14

**「背景」** 配套报道显示，WorkBuddy 于 2026 年 3 月发布，此次开放平台上线是腾讯首次较完整披露其开放生态战略；平台面向智能硬件、行业应用和开发者开放底层 Agent 能力，首批引入超过 100 家生态伙伴。现有材料未说明具体接口、权限治理、运行时机制或商业条款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://readhub.cn/topic/8w77Spj77zf">腾 讯 WorkBuddy 开 放 平 台 上 线 Agent 向更多 工 作 场 景 延伸</a></li>
<li><a href="https://m.mp.oeeee.com/a/BAAFRD0000202609031658795.html">腾 讯 WorkBuddy 接入超30个硬件品牌，打响生态大战 | 南都N视频</a></li>

</ul>
</details>

**标签**: `#腾讯`, `#WorkBuddy`, `#Agent平台`, `#开放平台`, `#企业工作场景`

---

<a id="item-ai-platform-4"></a>
### [科大讯飞首发星辰 TaaS](https://news.google.com/rss/articles/CBMiZEFVX3lxTFBnZ1RvMENlaHU3S2dGWnBZS1QwZmR0Rkc2emlJQU54X1RuTzkzMUpFNjFPM1Eza2VkNUluNWFvNW82dE1objJ0ekNLS0xESXhQY3RZNE5McnhJY04tb0g0NENkTDg?oc=5) ⭐️ 6.0/10

InfoQ 写作社区条目称，科大讯飞首发星辰 TaaS 平台，定位是统一整合大模型、智能体与企业业务流程。该平台面向需要把模型能力和智能体接入业务流程的企业场景，但现有材料未说明具体架构、版本、定价、开放范围、治理与可观测能力，也未提供客户案例或效果数据。

rss · InfoQ 中文（经 Google News） · 10月27日 21:25

**「背景」** Horizon 10 月 24 日日报已记录星辰 TaaS 的首次发布：科大讯飞将其定位为面向多行业的 Token 服务平台，但当时尚未披露架构、定价、开放范围、治理机制或客户落地。本次 InfoQ 写作社区文章进一步强调大模型、智能体与企业业务流程的整合，但现有材料没有提供可核验的新版本或新增能力细节。

**「平台启示」** 星辰 TaaS 的公开定位将模型、智能体和流程编排纳入同一平台范围，可作为企业 AI 平台设计统一编排层的参考方向；不过，材料不足以判断其是否具备权限控制、工具调用、运行时治理等落地能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jiqizhixin.com/articles/2026-10-23-10">2026-10-24 — 科大讯飞发布星辰 TaaS</a></li>

</ul>
</details>

**标签**: `#科大讯飞`, `#星辰TaaS`, `#智能体平台`, `#业务流程编排`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [Oracle 扩展 AI Lakehouse](https://news.google.com/rss/articles/CBMigAJBVV95cUxQUGlpZWdZS05iam1pdENVVVZuMl9DWXQzWmhzOUFWZlN3dDlVNGZObTR5WHBEVVk3YVd0OTVSNXlmRjdJUGVRTHlXSy1PcUtrZ1ZZc0lxZFhZVnM0S3hZS0xta1RiX181WHBWWmhfRUIyUTc4V3dlbGU0VmE4N3dMY0NtaG9pdFFnb0haMzlEUHV6ZUpIcXVlbjhqcG1kY3BHZ1FzcVgyUGZHUGVzWGVwdzU1S2g3ZUtWdUFrMmo4ZDVwLWpidUUwZXFIc1otdnp6ZDRabS14ZGpRM1lpVERLSW9SZjRMZ0lhXzZWRjVKaF9RRW81QjdRQzBZQzhJNWFy?oc=5) ⭐️ 7.0/10

Oracle 于 2026 年 10 月 27 日发布的条目称，其 Autonomous AI Lakehouse 新增业务语义层，并扩大了对 Apache Iceberg 数据的支持。该组合面向需要在湖仓数据之上统一业务口径，并为企业分析或 AI 应用提供语义解释的场景。现有材料未披露具体架构、版本、定价、开放范围、客户案例或验证数据，也无法确认相关能力已全面上线还是处于预告阶段。

rss · GN 本体与语义层 EN · 10月27日 06:46

**「背景」** 在企业数据平台中，业务语义层用于将底层数据字段映射为统一的业务术语和指标，Iceberg 支持则关系到湖仓表数据的访问与管理。当前材料仅有聚合标题，未提供 Oracle 此前方案、具体架构或能力上线范围，因而无法判断此次更新与既有产品的差异。

**「建模启示」** 将业务语义层与 Iceberg 数据支持并列，体现了把底层开放表格式与上层业务概念建模分层处理的产品思路；但其语义模型如何定义、治理及供 AI 调用，仍需更多资料确认。

**标签**: `#Oracle`, `#业务语义层`, `#AI Lakehouse`, `#Apache Iceberg`, `#企业数据平台`

---

## AI 评测、治理与安全

<a id="item-governance-1"></a>
### [IBM Agent Identity 正式可用](https://news.google.com/rss/articles/CBMiugFBVV95cUxPZHdVUnNTX0ZRbXlBUTE1V2ZlbWUwTHY5XzljOTlyX0pPaEh6YkZ4WUNTVHYxRzdmS3M5dUhBemdSc2YtbVpyVkMxdjFDaDc1NTlhdDdieGV4ZDl2aTd0ZFcxUV9hS1I0cnd1VDlaR21oWVFfN2JqSU1MZHE1WW5Nc1REQy1uSElvZVVFN19GTkJMNWRNY1VWY0pFdW5fY1JCZXBHLVlqd0drYkRrSmtCeUxkeWQxa19jaUE?oc=5) ⭐️ 7.0/10

IBM 宣布 Agent Identity 已正式可用，定位是为企业 AI 智能体提供身份与信任治理能力。IBM 将其描述为构建智能体信任的基础，但现有材料未披露具体身份模型、权限控制与审计机制，也没有提供价格、集成范围、客户案例或效果数据。该产品可关注于 CRM 智能体访问客户数据、调用企业系统及执行操作时的身份和权限治理场景。

rss · GN 智能体治理与评测 EN · 10月27日 01:14

**「背景」** 智能体身份治理的核心是把企业 AI 智能体作为可识别、可授权和可审计的主体，以约束其凭证与资源访问。IBM 已为 Agent Identity 建立独立产品文档入口，但当前检索摘要未披露其身份模型、权限粒度、审计机制或具体集成范围。

**「治理启示」** 企业 AI 平台可将智能体身份作为独立治理对象，与人类用户和应用身份区分管理；不过，IBM 此次产品是否支持细粒度授权、凭证轮换和运行时控制，仍需等待更多可核验资料。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/docs/vi/agent-identity">IBM Agent Identity - IBM Documentation</a></li>

</ul>
</details>

**标签**: `#智能体身份`, `#权限治理`, `#企业AI治理`, `#IBM`

---

<a id="item-governance-2"></a>
### [欧盟 AI 法案首项协调标准发布](https://news.google.com/rss/articles/CBMirAFBVV95cUxNTXlnTmhiNkotcVM5VEQyQmZzN2tBc1VFNDdldmlXLXJvdy1xMHFoQWRUZ0JFUDRlTGUxdGVNcHFrNWdrUjVJbkRMNDh5QVZ2QUhfbk45clVOMUVpM01FR2huRjM5OWRyNkcySGY2M0gxeWUxM0NkclNnTUk4N0wyWlBQSkFLXzk2bm1EY05Cci12d0ptelBRelZUSEhmVTdlVW9YcjhRaVgzNVQ0?oc=5) ⭐️ 7.0/10

Orrick 发布的文章称，欧盟《人工智能法案》框架下首项协调技术标准已经发布。现有材料未提供标准名称、适用对象、具体合规要求、法律效力或实施时间，因此尚无法判断企业采用该标准能否获得合规推定等实际效果。该进展可能涉及企业 AI 系统的合规评估、治理流程和产品规划，但具体适用场景仍需以标准正文及欧盟后续文件为准。

rss · GN AI 评测与提示注入 EN · 10月27日 20:03

**「背景」** 该条目仅提供 Orrick 的文章标题，称欧盟《人工智能法案》框架下首个协调技术标准已经发布，但未说明标准名称、适用对象、合规要求、法律效力或实施日期，因此暂时无法判断其对企业 AI 系统合规评估和治理流程的具体影响。

**标签**: `#EU AI Act`, `#协调标准`, `#AI合规`, `#技术标准`, `#AI治理`

---