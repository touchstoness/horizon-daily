---
layout: default
title: "Horizon Summary: 2026-11-25 (ZH)"
date: 2026-11-25
lang: zh
---

> 从 24 条内容中筛选出 6 条重要资讯。

---

**企业 AI 平台与运行时**
1. [Microsoft Foundry 更新智能体闭环](#item-ai-platform-1) ⭐️ 9.0/10
2. [Iceberg 新增目录标签](#item-ai-platform-2) ⭐️ 8.0/10
3. [OceanBase 发布 OceanLake](#item-ai-platform-3) ⭐️ 6.0/10

**Agent 协议与开发生态**
1. [Agents Python SDK 0.26 发布](#item-protocols-1) ⭐️ 6.0/10

**行业 AI 落地**
1. [LingSante Pulse 开源](#item-industry-1) ⭐️ 6.0/10
2. [GPT-6 展示蛋白质设计能力](#item-industry-2) ⭐️ 6.0/10

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [Microsoft Foundry 更新智能体闭环](https://devblogs.microsoft.com/foundry/whats-new-in-microsoft-foundry-ignite-2026/) ⭐️ 9.0/10

微软在 Ignite 2026 更新 Microsoft Foundry，覆盖智能体观测、评测、优化、训练、运行时控制、企业知识接入和模型管理。已正式可用的能力包括 Insights、多轮评测、语音智能体、外部智能体注册、A2A 工具、托管智能体出站控制、Foundry Dev Pack、Foundry CLI、Microsoft-Decision-1.1 和 Managed Compute；人工标注、规则评测器及 Agent Optimizer 的技能与成本优化仍处于预览阶段，Programmed Training 为公开预览，Foundry on AKS 为有限预览。微软明确表示 Agent Optimizer 不会自动修改生产智能体，企业可比较候选版本与当前基线后人工决定是否发布，适用于客服、语音服务和复杂业务流程智能体的持续改进与治理。微软披露，Gulf Air 在 Falcon Eye 的语音与聊天智能体上线前生成约 1 万个候选问题，并以每批约 100 个问题进行选测，同时保留人工审核环节。

rss · Microsoft Foundry Blog · 11月24日 16:00

**「背景」** 11 月 19 日的 Horizon 日报曾报道 Foundry Agent Service 的生产部署更新，重点包括已正式可用的托管智能体网络出口控制，以及部署至客户自有 AKS 集群的后续计划。此次平台总览进一步将出口控制列为 GA，但将 Foundry on AKS 标为有限预览，较此前所述“计划于 12 月上旬公开预览”提供了更审慎的当前可用性口径。【tool-1-1】

**「平台启示」** Foundry 将生产追踪、整段对话评测、候选修复测试和自定义训练串成“观测—评测—优化—训练”闭环，同时把生产发布保留为独立的人工决策点。这种分层方式可供 CRM+AI 平台参考：自动化发现问题和生成候选改动，但用版本基线、人工标注与发布审批控制生产风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://devblogs.microsoft.com/foundry/hosted-agents-foundry-agent-service-ignite-2026/">2026-11-19 — Foundry 托管智能体生产能力</a></li>

</ul>
</details>

**标签**: `#Microsoft Foundry`, `#Agent运行时`, `#评测与持续优化`, `#A2A与工具调用`, `#成本与模型路由`

---

<a id="item-ai-platform-2"></a>
### [Iceberg 新增目录标签](https://www.databricks.com/blog/sharing-catalog-metadata-across-data-platforms-engines-and-agents) ⭐️ 8.0/10

Databricks 宣布，Apache Iceberg REST Catalog API 已支持 catalog labels：通过 LoadTable 响应中的可选 labels 字段，以字符串键值对共享表级和列级的业务用途、所有权、敏感性及数据分类等上下文。Unity Catalog 已通过 Tag Exchange 公开其表和列标签；PyIceberg 则计划在下一版 0.13 中支持 Python 应用读取这些标签，尚属预告。该机制适用于跨数据平台和查询引擎的数据发现、治理，以及为企业 AI 智能体提供可移植的数据上下文；正文未披露价格、实际采用范围或落地效果。

rss · Databricks Blog · 11月24日 01:30

**「背景」** 企业的数据分类、业务用途和所有权等上下文通常保留在源目录中，跨平台使用时往往需要重复配置标签或维护自定义元数据同步管道。此次方案基于 Apache Iceberg REST Catalog API，在 LoadTable 响应中加入可选的 labels 字段，以字符串键值对形式传递表级和列级上下文，但不统一规定标签词汇及其解释方式。

**「平台启示」** 该设计将元数据交换格式与标签词汇、解释方式解耦：开放协议负责传递上下文，各平台仍可保留自身的标签体系、控制能力和处理逻辑。这种分层方式可减少 CRM+AI 智能体跨目录取数时重复建设元数据同步管道，但标签如何映射为权限或策略仍需由接入平台实现。

**标签**: `#Apache Iceberg`, `#元数据互操作`, `#数据治理`, `#智能体上下文`, `#Databricks`

---

<a id="item-ai-platform-3"></a>
### [OceanBase 发布 OceanLake](https://www.qbitai.com/2026/11/512330.html) ⭐️ 6.0/10

OceanBase 据条目标题发布湖库一体 AI 数据平台 OceanLake，并称其核心引擎将面向全球开源，产品定位指向企业 AI 的数据存储与分析基础设施。现有正文仅称“中国 AI 数据平台加速崛起”，未披露产品版本、具体架构、开源许可证与代码范围、价格、可用区域或客户案例，因此尚无法确认其实际开放程度及落地能力。

rss · 量子位 · 11月24日 03:30

**「背景」** OceanBase 此前已在 GitHub 维护其开源分布式数据库项目，并通过 GitHub Issues、Discord 等渠道接收问题与功能建议；此次所称 OceanLake 核心引擎开源，可视为其既有开源协作方式向 AI 数据平台方向的延伸，但现有材料尚未披露代码仓库、许可证及具体开放范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oceanbase/oceanbase">GitHub - oceanbase / oceanbase : OceanBase is the unified distributed...</a></li>

</ul>
</details>

**标签**: `#OceanBase`, `#OceanLake`, `#AI数据平台`, `#湖库一体`, `#开源`

---

## Agent 协议与开发生态

<a id="item-protocols-1"></a>
### [Agents Python SDK 0.26 发布](https://github.com/openai/openai-agents-python/releases/tag/v0.26.0) ⭐️ 6.0/10

OpenAI 已发布 Agents Python SDK v0.26.0，将 GPT-Live 演示升级至 1.1，并修复 Realtime 在回合结束时检查输出护栏、遵循全局追踪开关等问题。该版本还调整了 MCP 元数据优先级，保留 Session 历史中的交接脱敏，并加强 TAR 路径验证、Docker 存储挂载权限和本地镜像审批等安全控制。官方发布审查将其认定为兼容的小版本更新，继续支持 Python 3.10 及以上版本，适合构建实时客服、销售辅助及需要工具调用与会话交接的企业智能体。

github · openai-sdks\[bot\] · 11月24日 03:15

**「背景」** 此次更新从 v0.25.0 升级至 v0.26.0，共涉及 55 个文件；官方说明 Session 与 RunState 数据结构未变。其主要范围是工具、护栏、会话历史、Realtime、沙箱和示例维护，并非新的 Agent 协议或重大架构发布。

**「集成启示」** 对企业 Agent 平台的具体参考是，将治理控制覆盖到执行链路的不同层级：输入护栏拒绝后停止已排队工具，Realtime 在回合完成时检查输出护栏，同时在会话交接历史中持续保留脱敏结果。MCP 元数据采用“单次调用配置优先于发现阶段默认值”的机制，也为多租户或按请求覆盖连接配置提供了明确的优先级设计。

**标签**: `#OpenAI Agents SDK`, `#Python`, `#Realtime`, `#安全修复`, `#版本更新`

---

## 行业 AI 落地

<a id="item-industry-1"></a>
### [LingSante Pulse 开源](https://www.jiqizhixin.com/articles/2026-11-24-6) ⭐️ 6.0/10

11 月 24 日，蚂蚁百灵宣布开源医疗健康预测模型 LingSante Pulse；据厂商介绍，该模型可理解人体日常生理信号，预测未来六年内 150 种疾病表型的发生风险。其定位不同于面向单一生理信号或特定疾病的传统模型，可用于长期健康风险筛查、健康管理和人群风险分层等场景。现有材料未披露开源地址、模型架构、训练数据、验证指标、价格、部署方式或临床客户，因此预测能力及临床适用性目前仍属于厂商宣称。

rss · 机器之心 · 11月24日 06:25

**「背景」** 医疗健康 AI 的应用正从疾病识别和健康咨询向长期风险预测延伸。来源称，传统预测模型通常围绕单一生理信号或特定疾病训练，而 LingSante Pulse 试图利用日常生理信号覆盖多种疾病表型。

**「行业启示」** 该产品体现了一种从“识别当前疾病”转向“按时间跨度预测多种疾病表型风险”的产品设计思路，可为健康管理平台统一组织生理信号输入、风险周期和多病种输出提供参考；但进入企业或临床流程前，仍需补充数据来源、外部验证和风险阈值等治理信息。

**标签**: `#医疗健康AI`, `#疾病风险预测`, `#生理信号`, `#开源模型`, `#蚂蚁百灵`

---

<a id="item-industry-2"></a>
### [GPT-6 展示蛋白质设计能力](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities) ⭐️ 6.0/10

OpenAI 称，GPT-6 模型可结合推理与代码设计蛋白质结构和序列，实验室测试已在五个靶点上观察到结合证据。该能力可能适用于药物发现和蛋白质工程的早期候选设计，但官方尚未披露靶点名称、实验方法、成功率、对照结果、模型开放范围、价格或客户应用，因此现阶段只能视为厂商公布的实验结果，无法据此判断产品化效果。

rss · OpenAI News · 11月24日 13:00

**「背景」** 此次披露涉及从目标三维结构出发设计新蛋白质序列，以及重新设计抗体中负责结合靶点的区域，任务重点不只是预测既有蛋白质结构，而是生成候选结构与序列。现有公开页面仅说明实验室在五个靶点上观察到结合证据，尚未披露靶点、实验方法、对照结果或模型开放方式。

**「行业启示」** 这一案例体现了“模型推理与代码生成—结构及序列设计—实验室验证”的闭环思路；面向生命科学的企业 AI 平台若采用类似路径，需要将模型产出与可追溯的实验数据、对照设计和结果评估连接起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/">GPT - 6 models demonstrate intrinsic protein - design ... | OpenAI</a></li>

</ul>
</details>

**标签**: `#蛋白质设计`, `#生命科学AI`, `#生成式AI`, `#实验验证`

---