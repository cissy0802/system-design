# Topics Roadmap

> **⚠️ routine 须知**：本表即全部计划。只写下面**已列出**的条目；**全部写完就停**——别自己发明新主题、别往本文件加行。写完只发一条 PushNotification 请 BigCat 补充。（新条目由 BigCat / deep-research 反哺加进本表，届时你自然继续写。）

源是仓库中的文件本身（`ls *-{day,week,book,issue}*.html`）。本文件是主题查找表：N → 主题。

**本路线图已收口：Day 1–48 封顶，不再自动续写。** Day 45–48 为查漏补缺补齐的分布式系统硬核（共识协调 / 数据库内部 / 网络基础 / 容器编排）——此前只有 CAP 与区块链 PoW/PoS，缺真正的 Raft/Paxos 协调层。

- Day 1: Scalability 基础 — Vertical vs Horizontal scaling, Load balancing, Stateless services, 容量规划
- Day 2: 缓存 (Caching) — Cache layers, LRU/LFU/ARC, Cache-aside vs Write-through vs Write-back, Cache invalidation
- Day 3: 数据库选型 — SQL vs NoSQL, OLTP vs OLAP, ACID vs BASE, Postgres/DynamoDB/Cassandra/Redis 选型
- Day 4: 数据库分片 (Sharding) — Hash sharding vs Range sharding, Consistent hashing, Hot spots, Resharding
- Day 5: 复制 (Replication) — Leader-Follower vs Multi-leader vs Leaderless, Sync vs Async, Read replicas, Replication lag
- Day 6: 一致性 — Strong vs Eventual vs Causal, Read-your-writes, Monotonic reads, CAP 定理
- Day 7: 分布式事务 — 2PC, 3PC, Saga 模式, Outbox pattern, 为什么微服务要避免分布式事务
- Day 8: 消息队列 — Kafka vs RabbitMQ vs SQS, 投递语义, Backpressure, DLQ
- Day 9: API 设计 — REST vs GraphQL vs gRPC, Pagination, Versioning, Rate limiting
- Day 10: Rate Limiting — Token bucket vs Leaky bucket, Sliding window, Distributed rate limiting, Stripe 案例
- Day 11: 唯一 ID 生成 — UUID, Snowflake, KSUID, ULID
- Day 12: 搜索系统 — Inverted index, Elasticsearch 架构, 在线 vs 离线索引, Vector search
- Day 13: 推荐系统 — Collaborative filtering vs Content-based, Two-tower model, Cold start, LLM-based recommendation
- Day 14: Feed 系统 — Push vs Pull vs Hybrid, Twitter timeline, Fanout-on-write 限制, Ranking pipeline
- Day 15: 聊天系统 — WhatsApp/Discord 架构, WebSocket vs Long polling, 消息递交保证, E2E 加密
- Day 16: 视频流系统 — Netflix 架构, HLS/DASH adaptive streaming, CDN 设计, 转码 pipeline
- Day 17: 支付系统 — Idempotency, Stripe 架构, 分布式事务, 对账与核验
- Day 18: 订阅与计费 — Stripe billing, 预付 vs 后付, Proration, 多货币与税务
- Day 19: 地理系统 — Geo-indexing, S2 vs Geohash vs Uber H3, 附近查询, Uber dispatch
- Day 20: 计算作业系统 — Batch (Spark) vs Stream (Flink), Lambda vs Kappa, Watermark, Exactly-once
- Day 21: 监控与可观测性 — Metrics vs Logs vs Traces, OpenTelemetry, SLI/SLO/SLA, On-call
- Day 22: 上线与发布 — Blue-Green vs Canary vs Rolling, Feature flags, Backwards compatibility, DB migration
- Day 23: 可靠性 — Circuit breaker, Retry with backoff, Bulkhead, Graceful degradation
- Day 24: 安全基础 — AuthN vs AuthZ, OAuth2 / OIDC, JWT vs session, Secret management
- Day 25: 系统设计面试 — 需求澄清与范围界定, 4 步框架(功能/非功能→高层设计→深挖→权衡), 白板沟通与出声推理, 常见失分点(过早抠细节/不问假设/不谈 trade-off/不画图)
- Day 26: 容量估算与假设 — Back-of-envelope 估算, QPS/存储/带宽/内存推导, 数量级直觉(2 的幂 + 延迟数字), 如何显式声明并校验假设; 区分面试 vs 生产(面试靠 BOTE + 出声 justify, 生产靠真实指标/压测/可观测性回归, 见 Day 27)
- Day 27: 成本与容量工程 — 容量规划, 成本归因, 自动扩缩容, 资源效率
- Day 28: CDN 与 Edge — Cloudflare 架构, Edge compute, Cache invalidation, Anycast
- Day 29: 文件存储 — S3 架构, Object vs Block vs File, 上传下载优化, Backup
- Day 30: 权限与账号系统 — RBAC vs ABAC, Multi-tenancy, Org/Team/Project 层级, Audit log
- Day 31: 全文搜索与推荐集成 — BM25 + vector, 重排序, Multi-stage retrieval, Snippet 生成
- Day 32: LLM 服务架构 — 请求路由与负载均衡, Streaming response, Prompt caching, Cost/latency/quality 三角
- Day 33: AI 产品后端 — RAG 架构, Agent loop 服务化, Embedding 服务设计, 人机协同
- Day 34: 实时系统 — WebRTC, 实时协作传输, 低延迟架构, 实时游戏后端
- Day 35: 物联网与边缘 — IoT 数据摄取, 边缘计算, MQTT, 时序数据库
- Day 36: 区块链与分布式账本 — 共识算法(PoW/PoS), 智能合约架构, 去中心化存储, 性能权衡
- Day 37: 多租户 SaaS 架构 — 租户隔离, 数据分区, 资源配额, 计费集成
- Day 38: 数据湖与湖仓 — 数据湖 vs 数仓 vs 湖仓, Iceberg/Delta, 元数据管理, 批流一体
- Day 39: 工作流引擎 — Temporal/Airflow, Saga 编排, 持久化执行, 补偿事务
- Day 40: 特征平台与 ML 基础设施 — 特征存储, 在线/离线一致, 模型服务, A/B 实验平台
- Day 41: 快于人类反应的系统 — 把人移出快回路(自动检测+止血/熔断/Kill Switch), 限爆炸半径(Cell/隔板/Shuffle Sharding), 变更安全(金丝雀+自动回滚+Error Budget, 先护栏后规模), 可观测驱动自动决策(Knight Capital/Perrow)
- Day 42: 全球化与多区域 — 数据驻留, 多活架构, 跨区域一致性, 延迟优化
- Day 43: 隐私与合规架构 — GDPR 删除权, 数据脱敏, 审计追踪, 同意管理
- Day 44: 混沌工程与韧性测试 — 故障注入, 游戏日, 韧性验证, 金丝雀深化
- Day 45: 协作编辑系统 — OT vs CRDT, 冲突解决, 离线同步, Figma/Notion 架构

<!-- ↓ 查漏补缺追加（Day 46–49）：分布式系统硬核 -->
- Day 46: 分布式共识与协调 — Raft/Paxos, Leader election 选主, 分布式锁, Zookeeper/etcd, Quorum 与脑裂
- Day 47: 数据库内部与存储引擎 — B-tree vs LSM-tree, WAL 与崩溃恢复, MVCC, 索引内部与查询优化器
- Day 48: 网络基础 — TCP/UDP, HTTP/1.1·2·3·QUIC, DNS, TLS 握手, L4 vs L7 负载均衡
- Day 49: 容器与编排 — 容器原理(namespace/cgroup), Kubernetes 核心对象, Service Mesh(Envoy/Istio), 调度与自愈
- Day 50: 把 Code Review 当信号检测系统 — 误报预算与分诊层, 降噪架构(ReviewFilter/nitpick 过滤), AI 评论的信噪治理, 活动指标 vs 结果指标的度量陷阱(钩子·源自 deep-research #2)
- Day 51: 低底率下的告警系统 — 基率谬误的工程后果(低单次错误率 × 极低真报底率 = 报告级误报淹没真报, Argus 消融证明器 0/20 vs LLM 裁判 20/20), 独立 oracle 兜底 vs LLM 自任裁判, 分诊层的精确率地板, 报告级 vs 判定级误报率的度量陷阱, 与 Day 44 混沌工程/Day 50 信号检测的接口(钩子·源自 deep-research #5)
- Day 52: 给混沌工程装一个正确性 oracle — 传统故障注入只验可用性(还活着吗)不验正确性(故障下有没有静默返回错结果); 差分 oracle(同输入跑参照路径 vs 故障路径, 结果归一化后 checksum 比对)把"静默错结果"变成可 diff; 归一化层(全列定序/浮点量化/屏蔽非确定函数)+ 三态裁决(通过/可接受降级/正确性 bug); 参照跑用独立路径防错误趋同; AI 只坐生成器席产故障场景不当裁判(承 Day 44 混沌工程/Day 51 低底率告警; 钩子·源自 deep-research #5)
- Day 53: 项目风险要按肥尾管理 — 均值超支可控(IT +73%)但一in六黑天鹅 +200%、超支>50% 的 18% 平均 +447%(Flyvbjerg 1.6万项目库); 风险模型盯均值 vs 盯尾部的工程区别(预留金/止损线/分阶段承诺); "多杆全中"式成功定义如何制造假失败率(CHAOS 16.2% 与 0.5% 同构); 与容量规划 P99 思维的同源性(钩子·源自 deep-research #6)
- Day 54: Fail obviously — 给 AI 工作流做失效可见性设计 — Bainbridge 1983 的处方在 LLM 时代成为最难一条(LLM 的失效模式是"错得流畅"); 失效可见性工程(结构化断言/可执行自检/差异高亮, 让错误自曝而非靠人盯); 核验成本工程(给终审席配一条比重做便宜得多的核对路径——解释只在真降核验成本时降低过度依赖, Vasconcelos/Zhang 边界); 终审席位设计四参数(底率/核验成本/练习剂量/失效可见性, 承 Day 51 低底率告警)(钩子·源自 deep-research #7)
