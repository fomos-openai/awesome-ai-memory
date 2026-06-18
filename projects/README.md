# 20260618 Agent Memory Projects v1.0

This page curates open-source and closed/managed projects that are strongly related to agent memory. Rankings use [Agent Memory Scoring Standard v1.0](../score/README.md).

Review date: 2026-06-18.

## Project Taxonomy

| Code | Category | Description |
|---|---|---|
| P1 | Standalone memory layer | Dedicated memory product, SDK, server, or API |
| P2 | Temporal or graph memory | Knowledge graph, context graph, entity graph, or structured store |
| P3 | Agent framework memory | Memory module inside an agent framework |
| P4 | Research implementation | Code released with a paper or benchmark |
| P5 | Benchmark/eval infrastructure | Datasets, harnesses, leaderboards, or evaluation scripts |
| P6 | Managed/cloud memory | Hosted product or closed-source memory service |
| P7 | Storage substrate | Generic vector/RAG/database substrate used for memory |
| P8 | Governance and shared memory | Cross-agent memory, audit trails, permissions, privacy, fleet memory |

## Ranked Project Table

| Rank | Score | Project | Type | Taxonomy | Source type | Why it matters |
|---:|---:|---|---|---|---|---|
| 1 | 96 | [Mem0](https://github.com/mem0ai/mem0) | OSS plus managed platform | P1, P2, P6 | GitHub, arXiv | Universal memory layer for AI agents with user/session/agent state, benchmarks, SDKs, integrations, and cloud/self-hosted paths. |
| 2 | 95 | [Zep](https://github.com/getzep/zep) | Managed platform plus examples | P1, P2, P6 | GitHub, arXiv | Production context-graph infrastructure for agent memory; linked to temporal KG paper and Graphiti engine. |
| 3 | 94 | [Graphiti](https://github.com/getzep/graphiti) | Open-source temporal graph engine | P2 | GitHub, arXiv | Builds temporal context graphs with entity/fact validity, provenance, hybrid retrieval, and agent-specific graph updates. |
| 4 | 93 | [Letta](https://github.com/letta-ai/letta) | OSS plus managed platform | P1, P3, P6 | GitHub | Stateful-agent platform from the MemGPT lineage with advanced memory blocks, APIs, SDKs, and continual-learning focus. |
| 5 | 92 | [LangMem](https://github.com/langchain-ai/langmem) | OSS memory toolkit | P1, P3 | GitHub | Long-term memory primitives for agents, including memory tools, background memory manager, and LangGraph storage integration. |
| 6 | 91 | [Cognee](https://github.com/topoteretes/cognee) | OSS plus cloud memory platform | P1, P2, P6 | GitHub | AI memory platform with self-hosted knowledge graph, remember/recall/forget/improve operations, and agent integrations. |
| 7 | 90 | [CrewAI Memory](https://docs.crewai.com/en/concepts/memory) | Framework memory API | P3 | Official docs, GitHub | Unified Memory class with LLM-assisted extraction, hierarchical scopes, composite scoring, and crew/agent/flow integration. |
| 8 | 89 | [AutoGen Memory and RAG](https://microsoft.github.io/autogen/stable/user-guide/agentchat-user-guide/memory.html) | Framework memory protocol | P3, P7 | Official docs, GitHub | Memory protocol with add/query/update_context/clear/close and Chroma-backed RAG agent examples. |
| 9 | 88 | [LangGraph](https://github.com/langchain-ai/langgraph) | Agent framework/platform | P3 | GitHub, official docs | Provides durable stateful agents with short-term working memory and long-term persistent memory through LangGraph storage. |
| 10 | 86 | [Memobase](https://github.com/memodb-io/memobase) | OSS long-term user memory | P1 | GitHub | User profile-based long-term memory for chatbot applications; useful for personalization and profile memory. |
| 11 | 85 | [Supermemory](https://github.com/supermemoryai/supermemory) | OSS plus API/app | P1, P6 | GitHub | Memory and context engine/API for fast, scalable, local-capable AI-era memory. |
| 12 | 84 | [Memary](https://github.com/kingjulio8238/Memary) | OSS autonomous-agent memory layer | P1, P4 | GitHub | Early open-source memory layer targeted directly at autonomous agents. |
| 13 | 84 | [OpenMemory](https://github.com/mem0ai/mem0/tree/main/openmemory) | OSS app/server in Mem0 ecosystem | P1, P6 | GitHub | Practical memory app surface for using Mem0-style memory across assistants and applications. |
| 14 | 83 | [A-Mem](https://github.com/agiresearch/A-mem) | Research implementation | P4 | GitHub, arXiv | Implements agentic memory with structured notes, dynamic links, and evolving memory networks. |
| 15 | 82 | [LlamaIndex](https://github.com/run-llama/llama_index) | Data/agent framework | P3, P7 | GitHub | Strong agent-data framework with persistence, indexing, chat memory patterns, and memory substrate integrations. |
| 16 | 80 | [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | Framework memory connectors | P3, P7 | GitHub | Enterprise-friendly semantic memory and connector patterns for agent-like applications. |
| 17 | 79 | [MemGPT](https://github.com/cpacker/MemGPT) | Original OSS project lineage | P1, P4 | GitHub, arXiv | Historical implementation of virtual context management; superseded in practice by Letta but still important. |
| 18 | 78 | [MemoryBank](https://github.com/zhongwanjun/MemoryBank-SiliconFriend) | Research implementation | P4 | GitHub, arXiv | Companion-oriented long-term memory code lineage with updating and forgetting-curve ideas. |
| 19 | 77 | [Voyager](https://github.com/MineDojo/Voyager) | Research implementation | P4 | GitHub, arXiv | Embodied lifelong-learning agent with an expandable executable skill library. |
| 20 | 76 | [Reflexion](https://github.com/noahshinn/reflexion) | Research implementation | P4 | GitHub, arXiv | Verbal reinforcement and reflection memory for task improvement across trials. |
| 21 | 76 | [ExpeL](https://github.com/LeapLabTHU/ExpeL) | Research implementation | P4 | GitHub, arXiv | Experiential-learning agent code path for accumulating and recalling task insights. |
| 22 | 75 | [GITM](https://github.com/OpenGVLab/GITM) | Research implementation | P4 | GitHub, arXiv | Open-world Minecraft agent using text-based knowledge and memory. |
| 23 | 75 | [JARVIS-1](https://craftjarvis.org/JARVIS-1) | Research project | P4 | Project page, arXiv | Memory-augmented multimodal Minecraft agent for open-world multi-task behavior. |
| 24 | 74 | [Hindsight](https://arxiv.org/abs/2512.12818) | Research/system proposal | P4, P5 | arXiv | Structured retain/recall/reflect architecture; included as a high-signal research system even if project maturity is less public. |
| 25 | 73 | [ChatDev](https://github.com/OpenBMB/ChatDev) | Multi-agent software framework | P4, P8 | GitHub, arXiv | Boundary project with software-agent collaboration and historical memory relevance. |
| 26 | 72 | [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT) | Agent framework | P3, P7 | GitHub | Important legacy agent framework with memory backends, but memory is not the primary contribution. |
| 27 | 72 | [BabyAGI](https://github.com/yoheinakajima/babyagi) | Legacy task agent | P3, P7 | GitHub | Early task-loop memory pattern; useful historical context, not a modern memory layer. |
| 28 | 71 | [Haystack](https://github.com/deepset-ai/haystack) | RAG/agent framework | P3, P7 | GitHub | Strong retrieval substrate for agents, but agent memory is a derived use case. |
| 29 | 70 | [Chroma](https://github.com/chroma-core/chroma) | Vector database | P7 | GitHub | Common memory substrate; included only as supporting infrastructure, not an agent-memory system. |
| 30 | 70 | [Qdrant](https://github.com/qdrant/qdrant) | Vector database | P7 | GitHub | Common persistent vector substrate for memory retrieval; not agent-specific. |

## Managed and Closed Components

Some projects combine open-source code with managed products. The score reflects public technical detail, not private vendor claims.

| Project | Public surface | Closed/managed surface | Notes |
|---|---|---|---|
| Mem0 | OSS library, server, evaluation, SDKs | Hosted Mem0 Platform | Strongest public benchmark and integration story among standalone memory layers. |
| Zep | Public examples, legacy repo, Graphiti OSS core | Managed Zep context graph platform | Production system is primarily managed; Graphiti provides inspectable core concepts. |
| Letta | OSS repo and APIs | Hosted Letta endpoint/platform | Current continuation of MemGPT-style stateful agents. |
| Cognee | OSS memory platform | Cognee Cloud | Strong local/cloud split with graph memory and agent hooks. |
| Supermemory | OSS repo | Hosted API/app | Promising memory API direction; lower score until more agent-specific benchmarks are public. |

## Taxonomy Inverted Index by Weight

| Taxonomy | Highest-weight projects |
|---|---|
| P1 Standalone memory layer | Mem0 (96); Zep (95); Letta (93); LangMem (92); Cognee (91); Memobase (86); Supermemory (85); Memary (84) |
| P2 Temporal or graph memory | Zep (95); Graphiti (94); Cognee (91); Mem0 Graph Memory (96 as part of Mem0) |
| P3 Agent framework memory | CrewAI Memory (90); AutoGen Memory (89); LangGraph (88); LlamaIndex (82); Semantic Kernel (80) |
| P4 Research implementation | A-Mem (83); MemGPT (79); MemoryBank (78); Voyager (77); Reflexion (76); ExpeL (76); GITM (75); JARVIS-1 (75) |
| P5 Benchmark/eval infrastructure | Hindsight (74); benchmark repositories associated with LongMemEval, MemoryAgentBench, EvoMemBench, MemGym, and GroupMemBench |
| P6 Managed/cloud memory | Mem0 (96); Zep (95); Letta (93); Cognee (91); Supermemory (85) |
| P7 Storage substrate | LlamaIndex (82); Semantic Kernel (80); Haystack (71); Chroma (70); Qdrant (70) |
| P8 Governance and shared memory | Zep (95); Graphiti (94); Cognee (91); ChatDev (73 as boundary); emerging shared-memory projects tracked through awesome-agents |

## Deduplication and Aliases

- **MemGPT -> Letta:** Keep both because MemGPT is the foundational paper/project lineage and Letta is the current platform.
- **Zep -> Graphiti:** Keep both because Zep is a managed production platform and Graphiti is an open-source temporal graph engine.
- **Mem0 -> OpenMemory:** Keep OpenMemory as a subproject entry only when the user needs an app/server surface; otherwise score Mem0 as the main project.
- **Framework memory vs standalone memory:** LangGraph, CrewAI, AutoGen, LlamaIndex, and Semantic Kernel are scored lower than dedicated memory layers unless memory is the specific comparison target.
- **Vector databases:** Chroma and Qdrant are not agent-memory projects; they are included only as common substrates.

## Watchlist

Track but do not promote until stronger public evidence appears:

- New research code for MemFactory, Memory-R1, HiMPO, InfMem, Infini Memory, and Agent Memory Characterization.
- Emerging shared-memory projects listed in [kyrolabs/awesome-agents](https://github.com/kyrolabs/awesome-agents), including governed, cross-agent, and local-first memory runtimes.
- Managed assistant-memory products from major AI vendors, included only when official agent-memory APIs or technical benchmarks are public.
