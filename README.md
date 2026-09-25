<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Opall Huang — agent systems, evaluation, geometry" src="assets/header-light.svg" width="100%">
</picture>

<br>

I build agent systems that hold up under measurement — evaluation readings that can be trusted,
money that moves exactly once, failures that surface instead of passing as empty results.

<sub>做能被验证的 agent 系统。读数可信，钱只动一次，出错就显式报出来。</sub>

<br>

### Work

**Meshy AI** &nbsp;·&nbsp; Agent team, software engineering intern &nbsp;·&nbsp; 2026.07 – 09<br>
<sub>311 merged pull requests across 6 production repositories · Go / TypeScript / Python · private</sub>

- **Geometry kernel for the 3D-printing agent.** Inspect → repair / shell → split with locating pegs →
  exact-boolean fit → plate arrangement. CPU-only; every command leaves a structured report the agent reads.
- **Agent evaluation.** Sole author of the verdict-reading layer: releases are compared on pass ↔ fail flips
  alone, so an infrastructure failure never reads as a model regression.
- **Production database.** A query on a 155M-row table from **462 s to 5.2 ms** — I/O-timing forensics, then
  a partial index, literal predicates and a keyset cursor. The same pattern later freed ~70 GB of indexes.
- **Money that moves once.** Idempotent payouts, exactly-once under eight-way concurrency without a
  distributed lock; quoted price equals charged price across three repositories.

**AI operations system** &nbsp;·&nbsp; a family-owned manufacturer &nbsp;·&nbsp; designed, shipped and run alone &nbsp;·&nbsp; 2026.06 –<br>
<sub>148k multilingual emails read · ~15k SKUs priced · 1,027-order deal ledger reconciled to the books at +0.0% · private</sub>

- Mail becomes reviewable work: classified, attributed to customers, quote leads extracted. AI drafts; the
  system never sends mail on its own.
- Built with a fleet of coding agents working inside the architecture, acceptance criteria and merge gates I set.

<br>

### Open source

- [**weldcheck**](https://github.com/huangpengtao00-dotcom/weldcheck) &nbsp;—&nbsp; One undocumented preprocessing switch moves a published watertight ratio by +62.5 pp and reverses a three-system leaderboard.
- [**openagent-harness**](https://github.com/huangpengtao00-dotcom/openagent-harness) &nbsp;—&nbsp; Multi-model coding-agent evaluation: isolated workspaces, patch + pytest gates, a failure taxonomy, per-run cost. [Control plane →](https://github.com/huangpengtao00-dotcom/openagent-platform-backend)
- [**restore-rsi**](https://github.com/huangpengtao00-dotcom/restore-rsi) &nbsp;—&nbsp; A self-improving loop that measures its own gate — a coin flip — and loses to a ten-line baseline.
- [**memfusion-memory**](https://github.com/huangpengtao00-dotcom/memfusion-memory) &nbsp;—&nbsp; Wiki-style agent memory, BM25 + dense hybrid retrieval. First of 50 on one dimension of the Agent Memory Leaderboard.
- [**judge-lab**](https://github.com/huangpengtao00-dotcom/judge-lab) &nbsp;—&nbsp; The same judge: ρ 0.99 under a pseudo-ground-truth protocol, 0.58 in the real setting.
- [**minimal-agent-loop**](https://github.com/huangpengtao00-dotcom/minimal-agent-loop) &nbsp;—&nbsp; A zero-dependency agent loop with tool boundaries, traces, retries and a circuit breaker.

<br>

<sub>Go · TypeScript · Python · PostgreSQL · Redis / Valkey · FastAPI · React · Kubernetes · trimesh · manifold3d</sub><br>
<sub>Xiamen University, Computer Science · [opallagent.com](https://opallagent.com) · huangpengtao00@gmail.com</sub>
