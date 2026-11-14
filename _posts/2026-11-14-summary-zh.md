---
layout: default
title: "Horizon Summary: 2026-11-14 (ZH)"
date: 2026-11-14
lang: zh
---

> 从 26 条内容中筛选出 5 条重要资讯。

---

**企业 AI 平台与运行时**
1. [AgentCore Runtime V2 会话启动](#item-ai-platform-1) ⭐️ 8.0/10
2. [Amazon Bedrock 推理成本归因](#item-ai-platform-2) ⭐️ 8.0/10

**本体、语义层与知识图谱**
1. [Adyen Architect 关联服务依赖](#item-ontology-1) ⭐️ 7.0/10

**AI 评测、治理与安全**
1. [Introducing ChatGPT Wallet](#item-governance-1) ⭐️ 7.0/10

**分析师与研究**
1. [清华提出 CoACT 压缩上下文](#item-research-1) ⭐️ 6.0/10

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [AgentCore Runtime V2 会话启动](https://aws.amazon.com/blogs/machine-learning/architecture-patterns-for-fast-session-startup-on-amazon-bedrock-agentcore-runtime/) ⭐️ 8.0/10

AWS 介绍 Amazon Bedrock AgentCore Runtime V2：运行时在创建或更新时初始化容器、等待健康检查通过，再保存微型虚拟机的内存与磁盘快照；新会话通过恢复快照启动，并回收会话未使用的内存。AWS 称此机制可让会话启动更快且更稳定，但材料未提供具体性能或成本数据；构建快照会使每次创建或更新运行时耗时数分钟。该方案面向需要降低 Agent 冷启动等待的交互式聊天、语音场景，也适用于代码审查、理赔处理等长时间运行的任务；部分 Agent 需调整初始化流程或添加构建钩子才能充分受益。

rss · AWS Machine Learning Blog · 11月13日 22:02

**「背景」** AgentCore Runtime 为每个会话提供独立的隔离 microVM，并可在无任务时缩至零。此前的 Horizon 日报曾介绍其 Session Endpoints 可用于在会话内预览智能体构建的 Web 应用；本次内容聚焦运行时 V2 如何通过环境快照恢复加快新会话启动，属于同一运行时的不同能力。

**「平台启示」** V2 将环境初始化与会话启动分为两个阶段，并以快照恢复承接新会话；设计 Agent 时可把可复用的进程状态放在初始化阶段，同时注意镜像文件首次读取仍可能产生延迟。对于要求亚秒启动的场景，文中还建议在用户打开应用或聊天窗口时后台预热会话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/machine-learning/preview-web-apps-live-as-your-coding-agent-builds-them-with-amazon-bedrock-agentcore-runtime/">2026-10-31 — AgentCore 支持应用实时预览</a></li>

</ul>
</details>

**标签**: `#Amazon Bedrock AgentCore`, `#Agent运行时`, `#会话启动优化`, `#快照恢复`, `#资源与成本管理`

---

<a id="item-ai-platform-2"></a>
### [Amazon Bedrock 推理成本归因](https://aws.amazon.com/blogs/machine-learning/cost-attribution-and-controls-for-ai-developer-and-productivity-tools-on-amazon-bedrock/) ⭐️ 8.0/10

AWS 介绍了 Amazon Bedrock 面向 AI 开发与效率工具的推理成本归因方式：Bedrock 在 bedrock-runtime 和 bedrock-mantle 端点记录调用方 IAM ARN，并可将 IAM 主体标签或联邦会话标签带入 CUR 2.0，供 Athena 查询及 Cost Explorer 筛选。该机制按主体和用量类型、依 CUR 导出周期汇总，不提供逐请求成本；逐提示词明细需使用模型调用日志或请求元数据标签。文章还介绍了 Bedrock 原生用量控制，并以联邦身份配置、团队和成本中心标签为实施路径，适用于按用户或团队分析 AI 工具支出、开展预算规划与成本治理；材料未给出价格或具体控制限额。

rss · AWS Machine Learning Blog · 11月13日 18:44

**「背景」** Amazon Bedrock 的成本归因可按推理调用记录 IAM 主体，并将组织标签带入 CUR 2.0 和 Cost Explorer；CUR 按主体及用量类型、每个导出周期汇总，不提供逐请求成本。若需查看单次提示的细节，文章建议结合模型调用日志或请求元数据标签。

**标签**: `#Amazon Bedrock`, `#成本归因`, `#FinOps`, `#IAM 身份`, `#企业 AI 平台`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [Adyen Architect 关联服务依赖](https://neo4j.com/blog/genai/a-45-minute-answer-to-one-question/) ⭐️ 7.0/10

Neo4j 官方博客介绍了 Adyen 的 Architect：一个近实时、可查询的平台关系图，用于回答工程师“某项服务依赖什么”。系统分别构建服务图、代码图和基础设施图：覆盖约 3,000 个在线服务及约 47 万条服务调用、约 25 万个类和 6,000 多个模块，以及数万台主机；追踪数据每秒最多处理 700 万个 span。三张图保留为独立 Neo4j 数据库，并通过复合数据库供单条 Cypher 查询跨图访问；来源称查询可返回原本需要代理读取的数千行上下文，但未提供可复核的效果数据。该做法适用于需要在故障排查时关联代码、运行时调用与部署基础设施的工程平台。

rss · Neo4j Blog · 11月13日 09:43

**「背景」** 服务依赖信息分散在代码、运行时追踪和主机基础设施等不同工具中，静态架构图也可能与实际运行情况存在偏差。Architect 将这三类数据分别维护为图数据库，再通过复合数据库供单条 Cypher 查询跨图访问；各图按各自的数据变化节奏刷新。

**「建模启示」** Architect 将代码、运行时追踪和基础设施分别建图，并按各自变化节奏更新，再通过复合数据库跨图查询；这为企业知识平台提供了一种保留数据域与更新管道独立性、同时让应用统一查询关联上下文的具体设计参考。

**标签**: `#Neo4j`, `#Adyen`, `#知识图谱`, `#服务依赖映射`, `#企业上下文引擎`

---

## AI 评测、治理与安全

<a id="item-governance-1"></a>
### [Introducing ChatGPT Wallet](https://openai.com/index/introducing-chatgpt-wallet) ⭐️ 7.0/10

ChatGPT Wallet 让相关智能体在用户批准和现有银行卡保护下完成购买。

rss · OpenAI News · 11月13日 15:00

**标签**: `#智能体权限`, `#用户审批`, `#交易安全`, `#OpenAI`

---

## 分析师与研究

<a id="item-research-1"></a>
### [清华提出 CoACT 压缩上下文](https://www.jiqizhixin.com/articles/2026-11-13-4) ⭐️ 6.0/10

机器之心报道称，清华提出面向 Coding Agent 的 CoACT，并以 ICSE 2027 为题介绍；标题宣称该方法可降低 33% 的 Token 开销。报道指出，Coding Agent 在查看代码、修改程序和运行测试时，会不断将文件内容、搜索结果及日志累积到上下文中，导致后续每轮调用成本上升。现有材料未披露 CoACT 的具体实现、实验基线、任务完成率或适用范围，因此无法确认 33% 降幅的验证条件；其潜在适用场景是企业代码智能体的上下文管理与推理成本控制。

rss · 机器之心 · 11月13日 06:40

**「背景」** ICSE 是 IEEE/ACM 国际软件工程会议，ICSE 2027 计划于 2027 年 4 月 25 日至 5 月 1 日在爱尔兰都柏林举行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://conf.researchr.org/home/icse-2027">ICSE 2027</a></li>

</ul>
</details>

**标签**: `#Coding Agent`, `#智能体架构`, `#上下文压缩`, `#Token 开销`, `#软件工程研究`

---