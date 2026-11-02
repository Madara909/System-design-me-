# System Design — Case Study Series (0 → Senior)

A complete, beginner-friendly-to-senior system design curriculum. Each chapter is a standalone case study following the same structure:

1. **Problem framing** — what and why
2. **Step 1 — Requirements & scope** (functional, non-functional, clarifying questions)
3. **Back-of-the-envelope estimation**
4. **Step 2 — High-level design** (API, data model, architecture diagram)
5. **Step 3 — Deep dive** (the hard parts, alternatives, trade-offs)
6. **Step 4 — Wrap up** (bottlenecks, failure modes, monitoring)
7. **Senior-level notes** — what separates a strong hire from a hire
8. **Interview Questions** — warm-up → core → deep → discussion

All diagrams are **Mermaid** (renders natively on GitHub, Obsidian, VS Code, Notion).

---

## Part I — Foundations

| # | Chapter | Status |
|---|---|---|
| 02 | [Scale From Zero To Millions Of Users](./02-scale-from-zero-to-millions-of-users.md) | ✅ Done |
| 03 | [Back-of-the-Envelope Estimation](./03-back-of-the-envelope-estimation.md) | ✅ Done |
| 04 | [A Framework For System Design Interviews](./04-a-framework-for-system-design-interviews.md) | ✅ Done |

## Part II — Building Blocks

| # | Chapter | Status |
|---|---|---|
| 05 | [Design A Rate Limiter](./05-design-a-rate-limiter.md) | ✅ Done |
| 06 | Design Consistent Hashing | ⏳ Batch 2 |
| 07 | Design A Key-Value Store | ⏳ Batch 2 |
| 08 | Design A Unique ID Generator In Distributed Systems | ⏳ Batch 2 |
| 09 | Design A URL Shortener | ⏳ Batch 2 |
| 10 | Design A Web Crawler | ⏳ Batch 3 |

## Part III — Consumer-Scale Systems

| # | Chapter | Status |
|---|---|---|
| 11 | Design A Notification System | ⏳ Batch 3 |
| 12 | Design A News Feed System | ⏳ Batch 3 |
| 13 | Design A Chat System | ⏳ Batch 3 |
| 14 | Design A Search Autocomplete System | ⏳ Batch 4 |
| 15 | Design YouTube | ⏳ Batch 4 |
| 16 | Design Google Drive | ⏳ Batch 4 |

## Part IV — Location & Geo Systems

| # | Chapter | Status |
|---|---|---|
| 17 | Proximity Service | ⏳ Batch 5 |
| 18 | Nearby Friends | ⏳ Batch 5 |
| 19 | Google Maps | ⏳ Batch 5 |

## Part V — Infrastructure & Data Systems

| # | Chapter | Status |
|---|---|---|
| 20 | Distributed Message Queue | ⏳ Batch 6 |
| 21 | Metrics Monitoring and Alerting System | ⏳ Batch 6 |
| 22 | Ad Click Event Aggregation | ⏳ Batch 6 |
| 24 | Distributed Email Service | ⏳ Batch 7 |
| 25 | S3-like Object Storage | ⏳ Batch 7 |

## Part VI — Transactional & Financial Systems

| # | Chapter | Status |
|---|---|---|
| 23 | Hotel Reservation System | ⏳ Batch 7 |
| 26 | Real-time Gaming Leaderboard | ⏳ Batch 8 |
| 27 | Payment System | ⏳ Batch 8 |
| 28 | Digital Wallet | ⏳ Batch 8 |
| 29 | Stock Exchange | ⏳ Batch 8 |

---

## How to study this

**If you're a beginner:** read 02 → 03 → 04 in order. Do not skip. Then do 09 (URL shortener) — it's the gentlest full design. Then 05, 06, 08.

**If you're prepping for interviews in 2 weeks:** 04 (framework) → 03 (estimation) → then 09, 12, 13, 11, 15. Those five cover ~70% of what's actually asked.

**If you're senior:** skim the designs, read only the **Senior-level notes** sections and attempt the **Deep / senior** interview questions cold. If you can't answer them out loud in 3 minutes, read the chapter.

## Cross-cutting concepts (appear in many chapters)

| Concept | First introduced | Reused in |
|---|---|---|
| Horizontal scaling / statelessness | 02 | everywhere |
| Caching & cache-aside | 02 | 07, 09, 12, 14, 26 |
| Sharding & partition keys | 02 | 06, 07, 09, 13, 20 |
| Consistent hashing | 06 | 07, 20, 25 |
| CAP theorem / quorum (N, W, R) | 07 | 20, 25, 27 |
| Message queues & async workers | 02 | 11, 20, 21, 22, 27 |
| Fanout on write vs read | 12 | 13, 18 |
| Long polling / WebSocket / SSE | 13 | 11, 18, 26 |
| Idempotency & exactly-once | 05 | 20, 22, 27, 28 |
| Geohash / quadtree | 17 | 18, 19 |
