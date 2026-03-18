# Hi there, I'm Songshilong 👋

<p>
	<a href="https://github.com/Songshilongi">
		<img src="https://img.shields.io/github/followers/Songshilongi?label=Followers&style=social" alt="GitHub followers" />
	</a>
	<img src="https://komarev.com/ghpvc/?username=Songshilongi&label=Profile%20views&color=0e75b6&style=flat" alt="profile views" />
</p>

## 🧰 技术栈

<p>
	<img src="https://skillicons.dev/icons?i=nodejs,python,java,go,mysql,redis,docker,git,vscode,idea" />
</p>

## 工作经历

| 时间 | 公司 | 职位           |
|---|---|--------------|
| 2025.02 - 2026.04 | SAP Labs China | SAP钻石级杰出人才计划 |
| 2024.08 - 2025.01 | 壹沓科技 | Java 开发实习生   |

## 项目经历  

### SAP Ariba Invoice

> 思爱普（中国）有限公司（钻石级杰出人才计划）  
> 2025.02 - 至今

**项目简介**  
基于 SAP BTP 平台构建企业级发票解决方案，支持发票上传、集中管理、全球化落地与报表生成，提升发票处理效率、准确性与合规性，并与 SAP Business Network 等企业系统深度集成。

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

### 物流可视化平台

> 壹沓科技（上海）有限公司（Java 开发实习生）  
> 2024.08 - 2025.01

**项目简介**  
面向企业物流全流程，提供节点跟踪、时效预测、异常监控告警、分析报表与决策仪表盘等能力，解决传统物流信息不透明、数据分散、追踪困难等问题，支撑物流环节精细化管理与效率优化。

**项目职责**
- 负责物流可视化平台业务迭代，参与存量代码优化与技术改造，并处理线上日志告警信息。
- 实习期间独立承担港口拥堵/台风预警模块与内部配置交互后台开发，覆盖方案设计、评审、开发与测试全过程。

**项目技术栈**  
`Spring Boot` `MySQL` `Redis` `MongoDB` `MyBatis-Plus` `RocketMQ` `Nacos` `OpenFeign` `XXL-JOB` `ShardingSphere`

**主要贡献**
- 基于阿里云 ARMS 进行接口调用链与火焰图分析，定位慢 SQL 并完成优化：生产环境查询近半年用户订阅数据（约 807W）接口响应时间从 `2.4s` 降至 `190ms`。
- 针对定时任务集中扫描导致的 CPU 突增问题，引入线程池 + MQ 异步削峰处理，将记录并行分发至清洗流程，优化 CPU 峰值并提升系统稳定性。
- 对港口拥堵模块每日写入的 `3W+` 数据执行写入/查询链路优化：外部接口分批请求、响应异步落库，并对表结构增加时间字段 Range 分区，显著提升查询性能与历史数据维护效率。
- 面向约 `1700W` 级定时任务表，调研并落地分区/分表方案：分区按订阅类型字段进行水平拆分，分表基于 ShardingSphere + 自定义路由策略实现规则分发。
- 重构预警通知模块，基于模板方法 + 策略 + 责任链模式抽象推送流程，支持多来源消息自动路由与处理，降低迭代成本。
- 通过注解与反射实现 JSONPath、SpEL 表达式动态生成/更新，适配 DTO 与规则模型变化，支持页面化配置通知规则。


## 📫 联系我

- Email: `songshilong0503@163.com`
---
