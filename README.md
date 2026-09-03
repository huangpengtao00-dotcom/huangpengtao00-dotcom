# Hi, I'm Opall Huang 👋

I work on **whether agent benchmarks can be trusted** — evaluation validity, the reliability of
LLM/VLM-as-judge, and the hidden preprocessing assumptions that live in evaluation code but never
make it into the paper. Alongside that, platform engineering on event-sourced agent runtimes.

我做的是 **agent 评测这一侧能不能信**：评测集的有效性、LLM/VLM 评估器的可靠性、
以及那些只存在于评测代码、却系统性改变公开数字的预处理假设。
偏好把系统做得可运行、可追踪、可验证，并明确工具与人工审核的边界。

## Selected projects / 代表项目

- [**judge-lab**](https://github.com/huangpengtao00-dotcom/judge-lab) —
  Evidence-grounded evaluation of visual reward models. First runnable result: the same
  histogram judge scores **ρ=0.99** under a self-referential pseudo-GT protocol but only
  **ρ=0.58** once the reference content differs — traditional metrics are propped up by the
  protocol, not by the signal. 48 tests, verifiable synthetic data, offline re-judging.
  / 视觉评估器的证据锚定评测:同一判据在伪 GT 协议下 0.99、真实设定下 0.58。

- [**weldcheck**](https://github.com/huangpengtao00-dotcom/weldcheck) —
  A published watertight ratio can depend more on one undocumented preprocessing switch
  than on the meshes being measured. STL round-trips move it **+62.5 pp** while
  topology-carrying formats do not budge, and a three-system leaderboard **fully
  reverses** — the soundest system ranks last under the evaluation script's own settings.
  Reproduces with no downloads; ships an AST auditor for finding the same inconsistency
  in any project.
  / 一个没人写进论文的预处理开关就能决定公开的几何指标,并让排行榜完全反转。

- [**openagent-harness**](https://github.com/huangpengtao00-dotcom/openagent-harness) ·
  [**platform backend**](https://github.com/huangpengtao00-dotcom/openagent-platform-backend) —
  A multi-model coding-agent evaluation stack: isolated workspaces, **patch + pytest acceptance
  gates**, a failure taxonomy (NoPatch / Unverified / Regression / ScopeViolation), and per-run
  cost accounting — with a FastAPI control plane for idempotent submission and run history.
  / coding agent 多模型评测执行器 + 控制面:双重验收门、失败类型学、逐 run 成本追踪。

- [**3d-agent-eval-research**](https://github.com/huangpengtao00-dotcom/3d-agent-eval-research) —
  Evidence-grounded evaluation for 3D-generation agents: immutable evidence bundles with
  integrity checksums, so every verdict points back to third-party re-auditable evidence.
  / 把「agent 变好了吗」做成可复现的测量:证据包不可变、判定可回溯。

- [**memfusion-memory**](https://github.com/huangpengtao00-dotcom/memfusion-memory) —
  Wiki-style memory for long-horizon agents: an explore sub-agent retrieves with read-only
  tools, and spawn/aggregate/stop traces carry reward labels for learning when to stop.
  / 长时程 agent 的 wiki 式记忆 + explore 子 agent;编排轨迹带 reward 标签。

- [**minimal-agent-loop**](https://github.com/huangpengtao00-dotcom/minimal-agent-loop) —
  A zero-dependency Python agent loop with tool boundaries, traces, retries, circuit breaking,
  and independent verification. Clone and run, no API key needed.
  / 零依赖、可测试的最小 Agent 闭环,克隆即跑。

- [**signal-pipeline**](https://github.com/huangpengtao00-dotcom/signal-pipeline) —
  A file-based public-signal pipeline: automated collection, templated pre-screening, and a
  human review gate as the only path to publication.
  / 自动采集、文件留痕、人工审核作为唯一发布关口的信号管道。

More notes and experiments: [opallagent.com](https://opallagent.com)
