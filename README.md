# Mohamed Saba — Backend Engineer

Backend engineer focused on distributed systems and infrastructure tooling.
CS student at Capital University. I build things that other systems depend on.

---

## Projects

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
Published   3 npm packages
```

---

## Currently

- 📍 Cairo, Egypt
- 🎓 Computer Science @ Capital University
- 🔭 Building infrastructure tooling for backend developers
- 📦 Open to backend / backend-infrastructure roles

---

<a href="[https://linkedin.com/in/mohamedsabea](https://linkedin.com/in/mohamedsabea)">LinkedIn</a> · <a href="mailto:mohamedsabawork@gmail.com">Email</a>
