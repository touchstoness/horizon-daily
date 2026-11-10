---
layout: default
title: "Horizon Summary: 2026-11-10 (ZH)"
date: 2026-11-10
lang: zh
---

> 从 25 条内容中筛选出 5 条重要资讯。

---

**企业 AI 平台与运行时**
1. [Genie One 接入 Sendoso](#item-ai-platform-1) ⭐️ 7.0/10
2. [Bedrock 知识库扩展检索模式](#item-ai-platform-2) ⭐️ 7.0/10
3. [千问办公 2.0 发布 Team Agent](#item-ai-platform-3) ⭐️ 6.0/10

**本体、语义层与知识图谱**
1. [Neo4j 展示 Agentic GraphRAG 工具](#item-ontology-1) ⭐️ 7.0/10

**行业 AI 落地**
1. [Kuken 用 AI 检索 70 年图纸](#item-industry-1) ⭐️ 8.0/10

---

## 企业 AI 平台与运行时

<a id="item-ai-platform-1"></a>
### [Genie One 接入 Sendoso](https://www.databricks.com/blog/turn-buying-signals-pipeline-sendoso-gifts-genie-one) ⭐️ 7.0/10

Databricks 官方博客介绍，Genie One 可通过 Databricks Marketplace 中的 Sendoso MCP Server，将治理数据上的自然语言分析与赠礼操作连接起来；管理员完成一次接入后，业务用户即可在 Genie One 中调用 Sendoso 工具。演示流程包括识别意向升温且没有赠礼历史的目标账户、根据账户上下文推荐礼品并起草留言，以及由用户预览和批准赠礼，预览阶段不产生扣费。执行后，用户可通过发送 ID 追踪礼品，并在发货前取消；赠礼历史保存在同一工作区的表中，可供 Genie One 汇总，适用于销售跟进、客户维护和活动营销等场景。文中的账户与意向数据均为演示示例，未提供该集成带来销售管道增长的可复核客户成效数据。

rss · Databricks Blog · 11月9日 17:29

**「背景」** Databricks 将合作方 MCP Server 作为 Genie One 从治理数据分析走向业务动作的接入方式：管理员连接 Marketplace 中的 Sendoso 服务后，业务团队可在现有工作区调用其工具。本文以示例说明，用户可依据意向数据拟定赠礼、审批后发送，并在同一工作区查看发送记录；示例账户和数据为说明用途。

**「平台启示」** 这一集成展示了企业 Agent 将分析连接到业务执行的具体方式：用工作区数据提供行动上下文，通过 MCP 调用外部业务工具，在执行前加入人工确认，并将动作历史保留在可查询的数据表中。对 CRM+AI 产品设计而言，发送 ID、发货前取消和历史查询为业务动作提供了追踪与纠错入口；但材料没有展开权限映射或效果归因机制，不能据此认定已具备完整的治理与归因能力。

**标签**: `#Databricks Genie One`, `#MCP Server`, `#企业智能体平台`, `#工具调用`, `#数据治理`

---

<a id="item-ai-platform-2"></a>
### [Bedrock 知识库扩展检索模式](https://aws.amazon.com/blogs/machine-learning/single-shot-and-agentic-retrieval-with-amazon-bedrock-managed-knowledge-base/) ⭐️ 7.0/10

AWS 宣布 Amazon Bedrock Managed Knowledge Base 的 AgenticRetrieveStream 现已支持单次 RAG 和仅检索请求，并继续提供已有的智能体检索模式。单次 RAG 只检索一次，再调用基础模型根据命中文段生成带引用的答案；仅检索模式直接返回匹配文段，不生成答案；智能体检索则将复杂问题拆成子查询，在配置的迭代上限内执行、评估并补充多轮搜索。企业可通过同一 API 按请求选择模式，例如用单次 RAG 处理直接的政策查询，用智能体检索比较多份制度文件，或让员工直接审阅仅检索模式返回的原文；文中银行助手属于说明性示例，未提供真实客户、价格及完整成本或延迟数据。

rss · AWS Machine Learning Blog · 11月9日 20:13

**「背景」** Amazon Bedrock Managed Knowledge Base 此前已提供智能体检索：由基础模型拆分问题、执行多轮搜索，并在配置的迭代上限内评估和补充证据。此次新增的单次 RAG 与仅检索模式，分别适用于一次检索后生成答案，以及直接返回匹配段落供应用或用户处理的场景。

**「平台启示」** 该设计把仅检索、单次生成和多轮规划统一到同一接口，并通过请求级参数调节检索投入，为企业 AI 平台按问题复杂度控制模型调用、检索深度和可审查性提供了具体实现思路。Trace 事件可呈现规划与检索步骤，也为开发阶段检查复杂问答的证据获取过程提供了观测入口。

**标签**: `#Amazon Bedrock`, `#企业知识库`, `#RAG`, `#智能体检索`, `#检索接口`

---

<a id="item-ai-platform-3"></a>
### [千问办公 2.0 发布 Team Agent](https://www.qbitai.com/2026/11/508694.html) ⭐️ 6.0/10

11 月 9 日，千问办公发布 2.0 版本。报道标题称，该版本推出支持多人与 Agent 协作的 Team Agent；现有材料未提供具体功能、可用范围、价格或客户数据，企业协作场景的适用方式仍无法进一步确认。

rss · 量子位 · 11月9日 08:34

**「背景」** 千问办公属于 2026 年集中出现的桌面办公 Agent 产品之一；一篇行业盘点将其与 WorkBuddy、Kimi Work、TraeWork、AiPy 并列为当年上半年密集上线的产品。现有材料未提供千问办公此前版本的能力信息，因此无法判断 2.0 相较前版的具体变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://juejin.cn/post/7672915108385685531">2026 年 办 公 Agent ...</a></li>

</ul>
</details>

**标签**: `#千问办公`, `#Team Agent`, `#多智能体协作`, `#企业办公`

---

## 本体、语义层与知识图谱

<a id="item-ontology-1"></a>
### [Neo4j 展示 Agentic GraphRAG 工具](https://neo4j.com/blog/developer/agentic-graphrag-and-an-explorer-for-your-own-stack/) ⭐️ 7.0/10

Neo4j 开发者博客介绍了 graph-explorer-kit：该 Python 工具基于 neo4j-graphrag，可读取 Aura 中由 Document Intelligence 生成的知识图谱，通过检索器、智能体工具或 HTTP API 接入应用，并由 Graph Explorer 展示答案生成过程及支持人工补充图数据。作者以 240 份 UFO 解密文件测试完整流程，最终形成 54,044 条记录、58,429 条关系和 24,971 个段落；其中实体可回溯至原始段落和 PDF，但文章未提供可量化的回答质量或生产落地效果。该工具适合需要把文档知识图谱接入企业问答、调查分析或 CRM 智能体，并保留来源追溯能力的场景。

rss · Neo4j Blog · 11月9日 08:39

**「背景」** Neo4j 的 Document Intelligence 可将文件转换为 Aura 中的知识图谱；本文所述 graph-explorer-kit 建立在 neo4j-graphrag 之上，读取该图并通过 API 将检索与智能体接入应用。

**「建模启示」** 该方案把领域配置集中在 ProjectSpec 中，统一定义图模式、抽取规则、Cypher 示例和种子问题，并将 Claim、Evidence、Redaction 作为节点表达相互矛盾或被遮盖的材料。它还允许在 Document Intelligence 原有向量旁保存自选模型生成的嵌入，并提供 dry-run 和 undo，体现了语义检索层与原始知识图谱分离、增量适配且可回退的集成方式。

**标签**: `#Neo4j`, `#GraphRAG`, `#知识图谱`, `#智能体`, `#文档智能`

---

## 行业 AI 落地

<a id="item-industry-1"></a>
### [Kuken 用 AI 检索 70 年图纸](https://openai.com/index/kuken) ⭐️ 8.0/10

Kuken Industries 通过 OpenAI API 构建冷却塔工程图纸检索能力，覆盖其 70 年的历史图纸资料。OpenAI 披露，工程师查找维修所需图纸的时间已从接近 1 小时缩短至 4.5 分钟；材料未说明系统架构、部署规模及效果验证方式。该能力适用于工业制造企业的设备维修、历史工程资料查询和企业知识检索场景。

rss · OpenAI News · 11月9日 08:00

**「背景」** 冷却塔维修需要查找与设备相关的历史工程图纸；Kuken Industries 的案例聚焦于将这类跨越数十年的图纸用于维修检索。来源未说明图纸的数字化方式或检索系统架构。

**「行业启示」** 这一案例表明，企业知识检索的对象可以从文本扩展到长期积累的工程图纸，并以维修任务所需的查找时间作为可量化指标。对于 CRM+AI 或企业 AI 平台，类似能力可考虑连接售后服务流程与工程资料库，但材料未披露具体的图纸解析、索引和权限治理机制。

**标签**: `#工业制造`, `#企业知识库`, `#工程图纸检索`, `#OpenAI API`, `#维修智能化`

---