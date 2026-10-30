# Daniel Anastácio

Software engineer focused on systems, data and AI agents. I build tools that have to be reliable in production: explicit architecture decisions, cost control, traceability, and tests that protect the behavior of the system.

I'm currently building **ASTRO**, a multi-agent harness for AI-assisted development, and I work on operational planning and systems integration for a solar energy company.

🔗 [Portfolio](https://umtioaii.netlify.app/) · [LinkedIn](https://linkedin.com/in/SEU-PERFIL) · [Email](mailto:09someone29@gmail.com)

---

## What I do

- **Systems and backend:** domain modeling, integrations between teams, APIs and persistence with PostgreSQL and SQL Server.
- **AI agents:** model routing, handoffs between agents, cost control and per-tool permissions.
- **Data and automation:** pipelines and reports in Python, operational spreadsheet transformation and department-specific views.
- **Engineering quality:** automated tests, ADRs, documented invariants and release gates.

---

## Featured project: ASTRO
 
A local, terminal-first harness for AI coding agents, built with Bun and TypeScript.
 
Instead of letting the model decide what to do, the configuration defines which model runs each step. Every call is metered, every action goes into an audit trail, and each agent can only use the tools it was given.
 
- Deterministic routing across providers (NVIDIA NIM, OpenRouter, Codex) with fallback.
- Durable handoffs between agents, with idempotency and concurrency control.
- Cost governance per agent, profile and provider.
- Golden dataset as a continuous evaluation gate.
 
**Try it:**
 
```bash
npm install -g @umtioai/astro-harness@alpha
astro
```
 
📦 [github.com/UmTioAii/ASTRO](https://github.com/UmTioAii/ASTRO) · MIT · contributions are welcome
 
---
 
## Other projects
 
- **[Bud-Budget](https://github.com/UmTioAii/Bud-Budget)**: personal finance app for tracking income and expenses. [Demo](https://bud-budget.vercel.app)
- **[Memo-RY](https://github.com/UmTioAii/Memo-RY)**: responsive memory game in TypeScript. [Demo](https://memo-ry.vercel.app)
---
 
## Stack
 
| Area | Tools |
|---|---|
| Languages | TypeScript, Python, JavaScript, SQL |
| Backend and data | PostgreSQL, SQL Server, Supabase, Node.js, Bun |
| AI and agents | Multi-model routing, OpenAI-compatible APIs, MCP, golden-dataset evaluation |
| Quality and delivery | Automated tests, type checking, CI, Git and GitHub, ADRs |
 
---
 
## How I work
 
I document architecture decisions as ADRs, review changes through pull requests and write down the invariants the code must respect. I prefer systems that explain themselves over systems that depend on the memory of whoever built them.
 
---
 
## Contact
 
Open to conversations about software engineering, AI agent architecture, and backend, platform or systems roles.

---
[LinkedIn](https://linkedin.com/in/SEU-PERFIL) · [Email](mailto:09someone29@gmail.com)
