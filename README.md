### Hi, I'm Artur.

I'm a Go backend developer focused on distributed systems and developer tooling.

Most of my day is `Go` — services, libraries, and the occasional CLI. Comfortable area:
- Backend microservices with **gRPC**, **PostgreSQL**, **Redis**, **Kafka**, **RabbitMQ**
- Observability built on **OpenTelemetry** + **Prometheus** + **Grafana** + **Jaeger**
- Infrastructure with **Docker**, **Kubernetes**, **Helm**, **GitLab CI**
- Production reliability: graceful shutdown, idempotency keys, retries with jitter, circuit breakers, transactional outbox

### Currently building

**[Sundial](https://github.com/goncharovart/sundial)** — durable distributed cron scheduler for Go.
Postgres advisory locks for leader election, OpenTelemetry-instrumented, missed-fire recovery (Skip / RunOnce / RunAll iterator), exponential-backoff retry with jitter, dead-letter on exhaust. The case it solves: cron semantics + Postgres durability that scales beyond a single node, without bringing in Redis, Kafka, or Temporal. **v0.1.0 released**.

**[runlet](https://github.com/goncharovart/runlet)** — single-binary runner for Go scripts with inline dependencies. Like `uv run` for Python or `cargo script` for Rust, but for Go. Magic-comment dep declarations, content-addressed cache, shebang-friendly. Closes a documented gap in the Go ecosystem.

**[tinylink](https://github.com/goncharovart/tinylink)** — URL shortener documented as a five-stage `pprof`-driven optimization walkthrough. Every stage is a separate commit with a reproducible k6 benchmark; the bonus stage-5 monotonic allocator runs 22× faster than the baseline random+retry path (per included `go test -bench`).

**[goeval](https://github.com/goncharovart/goeval)** — RAGAS for Go. Pre-MVP scaffold of a Go-native RAG evaluation library: streaming `dataset → evaluator → result` pipeline, LLM-as-judge abstraction, deterministic metrics for CI gates. Python owns this space; Go teams currently shell out to Python or reinvent metrics. Roadmap to v0.1.0: 6 weeks of evening dev.

### Sharpening

- Go runtime internals — GC, escape analysis, `pprof` deep dive
- Distributed systems patterns — Raft alternatives via Postgres advisory locks, saga, transactional outbox
- System design at middle / senior backend level

📫 **Reach out:** [@gonartur](https://t.me/gonartur) · goncharov.artur.02@gmail.com

---

<sub>Open to middle Go backend roles. EN & RU. Project READMEs are EN by default; happy to switch.</sub>
