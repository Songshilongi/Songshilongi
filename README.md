<h1>Hi there, I'm Songshilong 👋</h1>

<h2>🧰 技术栈 & 📊 GitHub 使用语言统计</h2>

<table>
  <tr>
    <td valign="top" width="50%">
      <strong>技术栈</strong><br /><br />
      <img src="https://skillicons.dev/icons?i=nodejs,python,java,go,mysql,redis,docker,git,mongodb,vscode,idea,postman,maven&perline=5" alt="skills" />
    </td>
    <td valign="top" width="50%">
      <strong>GitHub 使用语言统计</strong><br /><br />
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Songshilongi&layout=compact&langs_count=8" alt="GitHub Top Languages" />
    </td>
  </tr>
</table>

## 工作经历

| 时间                | 公司             | 职位            |
|-------------------|----------------|---------------|
| 2025.02 - 2026.04 | SAP Labs China | SAP 钻石级杰出人才计划 |
| 2024.08 - 2025.01 | 壹沓科技           | Java 开发实习生    |

---

## 项目经历

### Nexus AI Chat（个人开源项目）

> **角色**：全栈开发  
> **时间**：2025.11 - 至今

**项目地址**

- 后端：<https://github.com/Songshilongi/Nexus-backend>
- 前端：<https://github.com/Songshilongi/Nexus-frontend>（基于 Google Gemini 进行 Vibe Coding）

**项目简介**

Nexus 为用户提供便捷的 LLM API 配置中心管理与 MCP 资源管理。用户注册并配置相关 API 与 MCP 资源后，即可在聊天框内输入文本进行对话和
MCP Tool 调用。项目实际效果基于阿里百炼 API 完成测试。

**项目技术栈**

`Spring Boot` `Spring WebFlux` `MongoDB` `Redis` `MySQL` `Prompt Engineering` `Agent`

**主要贡献**

- 负责后端用户模块（注册、登录、密码重置、邮箱验证码找回密码）、LLM API 配置管理、MCP 资源管理模块功能实现，包含项目搭建、通用组件封装、Docker
  镜像构建。
- 利用自定义注解 `AgentTool` 与 Spring Boot 事件监听机制，实现项目启动后本地自定义工具的注册与发现；并基于 MCP 协议完成远程
  MCP Tool 资源的发现与调用。
- 围绕用户名唯一登录机制，使用布隆过滤器存储已注册用户名，配合 `Redisson` 对目标用户名加锁，防止重复注册与并发竞争，保证用户名全局唯一。

### SAP Ariba Invoice

> **单位**：思爱普（中国）有限公司（钻石级杰出人才计划）  
> **时间**：2025.02 - 至今

**项目简介**

基于 SAP BTP 平台构建企业级发票解决方案，支持发票上传、集中管理、全球化落地与报表生成，提升发票处理效率、准确性与合规性，并与
SAP Business Network 等企业系统深度集成。

**项目职责**

- 参与印度、意大利 Globalization 功能开发，完成当地发票与税率政策适配。
- 编写并维护测试用例，相关场景通过率达到 100%。
- 在团队内持续沉淀技术认知，围绕 LLM、Agent、MCP 完成 3 次技术分享。

**项目技术栈**

`Spring Boot` `SAP CAP` `SAP HANA DB` `SAP BTP` `SAP Business Network`

**主要贡献**

- 基于现有字段，完成印度商品/服务税、供应商、商品分类、服务分类在 API、UI、S/4 集成链路中的兼容与适配。
- 为 Import Master Data 模块新增意大利 Withholding Tax 支持，实现客户通过 CSV 上传自定义发票导入规则。
- 基于 Feature Toggle 机制实现印度与意大利需求的按需启停，降低变更风险并保障客户系统稳定运行。

### 需求开发提效 Agent

> **单位**：思爱普（中国）有限公司（钻石级杰出人才计划）  
> **时间**：2025.06 - 至今

**项目简介**

需求开发提效 Agent（POC 项目）帮助开发人员检索现有开发文档，管理跨服务调用、包方法调用、API
调用等关系，提升项目管理与开发效率。支持需求一键分析、影响面自动估算、QA 测试文档生成等功能，为正式进入编码阶段前提供技术支持。项目完成后，向
GLO CIM 全球负责人做过技术路线与业务价值汇报。

**项目职责**

- 负责基于 SAP 现有 AI 套件开发 Agent 助手，实现各类 RAG Agent 组件。
- 针对用户案例实现工作流编排，针对非用户案例实现动态需求生成处理。
- 为服务调用、包方法调用、API 调用等关系定义模型并构建知识图谱。

**项目技术栈**

`Prompt Engineering` `Agent` `RAG` `LangChain` `Neo4j` `Flask` `SAP HANA`

**主要贡献**

- 利用 ESLint 自定义代码扫描逻辑，实现对现有 Node 项目依赖包/方法级别调用关系的自动解析，解决图谱数据来源问题。
- 基于 LangChain 自定义实现类管理历史对话记录，结合 SAP Gen AI SDK 封装模块化 Agent 组件，在此基础上构建以图谱、API
  文档、需求总结文档为核心的多 RAG Agent 协作智能体。
- 基于 Prompt Engineering 进行提示词调优，提升 Cypher 查询自动生成、QA 测试文档生成、影响面文档生成的稳定性。
- 利用 Python `subprocess` 模块运行 Git 命令，解决 CIM 项目 RAG 数据源自动拉取与同步问题。

### 物流可视化平台

> **单位**：壹沓科技（上海）有限公司（Java 开发实习生）  
> **时间**：2024.08 - 2025.01

**项目简介**

面向企业物流全流程，提供节点跟踪、时效预测、异常监控告警、分析报表与决策仪表盘等能力，解决传统物流信息不透明、数据分散、追踪困难等问题，支撑物流环节精细化管理与效率优化。

**项目职责**

- 负责物流可视化平台业务迭代，参与存量代码优化与技术改造，并处理线上日志告警信息。
- 实习期间独立承担港口拥堵/台风预警模块与内部配置交互后台开发，覆盖方案设计、评审、开发与测试全过程。

**项目技术栈**

`Spring Boot` `MySQL` `Redis` `MongoDB` `MyBatis-Plus` `RocketMQ` `Nacos` `OpenFeign` `XXL-JOB` `ShardingSphere`

**主要贡献**

- 基于阿里云 ARMS 进行接口调用链与火焰图分析，定位慢 SQL 并完成优化：生产环境查询近半年用户订阅数据（约 807W）接口响应时间从
  `2.4s` 降至 `190ms`。
- 针对定时任务集中扫描导致的 CPU 突增问题，引入线程池 + MQ 异步削峰处理，将记录并行分发至清洗流程，优化 CPU 峰值并提升系统稳定性。
- 对港口拥堵模块每日写入的 `3W+` 数据执行写入/查询链路优化：外部接口分批请求、响应异步落库，并对表结构增加时间字段 Range
  分区，显著提升查询性能与历史数据维护效率。
- 面向约 `1700W` 级定时任务表，调研并落地分区/分表方案：分区按订阅类型字段进行水平拆分，分表基于 ShardingSphere +
  自定义路由策略实现规则分发。
- 重构预警通知模块，基于模板方法 + 策略 + 责任链模式抽象推送流程，支持多来源消息自动路由与处理，降低迭代成本。
- 通过注解与反射实现 JSONPath、SpEL 表达式动态生成/更新，适配 DTO 与规则模型变化，支持页面化配置通知规则。

### 基于多智能体协作的多模态化学信息抽取（硕士课题）

> **单位**：华东理工大学（硕士研究生）
> **时间**：2024.03 - 至今

**项目简介**

项目支持对文本、分子结构图、反应方程式图、Reaxys 文献中的化合反应数据进行抽取并转储为结构化信息，旨在为化学实验人员提供端到端的信息抽取解决方案。

**项目职责**

- Java 端负责构建项目基础框架与业务功能开发。
- Python 端负责实现核心抽取方法与策略。

**项目技术栈**

`Spring Boot` `MongoDB` `Redis` `MySQL` `Prompt Engineering` `AutoGen` `RocketMQ` `FastAPI`

**主要贡献**

- 利用 Prompt Engineering 中的思维链与少样本提示优化提示词，实现文本模态反应参数提取准确率达到 `85%+`。
- 利用 VLM 与 YOLO 增强现有示意图解析方法：在标识符评估策略下准确率从 `58.62%` 提升至 `77.03%`，在 SMILES 评估策略下准确率从
  `47.41%` 提升至 `54.11%`。
- 整合现有信息抽取方法，在 Prompt Engineering 基础上，基于 Chat Group 多智能体架构并结合 AutoGen
  构建协作式信息抽取系统；提供基于模板与抽象问题的提示词案例，路由并解决问题成功率达到 `98.99%`。

---

## 📫 联系我

- Email: `songshilong0503@163.com`

---
