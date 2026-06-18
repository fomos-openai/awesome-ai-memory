# Agent Memory Academic Papers v1.0

This page curates academic papers and GitHub paper-list repositories that are strongly related to agent memory. Rankings use [Agent Memory Scoring Standard v1.0](../score/README.md).

Review date: 2026-06-18.

## Inclusion Standard

Included papers must make memory central to an LLM agent, long-term assistant, benchmark, or agent-memory infrastructure. Adjacent agent papers are included only when they shaped memory practice or clarify taxonomy boundaries.

Deduplication rules:

- Keep the canonical paper once, even if it appears in multiple survey lists.
- Keep survey papers only when they add distinct taxonomy or field coverage.
- Keep benchmark papers separate from memory-system papers because they serve different research jobs.
- Keep project papers separate from their implementation repositories; repositories are listed in [projects/README.md](../projects/README.md).

## Taxonomy

| Code | Category |
|---|---|
| T1 | Surveys and theory |
| T2 | Persistent conversational memory |
| T3 | Agentic memory management |
| T4 | Reflective and experiential memory |
| T5 | Embodied and environment memory |
| T6 | Structured, graph, and database memory |
| T7 | Benchmarks and evaluation |
| T8 | Learned memory policies |
| T9 | Framework and production systems |
| T10 | Boundary/general-agent work |

## Ranked Paper Table

| Rank | Score | Year | Paper | Taxonomy | Source type | Why it matters |
|---:|---:|---:|---|---|---|---|
| 1 | 95 | 2026 | [Agent Memory: Characterization and System Implications of Stateful Long-Horizon Workloads](https://arxiv.org/abs/2606.06448) | T1, T7, T9 | arXiv | Systems-oriented taxonomy and profiling of representative memory systems across construction, retrieval, and generation costs. |
| 2 | 94 | 2025 | [A-MEM: Agentic Memory for LLM Agents](https://arxiv.org/abs/2502.12110) | T3, T6 | arXiv, GitHub | Introduces adaptive, Zettelkasten-like agentic memory with dynamic indexing, linking, and memory evolution. |
| 3 | 94 | 2025 | [Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory](https://arxiv.org/abs/2504.19413) | T2, T9 | arXiv, GitHub | Production-focused long-term conversational memory with reported accuracy, latency, and token-cost gains. |
| 4 | 93 | 2025 | [Zep: A Temporal Knowledge Graph Architecture for Agent Memory](https://arxiv.org/abs/2501.13956) | T6, T9 | arXiv | Establishes temporal knowledge graphs as a production-grade memory substrate for enterprise agents. |
| 5 | 92 | 2023 | [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560) | T3, T6, T9 | arXiv | Foundational virtual-context management paper; directly influenced Letta and later production memory layers. |
| 6 | 92 | 2026 | [LongMemEval-V2: Evaluating Long-Term Agent Memory Toward Experienced Colleagues](https://arxiv.org/abs/2605.12493) | T5, T7 | arXiv | Moves memory evaluation from user-history chat toward environment experience for web agents. |
| 7 | 91 | 2026 | [MemGym: a Long-Horizon Memory Environment for LLM Agents](https://arxiv.org/abs/2605.20833) | T5, T7 | arXiv | Unifies tool-use dialogue, deep research, coding, and computer-use tracks behind memory-isolated scoring. |
| 8 | 91 | 2023 | [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) | T2, T4, T5 | arXiv | Popularized memory streams, reflection, and retrieval for believable social agents. |
| 9 | 90 | 2024 | [LongMemEval: Benchmarking Chat Assistants on Long-Term Interactive Memory](https://arxiv.org/abs/2410.10813) | T2, T7 | arXiv | Core benchmark for extraction, multi-session reasoning, temporal reasoning, updates, and abstention. |
| 10 | 90 | 2025 | [Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions](https://arxiv.org/abs/2507.05257) | T2, T7 | arXiv | Defines MemoryAgentBench with retrieval, test-time learning, long-range understanding, and selective forgetting. |
| 11 | 89 | 2026 | [GroupMemBench: Benchmarking LLM Agent Memory in Multi-Party Conversations](https://arxiv.org/abs/2605.14498) | T2, T7 | arXiv | Targets group memory, speaker-grounded belief tracking, audience adaptation, and multi-party ambiguity. |
| 12 | 89 | 2026 | [EvoMemBench: Benchmarking Agent Memory from a Self-Evolving Perspective](https://arxiv.org/abs/2605.18421) | T4, T7 | arXiv | Benchmarks in-episode and cross-episode memory across knowledge-oriented and execution-oriented tasks. |
| 13 | 88 | 2025 | [Hindsight is 20/20: Building Agent Memory that Retains, Recalls, and Reflects](https://arxiv.org/abs/2512.12818) | T2, T4, T6 | arXiv | Proposes retain, recall, and reflect over structured memory networks for long-horizon conversations. |
| 14 | 88 | 2025 | [Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning](https://arxiv.org/abs/2508.19828) | T3, T8 | arXiv | Uses RL to train memory management and answer agents for add/update/delete/noop and retrieval decisions. |
| 15 | 87 | 2023 | [MemoryBank: Enhancing Large Language Models with Long-Term Memory](https://arxiv.org/abs/2305.10250) | T2 | arXiv | Early long-term user memory with updating, personality adaptation, and forgetting-curve inspiration. |
| 16 | 87 | 2026 | [Infini Memory: Maintainable Topic Documents for Long-Term LLM Agent Memory](https://arxiv.org/abs/2606.10677) | T3, T6 | arXiv | Treats memory as maintainable topic documents with staged updates and iterative retrieval. |
| 17 | 86 | 2024 | [A Survey on the Memory Mechanism of Large Language Model based Agents](https://arxiv.org/abs/2404.13501) | T1 | arXiv, GitHub, ACM TOIS | Strong survey baseline for memory source, form, operation, evaluation, and application taxonomy. |
| 18 | 86 | 2023 | [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) | T4 | arXiv | Foundational reflective episodic memory method for agents learning from task feedback without weight updates. |
| 19 | 85 | 2023 | [Voyager: An Open-Ended Embodied Agent with Large Language Models](https://arxiv.org/abs/2305.16291) | T4, T5 | arXiv, GitHub | Demonstrates lifelong embodied learning through an ever-growing executable skill library. |
| 20 | 85 | 2026 | [MemFactory: Unified Inference & Training Framework for Agent Memory](https://arxiv.org/abs/2603.29493) | T3, T8, T9 | arXiv | Modular framework for inference, training, and RL optimization of memory-augmented agents. |
| 21 | 84 | 2026 | [Evaluating Memory Structure in LLM Agents](https://arxiv.org/abs/2602.11243) | T6, T7 | arXiv | Tests whether agents can organize memory into task-appropriate structures, not just retrieve facts. |
| 22 | 84 | 2026 | [Is Agent Memory a Database? Rethinking Data Foundations for Long-Term AI Agent Memory](https://arxiv.org/abs/2605.26252) | T1, T6 | arXiv | Frames long-term agent memory as governed evolving state rather than record-level storage. |
| 23 | 83 | 2026 | [HiMPO: Hindsight-Informed Memory Policy Optimization for Less-Entangled Credit in Long-Horizon Agents](https://arxiv.org/abs/2606.16285) | T3, T8 | arXiv | Targets the credit-assignment problem for memory-writing actions in long-horizon agents. |
| 24 | 83 | 2026 | [InfMem: Learning System-2 Memory Control for Long-Context Agent](https://arxiv.org/abs/2602.02704) | T3, T8 | arXiv | Learns retrieval, writing, and stopping control for bounded memory over ultra-long documents. |
| 25 | 82 | 2023 | [ExpeL: LLM Agents Are Experiential Learners](https://arxiv.org/abs/2308.10144) | T4 | arXiv | Extracts reusable natural-language insights from training tasks and recalls them at inference. |
| 26 | 82 | 2023 | [JARVIS-1: Open-World Multi-task Agents with Memory-Augmented Multimodal Language Models](https://arxiv.org/abs/2311.05997) | T5 | arXiv | Adds multimodal memory for embodied Minecraft planning from actual survival experience. |
| 27 | 81 | 2025 | [Position: Episodic Memory is the Missing Piece for Long-Term LLM Agents](https://arxiv.org/abs/2502.06975) | T1, T4 | arXiv | Argues for explicit episodic-memory properties as a unifying roadmap for long-term agents. |
| 28 | 80 | 2023 | [Ghost in the Minecraft: Generally Capable Agents for Open-World Environments via LLMs with Text-based Knowledge and Memory](https://arxiv.org/abs/2305.17144) | T5 | arXiv, GitHub | Uses text knowledge and memory for open-world Minecraft agents and long-horizon task completion. |
| 29 | 78 | 2026 | [AutoAgent: Evolving Cognition and Elastic Memory Orchestration for Adaptive Agents](https://arxiv.org/abs/2603.09716) | T3, T4 | arXiv | Multi-agent framework with elastic memory orchestration and cognition evolution. |
| 30 | 77 | 2023 | [RET-LLM: Towards a General Read-Write Memory for Large Language Models](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T3, T6 | GitHub list, arXiv | Early read-write memory direction frequently cited in agent-memory paper lists. |
| 31 | 76 | 2023 | [Memory Sandbox: Transparent and Interactive Memory Management for Conversational Agents](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T2, T3 | GitHub list, arXiv | Focuses on transparent memory management for conversational agents. |
| 32 | 75 | 2023 | [ChatDB: Augmenting LLMs with Databases as Their Symbolic Memory](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T6 | GitHub list, arXiv | Representative symbolic/database memory direction for LLM systems. |
| 33 | 74 | 2023 | [AgentSims: An Open-Source Sandbox for Large Language Model Evaluation](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T5, T7 | GitHub list, arXiv | Sandbox evaluation environment where memory retrieval and simulation consistency matter. |
| 34 | 73 | 2023 | [RecurrentGPT: Interactive Generation of Arbitrarily Long Text](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T2, T10 | GitHub list, arXiv | Useful historical context for recurrent/summarizing memory, but less agent-specific. |
| 35 | 72 | 2023 | [Unleashing Infinite-Length Input Capacity for LLMs with Self-Controlled Memory System](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T3, T10 | GitHub list, arXiv | Boundary long-context memory method relevant to agent-memory mechanisms. |
| 36 | 72 | 2023 | [Communicative Agents for Software Development](https://github.com/WooooDyy/LLM-Agent-Paper-List#113-memory) | T4, T10 | GitHub list, arXiv | Software-agent work where memory is supporting rather than primary. |
| 37 | 70 | 2022 | [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) | T10 | arXiv | Boundary agent pattern; important for agent loops, but persistent memory is not the main contribution. |

## Curated GitHub Paper Lists

| Score | Repository | Scope | Source type | Notes |
|---:|---|---|---|---|
| 88 | [nuster1128/LLM_Agent_Memory_Survey](https://github.com/nuster1128/LLM_Agent_Memory_Survey) | Memory mechanism survey companion | GitHub, arXiv, ACM TOIS | Best targeted list for memory mechanisms, sources, forms, operations, evaluations, and applications. |
| 82 | [VoltAgent/awesome-ai-agent-papers](https://github.com/VoltAgent/awesome-ai-agent-papers) | 2026 AI agent papers | GitHub, arXiv | Useful weekly-style source for new 2026 memory and RAG agent papers. |
| 79 | [WooooDyy/LLM-Agent-Paper-List](https://github.com/WooooDyy/LLM-Agent-Paper-List) | Large LLM-agent survey paper list | GitHub | Broad historical list; memory subsection captures foundational 2023 work. |
| 74 | [kyrolabs/awesome-agents](https://github.com/kyrolabs/awesome-agents) | AI agent projects and tools | GitHub | Better for project discovery than academic filtering, but includes memory products and tools. |

## Taxonomy Inverted Index by Weight

Entries are sorted by score within each category.

| Taxonomy | Highest-weight entries |
|---|---|
| T1 Surveys and theory | Agent Memory Characterization (95); Survey on Memory Mechanism (86); Is Agent Memory a Database? (84); Position: Episodic Memory (81) |
| T2 Persistent conversational memory | Mem0 (94); Generative Agents (91); LongMemEval (90); GroupMemBench (89); Hindsight (88); MemoryBank (87) |
| T3 Agentic memory management | A-MEM (94); MemGPT (92); Memory-R1 (88); Infini Memory (87); HiMPO (83); InfMem (83) |
| T4 Reflective and experiential memory | Generative Agents (91); EvoMemBench (89); Reflexion (86); Voyager (85); ExpeL (82) |
| T5 Embodied and environment memory | LongMemEval-V2 (92); MemGym (91); Voyager (85); JARVIS-1 (82); GITM (80); AgentSims (74) |
| T6 Structured, graph, and database memory | A-MEM (94); Zep (93); MemGPT (92); Hindsight (88); Infini Memory (87); Evaluating Memory Structure (84) |
| T7 Benchmarks and evaluation | Agent Memory Characterization (95); LongMemEval-V2 (92); MemGym (91); LongMemEval (90); MemoryAgentBench (90); GroupMemBench (89); EvoMemBench (89) |
| T8 Learned memory policies | Memory-R1 (88); MemFactory (85); HiMPO (83); InfMem (83); MemAgent (tracked through MemFactory family) |
| T9 Framework and production systems | Agent Memory Characterization (95); Mem0 (94); Zep (93); MemGPT (92); MemFactory (85) |
| T10 Boundary/general-agent work | ReAct (70); ChatDev (72); RecurrentGPT (73); Self-Controlled Memory System (72) |

## Notes on Known Duplicates and Near-Duplicates

- **MemGPT and Letta:** MemGPT is the paper/original open-source lineage; Letta is the current platform/project lineage.
- **Zep and Graphiti:** Zep is the production memory platform; Graphiti is the open-source temporal graph engine that powers Zep-style context graphs.
- **Mem0 and OpenMemory:** Mem0 is the core memory layer; OpenMemory is a related app/server surface in the Mem0 repository.
- **LongMemEval and LongMemEval-V2:** V1 targets long-term interactive chat memory; V2 targets environment-specific web-agent experience.
- **Survey entries:** Broad LLM-agent surveys are not duplicated unless they add a memory-specific taxonomy.
