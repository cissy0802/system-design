# Topics Roadmap

源是仓库中的文件本身（`ls *-{day,week,book,issue}*.html`）。本文件只是主题查找表：N → 主题。超过现有编号时 routine 会 append 新主题。

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
- Day 25: CDN 与 Edge — Cloudflare 架构, Edge compute, Cache invalidation, Anycast
- Day 26: 文件存储 — S3 架构, Object vs Block vs File, 上传下载优化, Backup
- Day 27: 权限与账号系统 — RBAC vs ABAC, Multi-tenancy, Org/Team/Project 层级, Audit log
- Day 28: 全文搜索与推荐集成 — BM25 + vector, 重排序, Multi-stage retrieval, Snippet 生成
- Day 29: LLM 服务架构 — 请求路由与负载均衡, Streaming response, Prompt caching, Cost/latency/quality 三角
- Day 30: AI 产品后端 — RAG 架构, Agent loop 服务化, Embedding 服务设计, 人机协同
