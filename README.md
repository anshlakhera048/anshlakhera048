<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1f2e,100:A371F7&height=200&section=header&text=Ansh%20Lakhera&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=Backend%20Engineer%20%C2%B7%20Distributed%20Systems%20%C2%B7%20Low-Latency%20Systems&descAlignY=58&descSize=18&descColor=8b949e" alt="Ansh Lakhera, Backend Engineer" />
</div>

<div align="center">

**I build correctness-critical backend systems: exchange engines, event-driven payments and real-time streaming pipelines.**
<br/>
SDE intern at Tripfactory · B.Tech, Nirma University · **Open to SDE / Backend roles**

[![Resume](https://img.shields.io/badge/Resume-A371F7?style=for-the-badge&logo=readme&logoColor=white)](https://drive.google.com/file/d/1sHOIbc7x4L0uW8tgWos_Qcyf5aePHv_G/view?usp=sharing)
[![Portfolio](https://img.shields.io/badge/Portfolio-161B22?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.anshlakhera.in)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ansh-lakhera/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anshlakhera048@gmail.com)
[![Instagram](https://img.shields.io/badge/@swe.ngineer-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/swe.ngineer)

<table>
<tr>
<td align="center"><h3>400K / sec</h3>orders matched<br/>at 3µs p50<br/><sub><a href="https://github.com/anshlakhera048/AxiomX">AxiomX</a></sub></td>
<td align="center"><h3>1,000+ TPS</h3>payments validated<br/>with k6 load tests<br/><sub><a href="https://github.com/anshlakhera048/Distributed-Payment-Infrastructure">Payments</a></sub></td>
<td align="center"><h3>3★ | 1638</h3>#56 · Starters 251<br/>CodeChef<br/><sub><a href="#-competitive-programming">Details</a></sub></td>
<td align="center"><h3>35K+ / mo</h3>views teaching<br/>backend and systems<br/><sub><a href="https://instagram.com/swe.ngineer">@swe.ngineer</a></sub></td>
</tr>
</table>

[**🌱 Open Source**](#-open-source-contributions) · [**🚀 Projects**](#-featured-projects) · [**💼 Experience**](#-experience) · [**🛠️ Stack**](#️-tech-stack) · [**🏆 CP**](#-competitive-programming)

</div>

---

## 🌱 Open Source Contributions

<div align="center">

[![Merged PRs](https://img.shields.io/github/issues-search?query=is%3Apr%20is%3Amerged%20author%3Aanshlakhera048%20-user%3Aanshlakhera048&label=Merged%20PRs&color=A371F7&style=for-the-badge&logo=git&logoColor=white)](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3Aanshlakhera048+-user%3Aanshlakhera048)
[![Open PRs](https://img.shields.io/github/issues-search?query=is%3Apr%20is%3Aopen%20author%3Aanshlakhera048%20-user%3Aanshlakhera048&label=Open%20PRs&color=238636&style=for-the-badge&logo=github&logoColor=white)](https://github.com/pulls?q=is%3Apr+is%3Aopen+author%3Aanshlakhera048+-user%3Aanshlakhera048)
[![Issues Reported](https://img.shields.io/github/issues-search?query=is%3Aissue%20author%3Aanshlakhera048%20-user%3Aanshlakhera048&label=Issues%20Opened&color=D29922&style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/issues?q=is%3Aissue+author%3Aanshlakhera048+-user%3Aanshlakhera048)

</div>

> Contributing upstream to projects I use and learn from. This table updates automatically with my latest merged PRs.

<!--OSS-START-->
| Project | Contribution | Merged |
|---|---|---|
| [JayPokale/Chisle](https://github.com/JayPokale/Chisle) | [feat: report turns in agentic benchmark score](https://github.com/JayPokale/Chisle/pull/35) | 2026-10-04 |
| [JayPokale/Chisle](https://github.com/JayPokale/Chisle) | [feat: add 2026-10-01 rerun benchmark chart](https://github.com/JayPokale/Chisle/pull/34) | 2026-10-03 |
| [JayPokale/Chisle](https://github.com/JayPokale/Chisle) | [feat: break replay savings down by tool](https://github.com/JayPokale/Chisle/pull/30) | 2026-10-03 |
| [SINTEF/Muscade.jl](https://github.com/SINTEF/Muscade.jl) | [docs: move Diagnostic under User manual](https://github.com/SINTEF/Muscade.jl/pull/112) | 2026-10-02 |
<!--OSS-END-->

<div align="center">

[**View all my PRs →**](https://github.com/pulls?q=is%3Apr+author%3Aanshlakhera048+-user%3Aanshlakhera048)

</div>

---

## 🚀 Featured Projects

### ⚡ [AxiomX](https://github.com/anshlakhera048/AxiomX) — Deterministic exchange matching engine
![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Disruptor](https://img.shields.io/badge/LMAX_Disruptor-4B0082?style=flat-square)
![Agrona](https://img.shields.io/badge/Agrona-555?style=flat-square)
![fastutil](https://img.shields.io/badge/fastutil-555?style=flat-square)
![HdrHistogram](https://img.shields.io/badge/HdrHistogram-555?style=flat-square)

> A continuous limit order book with price-time priority, FIX gateway, event sourcing and crash recovery, built so every run produces the same result.

| Throughput | Latency | Hot path | Correctness |
|---|---|---|---|
| **400K orders/sec** (250K under mixed load) | **3µs p50** | **8M FIX parses/sec**, zero GC on the matching loop | **116 tests**, deterministic replay from snapshots |

**Key design decisions**
- **Single-writer principle:** many producers feed an Agrona MPSC queue, one publisher feeds a single-producer Disruptor, so ordering is strict with no lock contention.
- **Price-time book:** TreeMap + FIFO price levels give O(log N) match and O(1) cancel.
- **Zero-allocation hot path:** object pooling and primitive collections keep GC off the matching loop.
- **Event sourcing:** every state change is logged, so a crash recovers to the exact same state.

<details>
<summary><b>Architecture</b></summary>

```mermaid
flowchart LR
  C["Clients"] --> G["FIX gateway"] --> R["Order router by instrument"]
  R --> Q
  subgraph P["Per-instrument partition"]
    Q["MPSC ingress queue"] --> I["Single-writer publisher"] --> D["Disruptor ring buffer"] --> M["Matching engine"]
    M --> L["Event log and snapshots"]
    M --> W["Market data over WebSocket"]
  end
```

</details>

<br/>

### 💳 [Distributed Payment Infrastructure](https://github.com/anshlakhera048/Distributed-Payment-Infrastructure)
![Spring](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Grafana](https://img.shields.io/badge/Prometheus_%2B_Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

> An event-driven payment platform designed so there are no duplicate charges and no lost transactions, even when infrastructure fails.

| Scale | Consistency | Idempotency | Resilience |
|---|---|---|---|
| **1,000+ TPS** validated with k6 | **Double-entry ledger**, SUM(DEBIT) = SUM(CREDIT) enforced | **3 tiers:** Redis, DB lock, UNIQUE constraint | Outbox, retries, DLQs, circuit breakers, adaptive backpressure |

**Key design decisions**
- **Transactional outbox:** the payment and its event commit in one DB transaction, which removes the dual-write problem.
- **Effectively-once processing:** idempotent API plus a `processed_events` table make Kafka redeliveries harmless.
- **Two-stage fraud detection:** rules first, then an IsolationForest model with versioning, behind a circuit breaker that fails open.

<details>
<summary><b>Payment flow</b></summary>

```mermaid
sequenceDiagram
  participant C as Client
  participant G as API Gateway
  participant P as Payment Service
  participant K as Kafka
  participant F as Fraud Service
  C->>G: POST /payments with Idempotency-Key
  G->>P: JWT check and rate limit
  P->>P: Payment and outbox event in one DB transaction
  P->>K: Outbox publisher emits payment.created
  K->>F: fraud.request
  F->>K: fraud.result from rules and ML model
  K->>P: Finalize as SUCCESS with ledger entries, or FRAUD_REJECTED
```

</details>

<br/>

### 📊 [QuantStream](https://github.com/anshlakhera048/QuantStream) — Real-time market feature pipeline
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Flink](https://img.shields.io/badge/Flink-E6526F?style=flat-square&logo=apacheflink&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Avro](https://img.shields.io/badge/Avro_%2B_Schema_Registry-555?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

> Binance trade stream to SMA, VWAP and volatility features, served from an online store and an offline store that are continuously checked against each other.

| Throughput | Semantics | Dual store | Testing |
|---|---|---|---|
| **10-20K events/sec** | **Exactly-once** ingest-to-state path, RocksDB with 5s checkpoints | Redis (online) + ClickHouse (offline), **5% drift alerts** | Deterministic replay, load generator, **chaos service**, 16-service Compose stack |

**Key design decisions**
- **Event-time windows:** 60s windows sliding every 5s with watermarks, aggregated incrementally in O(1) per event.
- **Schema discipline:** Avro with Schema Registry, idempotent producers and a DLQ, so bad data is isolated rather than dropped.
- **Verifiable by design:** the repo includes chaos tests for Kafka, Redis and Flink failures, plus consistency and data-quality checkers.

<details>
<summary><b>Architecture</b></summary>

```mermaid
flowchart LR
  B["Binance WebSocket"] --> I["Ingestion service"] --> K[("Kafka ticks")]
  K --> F["Flink: sliding windows, RocksDB, exactly-once"]
  F --> RD[("Redis online store")]
  F --> CH[("ClickHouse offline store")]
  RD --> A["Feature API and signals"]
  I -. failed messages .-> DLQ["DLQ"]
  RD -. "drift check" .- CH
```

</details>

---

## 💼 Experience

**Tripfactory** · SDE Intern · Bengaluru · *Jan 2026 - Jun 2026*
- Integrated BPoint REST v5 into B2B booking infrastructure, owning the auth-to-settlement lifecycle across a multi-gateway architecture.
- Built an **idempotent FSM refund engine** with excess-refund prevention and precision-safe arithmetic under concurrency.
- Audited the **CDC pipeline** (Postgres, Debezium, Kafka, ClickHouse) and designed a star-schema warehouse with MergeTree materialized views.
- Built a config-driven **Visa Rule Engine** in Java and a BI dashboard (JS + Chart.js) used across 36+ offices with role-based access.

**Bluestock Fintech** · SDE Intern · Remote · *May 2025 - Jun 2025*
- Built a real-time IPO market dashboard (React, Node, Tailwind) with a modular, WebSocket-ready architecture.

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Stack |
|---|---|
| **Languages** | Java · C++ · Python · JavaScript · SQL |
| **Backend** | Spring Boot · REST · Microservices · Resilience4j |
| **Streaming and data** | Kafka · Flink · Avro · Schema Registry · Debezium (CDC) |
| **Low-latency** | LMAX Disruptor · Agrona · fastutil · HdrHistogram |
| **Storage** | PostgreSQL · ClickHouse · Redis |
| **Patterns** | Outbox · Saga · Idempotency · Event sourcing · Double-entry ledger |
| **Infra and observability** | Docker · Kubernetes · Prometheus · Grafana · Linux · k6 |

<sub>Also: React · Node.js · Tailwind · JUnit · Mockito</sub>

</div>

---

## 🏆 Competitive Programming

<div align="center">

| Platform | Handle | Highlight |
|---|---|---|
| **LeetCode** | [`anshlakhera048`](https://leetcode.com/u/anshlakhera048) | **Top 3.3% globally** (rank 1011 of 30,750+, Biweekly 148) · max rating 1648 |
| **CodeChef** | [`anshlakhera048`](https://www.codechef.com/users/anshlakhera048) | **3★** · global rank 74 in Starters 251 · max rating 1601 |
| **Codeforces** | [`ansh174`](https://codeforces.com/profile/ansh174) | Active · graphs and DP |

<sub>500+ DSA problems solved across platforms</sub>

</div>

---

## 📡 Teaching what I build

I run **[@swe.ngineer](https://instagram.com/swe.ngineer)**, where I explain backend engineering, system design and AI to **35K+ viewers a month**. Explaining a concept clearly is the best test of whether I understand it.

---

<div align="center">

### Let's talk

**Hiring for backend, distributed systems or low-latency work?**

[![Email me](https://img.shields.io/badge/Email_me-anshlakhera048%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anshlakhera048@gmail.com)
[![LinkedIn](https://img.shields.io/badge/Connect_on-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ansh-lakhera/)

</div>
