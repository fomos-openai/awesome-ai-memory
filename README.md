# Awesome AI Memory v1.0

A curated research index for **Agent Memory**: persistent, structured, retrievable, updateable, and governable memory systems for LLM-based agents.

This repository tracks academic papers, benchmarks, GitHub collections, open-source projects, and production-oriented memory platforms that are directly relevant to long-horizon AI agents. It is intentionally narrower than a general RAG or vector database list: an entry should help an agent remember, revise, retrieve, reflect, or act from accumulated experience across turns, tasks, sessions, users, environments, or agent fleets.

## Contents

- [Agent Memory Scoring Standard v1.0](score/README.md)
- [Agent Memory Academic Papers v1.0](papers/README.md)
- [Agent Memory Projects v1.0](projects/README.md)
- [Agent Memory Update Plan v1.0](PLAN.md)

## Classification Model

The taxonomy uses two linked views:

- **Mechanism view:** what the memory system does: write, manage, retrieve, reflect, forget, evaluate, or govern.
- **Substrate view:** how the memory is represented: prompt/context, vector store, episodic log, structured notes, temporal graph, symbolic database, learned policy, or benchmark harness.

Primary categories used throughout the repository:

| Code | Category | Scope |
|---|---|---|
| T1 | Surveys and theory | Taxonomies, definitions, system implications, position papers |
| T2 | Persistent conversational memory | User/session/assistant memory across long interactions |
| T3 | Agentic memory management | Agent-controlled write/update/delete/retrieve policies |
| T4 | Reflective and experiential memory | Self-reflection, trial learning, lessons, reusable experience |
| T5 | Embodied and environment memory | Minecraft, web, game, computer-use, and environment-specific memory |
| T6 | Structured, graph, and database memory | Temporal KGs, symbolic stores, topic documents, governed states |
| T7 | Benchmarks and evaluation | Long-term memory and agent-memory benchmarks |
| T8 | Learned memory policies | RL/SFT-trained memory managers and compression controllers |
| T9 | Framework and production systems | Open-source and commercial memory layers |
| T10 | Boundary/general-agent work | Important adjacent agent systems where memory is secondary |

## Scoring Model

All rankings use **Agent Memory Scoring Standard v1.0**. Scores are out of 100 and are weighted differently for papers and projects.

- Papers emphasize agent-memory relevance, novelty, evaluation strength, artifact quality, and reproducibility.
- Projects emphasize memory fit, functional completeness, engineering maturity, integrations, adoption, evaluation evidence, and governance.
- Scores are research triage signals, not claims of absolute scientific truth.

See [score/README.md](score/README.md) for the full rubric, inclusion gates, source confidence levels, and re-scoring policy.

## High-Weight Paper Snapshot

| Score | Year | Paper | Category | Source |
|---:|---:|---|---|---|
| 95 | 2026 | [Agent Memory: Characterization and System Implications of Stateful Long-Horizon Workloads](https://arxiv.org/abs/2606.06448) | T1, T7, T9 | arXiv |
| 94 | 2025 | [A-MEM: Agentic Memory for LLM Agents](https://arxiv.org/abs/2502.12110) | T3, T6 | arXiv, GitHub |
| 94 | 2025 | [Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory](https://arxiv.org/abs/2504.19413) | T2, T9 | arXiv, GitHub |
| 93 | 2025 | [Zep: A Temporal Knowledge Graph Architecture for Agent Memory](https://arxiv.org/abs/2501.13956) | T6, T9 | arXiv |
| 92 | 2023 | [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560) | T3, T6, T9 | arXiv |
| 92 | 2026 | [LongMemEval-V2: Evaluating Long-Term Agent Memory Toward Experienced Colleagues](https://arxiv.org/abs/2605.12493) | T5, T7 | arXiv |

Full paper table: [papers/README.md](papers/README.md).

## High-Weight Project Snapshot

| Score | Project | Type | Category | Source |
|---:|---|---|---|---|
| 96 | [Mem0](https://github.com/mem0ai/mem0) | OSS plus managed platform | P1, P2 | GitHub, arXiv |
| 95 | [Zep](https://github.com/getzep/zep) | Managed platform plus examples | P1, P2 | GitHub, arXiv |
| 94 | [Graphiti](https://github.com/getzep/graphiti) | OSS temporal graph engine | P2 | GitHub |
| 93 | [Letta](https://github.com/letta-ai/letta) | OSS plus managed platform | P1, P3 | GitHub |
| 92 | [LangMem](https://github.com/langchain-ai/langmem) | OSS agent memory toolkit | P1, P3 | GitHub |
| 91 | [Cognee](https://github.com/topoteretes/cognee) | OSS plus cloud memory platform | P1, P2 | GitHub |

Full project table: [projects/README.md](projects/README.md).

## Year Quick Lookup: Academic Papers

| Year | High-signal entries |
|---:|---|
| 2026 | Agent Memory Characterization; LongMemEval-V2; MemGym; GroupMemBench; EvoMemBench; Infini Memory; MemFactory; InfMem; Evaluating Memory Structure; Is Agent Memory a Database |
| 2025 | A-MEM; Mem0; Zep; MemoryAgentBench; Memory-R1; MemAgent; Position on Episodic Memory; Hindsight; LOCOMO-family long-term memory work |
| 2024 | Survey on Memory Mechanism of LLM-based Agents; LongMemEval; broader autonomous-agent surveys with memory taxonomies |
| 2023 | Generative Agents; Reflexion; MemoryBank; Voyager; GITM; ExpeL; MemGPT; JARVIS-1; Memory Sandbox; RET-LLM; ChatDB |
| 2022 | ReAct and early agent patterns, included only as boundary context where memory is not the main contribution |

## Year Quick Lookup: Open-Source Projects

| Year / Era | Project families |
|---|---|
| 2026-current | Mem0, Zep, Graphiti, Letta, LangMem, Cognee, CrewAI Memory, AutoGen Memory, OpenMemory, Supermemory, Memobase |
| 2025 | A-Mem, Memory-R1, MemFactory, Hindsight-style research implementations, emerging benchmark harnesses |
| 2024 | LangGraph long-term memory, agent framework memory APIs, productionized MemGPT/Letta transition |
| 2023 | MemGPT, Generative Agents, Voyager, Reflexion, MemoryBank, GITM, ExpeL, JARVIS-1 |
| Legacy / adjacent | BabyAGI task memory, AutoGPT memory backends, vector databases and RAG frameworks used as substrates rather than agent-memory systems |

## Source Policy

Each curated item records a source type:

- **arXiv / ACL / ACM / OpenReview:** academic paper source.
- **GitHub:** implementation, project page, or curated list.
- **Official docs:** vendor or framework documentation.
- **Industry blog / news:** deployment claims, product updates, or market signal.
- **Benchmark:** benchmark paper, benchmark repository, or leaderboard.

## Maintenance

Follow [PLAN.md](PLAN.md) for weekly and monthly update jobs. The repository should be refreshed whenever a new agent-memory benchmark, production memory layer, major framework API, or high-citation survey appears.
