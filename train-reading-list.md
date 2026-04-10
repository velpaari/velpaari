# Reading List — Level Up to Principal/SE5

## Priority: ★★★ = Read this week | ★★ = Read before interview | ★ = When you have time

---

## 1. PAYMENT SYSTEMS & PARTNER INTEGRATIONS

### ★★★ Must-Read for Netflix
- [How Stripe Builds Payment Processing at Scale](https://stripe.com/blog/payment-api-design) — Stripe Engineering Blog. API design, idempotency keys, exactly-once delivery. **Directly maps to Netflix Partner Payments.**
- [Designing Robust and Predictable APIs with Idempotency](https://stripe.com/blog/idempotency) — Stripe. The definitive guide on idempotency in payment systems. **Memorize this pattern.**
- [Avoiding Double Payments in a Distributed Payments System](https://medium.com/airbnb-engineering/avoiding-double-payments-in-a-distributed-payments-system-2981f6b070bb) — Airbnb Engineering. Real-world dedup in payments. Extremely relevant.
- [The Architecture of Stripe's Payment System](https://newsletter.pragmaticengineer.com/p/stripe-engineering) — Pragmatic Engineer. High-level view of how Stripe handles billions in payments.

### ★★ Deep Dive
- [Building a Reliable Payment Gateway](https://engineering.mercadolibre.com/en/building-a-reliable-payment-gateway) — MercadoLibre. Latin America's largest payment processor. Reconciliation patterns.
- [How Netflix Uses Payment Tokens](https://netflixtechblog.com/) — Search for payment-related posts on Netflix Tech Blog.
- [Double-Entry Bookkeeping for Engineers](https://martin.kleppmann.com/2011/03/07/accounting-for-computer-scientists.html) — Martin Kleppmann (DDIA author). Why ledgers work the way they do.
- [Payment State Machines at Square](https://developer.squareup.com/blog/) — Square Engineering. State machine patterns for payment lifecycle.

---

## 2. DISTRIBUTED SYSTEMS (Core Knowledge)

### ★★★ Must-Read
- [Designing Data-Intensive Applications (DDIA)](https://dataintensive.net/) — Martin Kleppmann. **THE book.** Key chapters for you:
  - Chapter 5: Replication (DynamoDB Global Tables, Redis replication)
  - Chapter 6: Partitioning (DynamoDB partition keys, hot partitions)
  - Chapter 8: Distributed Systems Trouble (failure modes, exactly-once)
  - Chapter 9: Consistency and Consensus (eventual consistency trade-offs)
  - Chapter 11: Stream Processing (event-driven architecture)
- [The Amazon Builders' Library](https://aws.amazon.com/builders-library/) — Amazon's internal engineering practices, made public. **Gold mine:**
  - [Avoiding insurmountable queue backlogs](https://aws.amazon.com/builders-library/avoiding-insurmountable-queue-backlogs/)
  - [Making retries safe with idempotent APIs](https://aws.amazon.com/builders-library/making-retries-safe-with-idempotent-APIs/)
  - [Timeouts, retries, and backoff with jitter](https://aws.amazon.com/builders-library/timeouts-retries-and-backoff-with-jitter/)
  - [Caching challenges and strategies](https://aws.amazon.com/builders-library/caching-challenges-and-strategies/)
  - [Using load shedding to avoid overload](https://aws.amazon.com/builders-library/using-load-shedding-to-avoid-overload/)

### ★★ Deep Dive
- [The Log: What every software engineer should know](https://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying) — Jay Kreps (Kafka creator). Why event logs are fundamental.
- [How Slack Built Shared Channels](https://slack.engineering/how-slack-built-shared-channels/) — Multi-tenant architecture at scale.
- [Consistent Hashing Explained](https://systemdesign.one/consistent-hashing-explained/) — Visual guide. Relevant for DynamoDB partition understanding.

---

## 3. NETFLIX ENGINEERING (Know Their Stack)

### ★★★ Must-Read Before Netflix Interview
- [Netflix Tech Blog](https://netflixtechblog.com/) — Read the 10 most recent posts. Shows what they care about NOW.
- [Scaling Netflix's API via GraphQL Federation](https://netflixtechblog.com/how-netflix-scales-its-api-with-graphql-federation-part-1-ae3557c187e2) — How Netflix serves API at scale. **Directly relevant to Partner API work.**
- [Netflix Zuul 2: The Netflix Journey to Asynchronous, Non-Blocking Systems](https://netflixtechblog.com/zuul-2-the-netflix-journey-to-asynchronous-non-blocking-systems-45947377fb5c) — Their API gateway. Know this for partner API design discussions.
- [Rapid Event Notification System at Netflix](https://netflixtechblog.com/rapid-event-notification-system-at-netflix-6deb1d2b57d1) — Event-driven architecture at Netflix.
- [Netflix Cosmos Platform](https://netflixtechblog.com/the-netflix-cosmos-platform-35c14d9351ad) — How Netflix thinks about platform engineering (you're interviewing for a platform team).

### ★★ Deep Dive
- [Resilience Engineering at Netflix — Chaos Monkey](https://netflixtechblog.com/the-netflix-simian-army-16e57fbab116) — Chaos engineering. Expect failure mode questions.
- [How Netflix Microservices Tackle Dataset Pub-Sub](https://netflixtechblog.com/) — Event streaming patterns.
- [Netflix Culture Deck](https://jobs.netflix.com/culture) — **Read this.** It's assessed in every round.

---

## 4. SYSTEM DESIGN INTERVIEW PREP

### ★★★ Must-Read
- [The System Design Primer](https://github.com/donnemartin/system-design-primer) — GitHub. 200K+ stars. Comprehensive reference.
- [Hello Interview — What is Expected at Each Level](https://www.hellointerview.com/blog/the-system-design-interview-what-is-expected-at-each-level) — **Critical read.** Maps exactly to L5/L6/L7 expectations.
- [interviewing.io System Design Guide](https://interviewing.io/guides/system-design-interview) — Framework used by top interviewers.
- [ByteByteGo](https://blog.bytebytego.com/) — Alex Xu's blog. Visual system design explanations. **Read weekly.**

### ★★ Practice Problems (Netflix-relevant)
- Design a payment processing system (Stripe-style)
- Design a webhook delivery system (like Stripe/Twilio)
- Design a subscription management platform
- Design a partner API gateway with rate limiting
- Design a reconciliation system for financial transactions

---

## 5. STAFF+ CAREER & INTERVIEW STRATEGY

### ★★★ Must-Read
- [StaffEng.com — Guides](https://staffeng.com/guides/) — Will Larsen. **The definitive resource for Staff+ careers.**
  - [Staff-plus Interview Process](https://staffeng.com/guides/staff-plus-interview-process/)
  - [Interviewing for Staff-plus Roles](https://staffeng.com/guides/interviewing-staff-plus-roles/)
  - [Staff Engineer Archetypes](https://staffeng.com/guides/staff-archetypes/) — Know which archetype you are
- [The Pragmatic Engineer Newsletter](https://newsletter.pragmaticengineer.com/) — Gergely Orosz. Industry insights, comp data, interview trends. **Subscribe.**
- [Levels.fyi](https://www.levels.fyi/) — Comp benchmarks for Netflix SE5, Google L7, etc.

### ★★ Deep Dive
- *Staff Engineer* book — Will Larsen. How Staff+ engineers operate day-to-day.
- [Senior Engineer Interviews in 2025-2026](https://medium.com/@rohitverma_87831/senior-engineer-interviews-in-2025-2026-what-actually-decides-your-offer-a-real-unfiltered-dd035414ef7d) — Rohit Verma. Current market reality.
- [Prepping for Principal IC Interviews](https://www.linkedin.com/pulse/prepping-partnersenior-staffprincipal-ic-interviews-brett-flegg) — Brett Flegg. Practical prep framework.

---

## 6. JAVA DEEP DIVE (Netflix is Java-heavy)

### ★★★ Must-Read
- [Java Concurrency in Practice](https://jcip.net/) — Goetz. **THE Java concurrency book.** Key chapters:
  - Chapter 5: Building Blocks (ConcurrentHashMap, BlockingQueue)
  - Chapter 6: Task Execution (thread pools, CompletableFuture)
  - Chapter 8: Thread Pools (sizing, saturation policies)
- [Effective Java 3rd Edition](https://www.oreilly.com/library/view/effective-java/9780134686097/) — Bloch. Items to review:
  - Item 17: Minimize mutability
  - Item 50: Make defensive copies
  - Item 78-84: Concurrency items

### ★★ Deep Dive
- [JVM Internals](https://blog.jamesdbloom.com/JVMInternals.html) — How JVM works under the hood.
- [Java HashMap Internals](https://www.baeldung.com/java-hashmap-advanced) — Expect this in coding rounds.
- [CompletableFuture Guide](https://www.baeldung.com/java-completablefuture) — Async patterns in Java.

---

## 7. AI/ML FOR ENGINEERS (For Intuit AI Tool Interview)

### ★★ Deep Dive
- [RAG is Dead, Long Live RAG](https://www.rungalileo.io/blog/mastering-rag-how-to-architect-an-enterprise-rag-system) — Enterprise RAG architecture patterns.
- [Building LLM Applications for Production](https://huyenchip.com/2023/04/11/llm-engineering.html) — Chip Huyen. Practical LLM engineering.
- [AWS Bedrock Best Practices](https://docs.aws.amazon.com/bedrock/latest/userguide/best-practices.html) — Since you use Bedrock.
- [LangChain/LangGraph Documentation](https://python.langchain.com/docs/langgraph) — Agentic AI patterns.

---

## 8. COMPANY ENGINEERING BLOGS (Bookmark These)

| Company | Blog | Why |
|---------|------|-----|
| **Netflix** | [netflixtechblog.com](https://netflixtechblog.com) | **Your target company** |
| **Stripe** | [stripe.com/blog/engineering](https://stripe.com/blog/engineering) | Payment system design patterns |
| **Amazon** | [aws.amazon.com/builders-library](https://aws.amazon.com/builders-library) | Distributed systems best practices |
| **Uber** | [eng.uber.com](https://eng.uber.com) | Real-time systems, event-driven |
| **Airbnb** | [medium.com/airbnb-engineering](https://medium.com/airbnb-engineering) | Payment dedup, data infrastructure |
| **Google** | [research.google/blog](https://research.google/blog/) | Distributed systems research |
| **Meta** | [engineering.fb.com](https://engineering.fb.com) | Scale, caching, sharding |
| **LinkedIn** | [engineering.linkedin.com](https://engineering.linkedin.com) | Event streaming (Kafka origins) |
| **Cloudflare** | [blog.cloudflare.com](https://blog.cloudflare.com) | Edge computing, rate limiting |

---

## WEEKLY READING SCHEDULE

### Week 1 (Apply + Foundation)
| Day | Read | Time |
|-----|------|------|
| Mon | Stripe idempotency blog + Airbnb double payments | 45 min |
| Tue | Amazon Builders' Library: retries + caching | 45 min |
| Wed | Netflix Tech Blog: 3 most recent posts | 30 min |
| Thu | Hello Interview: level expectations | 20 min |

### Week 2 (Depth)
| Day | Read | Time |
|-----|------|------|
| Mon | DDIA Chapter 5 (Replication) | 1h |
| Tue | DDIA Chapter 6 (Partitioning) | 1h |
| Wed | Netflix Zuul + GraphQL Federation posts | 45 min |
| Thu | StaffEng.com: Interview guides | 30 min |

### Week 3 (Java + Practice)
| Day | Read | Time |
|-----|------|------|
| Mon | Java Concurrency Ch 5-6 (ConcurrentHashMap, thread pools) | 1h |
| Tue | Netflix Culture Deck + Chaos Monkey post | 30 min |
| Wed | System Design Primer: payment system section | 45 min |
| Thu | Pragmatic Engineer: latest newsletter | 20 min |

### Week 4 (Polish)
| Day | Read | Time |
|-----|------|------|
| Mon | Re-read Stripe idempotency + Amazon retry patterns | 30 min |
| Tue | ByteByteGo: latest 2 posts | 20 min |
| Wed | Netflix Tech Blog: any new posts | 20 min |
| Thu | Light review — skim bookmarks | 15 min |

---

*Last updated: 2026-04-09*
