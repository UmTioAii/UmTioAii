# Daniel Anastácio · UmTioAii

Software engineer building systems around AI agents. My current work is ASTRO, a multi-agent coding harness where every model call is routed by configuration, metered, and recorded in an append-only audit trail. I'm interested in how to make LLM-driven tooling reliable enough to trust: deterministic routing, least-privilege tools, cost governance, and evaluation gates.

🔗 [Portfolio](https://umtioaii.netlify.app/) ·  · [Email](mailto:09someone29@gmail.com)

---

## 🧭 ASTRO

**A local, terminal-first harness for AI coding agents**, built with Bun and TypeScript.

A request becomes a session that plans, reads, writes and executes inside a declared scope. Multiple named agents, each bound to a model or profile, pass work to each other through durable handoffs.

**Design principles:** determinism over flexibility · security as a contract · every action auditable · extend, don't recreate.

- **The config chooses the model, never the LLM.** Every completion is recorded with its agent, real provider, model, tokens and cost.
- **Cost governance:** usage is attributed per agent, profile and provider, and checked before each call.
- **Durable handoffs** with acknowledgement, compare-and-swap and idempotency by handoff ID.
- **Least privilege:** each agent has its own tool allowlist. Denied calls are audited.
- **Provider fallback** by priority, retrying only transient errors.
- **Secrets only from the environment**, redacted from logs, audit records and errors.
- **Invariants mapped to code and tests** (I-01 to I-22), with a golden-dataset evaluation gate.

**Status:** Phases F0–F7 are complete. Layer 0 (durable handoffs, model pools and profiles, per-agent cost, provider fallback) is in progress. The next layers add skills, MCP support, web tools, a richer TUI and session management. Open issues are tracked on GitHub.

```bash
npm install -g @umtioai/astro-harness@alpha
astro
```

📦 [github.com/UmTioAii/ASTRO](https://github.com/UmTioAii/ASTRO) · MIT License

### 🤝 Contributing

ASTRO is in active development and contributions are welcome. Start with [CONTRIBUTING.md](https://github.com/UmTioAii/ASTRO/blob/main/CONTRIBUTING.md) and [docs/workflow.md](https://github.com/UmTioAii/ASTRO/blob/main/docs/workflow.md). The process is one issue per change, a branch per item, and a pull request with review. Good places to start are the planned layers in [docs/roadmap-complementar.md](https://github.com/UmTioAii/ASTRO/blob/main/docs/roadmap-complementar.md) and the open issues on the repo.

---

## ⚙️ Languages & Stack

**Languages:** TypeScript (primary), JavaScript, Python, SQL
**Runtime & tooling:** Bun, Node.js 18+, Ink (terminal UI), Git and GitHub
**AI & agents:** OpenAI-compatible APIs (NVIDIA NIM, OpenRouter), Codex OAuth, multi-model routing, durable handoffs, golden-dataset evaluation
**Observability:** OpenTelemetry tracing, Prometheus metrics, append-only JSONL ledger and audit logs
**Quality & delivery:** Bun test, type checking, secret scanning, CI workflows, ADRs and written invariants

---

## 🛠️ Other work

**[Bud-Budget](https://github.com/UmTioAii/Bud-Budget)**: personal finance app for tracking income and expenses. [Demo](https://bud-budget.vercel.app)
**[Memo-RY](https://github.com/UmTioAii/Memo-RY)**: responsive memory game in TypeScript. [Demo](https://memo-ry.vercel.app)

---

## 📫 Let's talk

I'm happy to discuss agent architecture, developer tooling, and reliable AI systems. Feedback and contributions to ASTRO are always welcome.

· [Email](mailto:09someone29@gmail.com)
