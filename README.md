# Mohamed Saba — Backend Engineer

Backend engineer focused on distributed systems and infrastructure tooling.
CS student at Capital University. I build things that other systems depend on.

---

## Projects

### [Airlock](https://github.com/mohamedsaba/airlock)

Production-grade Transactional Outbox library for NestJS solving the Dual-Write Problem — the silent data loss that occurs between a database commit and a broker publish. Implements a Claim-Lease model that decouples the DB lock from the network call, preventing connection pool exhaustion. Built around 10 production invariants: poison pill containment, bounded memory (OOM protection), DB-authoritative time to eliminate clock drift, chunked GC with SKIP LOCKED, producer idempotency, serialization guards, and graceful SIGTERM draining. Uses partial indexes to keep the polling hot-path index minimal even at 10M+ processed rows.

`NestJS` `PostgreSQL` `Kafka` `RabbitMQ` `TypeORM` `TypeScript` `npm package`

---

### [isIdempotent](https://github.com/mohamedsaba/isIdempotent)
Distributed idempotency protection library for NestJS to prevent double-spend and retry-storm anomalies in distributed transactions. Implements atomic distributed locking via Redis and custom Lua scripts, coupled with deep-sorted SHA-256 request fingerprinting to eliminate key collisions. Features a resilient O(1) memory store with lazy expiration and status-aware caching for production-grade scale.

`NestJS` `Redis` `Lua` `TypeScript` `npm package`

---

### [Distributed Rate Limiter as a Service](https://github.com/mohamedsaba/RateLimiterSDK)
Multi-tenant rate limiting microservice with REST API and npm SDK. Implemented three algorithms — fixed window, sliding window log, and sliding window counter — using Redis sorted sets and atomic Lua scripts to eliminate race conditions under concurrent load. Supports 2,000+ req/sec at sub-5ms p99.

`NestJS` `Redis` `Lua` `BullMQ` `TypeScript` `Docker` `npm SDK`

---

### [Webhook Delivery Engine](https://github.com/mohamedsaba/webhook-engine)
Webhook delivery service guaranteeing at-least-once event delivery with exponential backoff retries, HMAC-SHA256 payload signing, and idempotency key deduplication. API and worker run as separate scalable services. Includes a real-time delivery log dashboard via SSE.

`NestJS` `BullMQ` `Redis` `TypeScript` `Next.js` `Docker` `npm SDK`

---

### [BullMQ Metrics](https://github.com/mohamedsaba/bullmq-metrics)

Zero-configuration Prometheus metrics exporter for BullMQ. Auto-discovers all Queues and Workers in a NestJS application and exposes queue depth, job throughput, execution latency, wait time, retry counts, and worker count via `prom-client`. Uses a hybrid monitoring approach — real-time event listeners for throughput and latency, lightweight polling for queue depth. Cluster-ready with configurable global/local event modes to prevent metric over-counting in distributed environments. Supports dynamic job labels for extracting business data (e.g., `tenant_id`, `user_id`) into metrics.

`NestJS` `BullMQ` `Prometheus` `TypeScript` `npm package`

---

### [NestJS AuthKit](https://github.com/mohamedsaba/Nestjs-AuthKit)

Production-grade authentication and session management library for NestJS targeting "Day 2" auth problems. Implements Refresh Token Family rotation with automatic reuse detection — a reused token flags a potential theft and immediately revokes the entire session family. Provides instant session revocation via a Redis-backed blocklist, native TOTP 2FA with Google Authenticator/Authy support, and simple RBAC decorators. Stateful security layer without sacrificing JWT performance.

`NestJS` `Redis` `JWT` `TypeScript` `npm package`

---

### [League of Legends Competitive Analytics Engine](https://github.com/mohamedsaba/TRUSIGHT)
Full-stack competitive gaming analytics and matchmaking system. MMR calculation engine using KNN algorithm, player performance tracking, Redis caching layer, and Riot Games API integration. Built as a pnpm monorepo with a shared mmr-engine package.

`NestJS` `Next.js` `Redis` `TypeScript` `BullMQ` `Riot API` `pnpm monorepo`

---

## Stack

```
Backend     NestJS · TypeScript · Node.js · REST · BullMQ
Databases   Redis · PostgreSQL · MongoDB · MySQL
DevOps      Docker · Docker Compose · Railway
Frontend    Next.js · React · Tailwind CSS
Published   4 npm packages
```

---

## Currently

- 📍 Cairo, Egypt
- 🎓 Computer Science @ Capital University
- 🔭 Building infrastructure tooling for backend developers
- 📦 Open to backend / backend-infrastructure roles

---

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohamedsabea/) · <a href="mailto:mohamedsabawork@gmail.com">Email</a>
