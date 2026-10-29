---
layout: default
title: "Horizon Summary: 2026-10-29 (ZH)"
date: 2026-10-29
lang: zh
---

> 从 10 条内容中筛选出 4 条重要资讯。

---

**Agentic CRM 与竞品**
1. [Slack Code API 正式上线](#item-crm-vendors-1) ⭐️ 7.0/10

**企业 AI 平台与运行时**
1. [AgentCore 企业平台蓝图](#item-ai-platform-1) ⭐️ 8.0/10
2. [Foundry 公测 Copilot harness](#item-ai-platform-2) ⭐️ 8.0/10

**分析师与研究**
1. [StreamVibe 研究动态意图](#item-research-1) ⭐️ 6.0/10

---

## Agentic CRM 与竞品

<a id="item-crm-vendors-1"></a>
### [Slack Code API 正式上线](https://www.salesforce.com/news/linked-content/introducing-the-slack-code-api-your-agents-your-team-one-code-channel/) ⭐️ 7.0/10

Salesforce 宣布 Slack Code API 已正式全面可用，开发者可让自研或 Slack Marketplace 中的开发智能体自动创建“代码频道”，加入相关人员与文件、持续发布任务进展，并在完成后归档频道。团队成员可在 Slack 内查看执行历史、补充上下文、审阅代码差异并批准变更；该能力沿用 Slack 现有的工作区控制、数据边界和消息合规机制，适用于有协同开发、人工审批或严格安全要求的企业。Salesforce 称，此前已有超过 150 家客户和合作伙伴申请构建相关体验；GitHub Copilot 则在 30%的智能体会话中开启专用代码频道，但这些数据均为厂商披露。

rss · Salesforce News · 10月28日 15:15

**「背景」** Slack Code 于同年 8 月推出，首批合作伙伴包括 Anthropic、Cognition、GitHub 和 Vercel，其核心“代码频道”是由开发智能体按任务创建的独立协作空间，用于集中人员、上下文、执行计划与审批。此次开放 Slack Code API，是将原先主要由少数合作伙伴使用的频道能力扩展给企业自建智能体和面向 Slack Marketplace 的第三方智能体。

**「竞争启示」** Slack 将智能体执行界面抽象为可复用的协作层：智能体负责具体任务和呈现方式，平台统一承载人员、上下文、执行记录、审批与合规控制。对企业 AI 平台而言，这种“智能体可替换、协作与治理界面稳定”的设计，可降低接入不同自研或第三方智能体时重复建设交互和审阅流程的成本。

**标签**: `#Salesforce`, `#Slack Code API`, `#开发智能体`, `#人机协作`, `#企业AI平台`

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [AgentCore 企业平台蓝图](https://aws.amazon.com/blogs/machine-learning/building-an-agentic-ai-platform-on-amazon-bedrock-agentcore/) ⭐️ 8.0/10

AWS 发布技术文章，介绍基于 Amazon Bedrock 与 Bedrock AgentCore 构建企业智能体平台的架构及参考实现，面向同时承载多个业务团队智能体的场景。AgentCore 提供运行时、网关、身份、记忆、策略、注册表和评估等模块化服务；配套的 Enterprise Agentic AI Platform Blueprint 则以基础设施即代码补充多账户边界、所有权、软件交付、可观测性、成本治理和退役机制。该方案要求推理与工具调用分别经过受控网关，并通过短期工作负载身份、运行时和记忆隔离、自动评估及生产晋级门禁，支持团队在预设边界内独立发布和回滚；文章未提供客户落地数据或价格信息。

rss · AWS Machine Learning Blog · 10月28日 18:28

**「背景」** Amazon Bedrock AgentCore 由运行时、网关、身份、记忆、策略、注册表和评估等模块化服务组成，用于构建、部署和运营智能体。此次介绍的 Enterprise Agentic AI Platform Blueprint 并非单一智能体应用，而是在 AgentCore 之上以基础设施即代码补充多账户边界、所有权、软件交付、可观测性、成本治理和退役机制。

**「平台启示」** 该架构将平台控制面与各业务团队的部署单元分离，并把模型访问、MCP 工具访问和评估晋级设计成独立治理关口，可减少团队自行拼装安全、交付和监控机制导致的控制漂移。成本归因随工作负载身份和调用遥测进入跨账户视图，也使按智能体、团队或业务单元实施预算管理和内部核算成为平台契约的一部分。

**标签**: `#Amazon Bedrock AgentCore`, `#Agent运行时`, `#多团队治理`, `#AgentOps与可观测性`, `#身份与隔离`

---

<a id="item-ai-platform-2"></a>
### [Foundry 公测 Copilot harness](https://devblogs.microsoft.com/foundry/microsoft-copilot-harness-in-foundry/) ⭐️ 8.0/10

微软在 Foundry Agent Service 中推出 Microsoft Copilot harness 公测版，并将托管智能体的长任务韧性能力转为正式可用。该托管运行时负责 Agent Loop、沙箱、工作上下文以及模型与工具调用编排，首批能力包括可复用技能、Foundry 与 MCP 工具连接、文件及代码执行、向内置子智能体委派受限任务，以及源码管理的智能体定义；身份验证、审批、执行限制和策略边界需要显式配置。开发者可选择受支持的 Foundry 模型，并自行提供知识、流程与工具，适用于市场研究、运营分析、内部规划等复杂长流程。客户案例方面，Confluence Technologies CTO 称其不到一周便运行了解决方案；Fashable 则将生成技术包、供应商协作和采购谈判描述为计划场景，并强调具有商业约束力的决定仍由人工控制，这些均属于客户陈述而非微软公布的量化成效。

rss · Microsoft Foundry Blog · 10月28日 16:45

**「背景」** 智能体 harness 是连接模型、上下文、工具、执行环境与控制策略的运行时层，负责协调多轮模型及工具调用、维护工作上下文并管理文件等执行资源。微软此次采用统一 harness 策略：平台提供托管的 Agent Loop 与沙箱，开发者可选择受支持的 Foundry 模型，并自行配置知识、流程和工具，而不必搭建完整的编排栈。

**「平台启示」** 这一设计将智能体平台拆分为微软托管的执行基础，以及客户维护的知识、流程、技能和工具层，并允许在受支持模型间切换而不重写编排。对 CRM+AI 产品而言，可复用技能、显式工具授权与审批、受限子任务委派及源码化定义，可以作为业务流程复用、权限治理和版本管理的独立设计层。

**标签**: `#Microsoft Foundry`, `#Agent Runtime`, `#Copilot harness`, `#长任务韧性`, `#托管智能体`

---

## 分析师与研究

<a id="item-research-1"></a>
### [StreamVibe 研究动态意图](https://www.jiqizhixin.com/articles/2026-10-28-9) ⭐️ 6.0/10

机器之心报道称，Google 等提出 StreamVibe，研究个人智能体如何在持续交互中结合用户背景、历史记忆和应用上下文，理解不断变化的用户意图。该项目目前属于研究线索，材料未提供具体方法、版本、评测数据、价格、开放范围或落地客户，也不能视为已上线产品能力。其潜在企业场景包括 Agentic CRM 中的连续客户意图识别、跨会话任务推进和长期目标管理。

rss · 机器之心 · 10月28日 09:19

**「背景」** StreamVibe 的研究对象更具体地说是主动式流媒体视频智能体，重点在于从连续交互中推断隐含意图、跟踪不断变化的请求，并判断何时及如何提供协助，而非泛指所有个人智能体。项目由 StreamVibe-Bench 基准、StreamVibe-VL 流式视觉语言模型和 StreamVibe-Harness 分层记忆框架组成。

**「研究启示」** 对 CRM+AI 产品设计的具体参考是，将相对稳定的用户背景、可持续更新的历史记忆和实时应用上下文分层管理，再用于动态意图判断；但 StreamVibe 如何实现这种组合以及效果如何，仍需论文方法与评测结果验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/papers/2610.34662">Paper page - StreamVibe : Proactive Video Agents for Evolving User...</a></li>
<li><a href="https://stream-vibe.github.io/">StreamVibe : Proactive Video Agents for Evolving User Intent</a></li>

</ul>
</details>

**标签**: `#Personal Agent`, `#StreamVibe`, `#动态意图理解`, `#用户记忆`, `#智能体研究`

---