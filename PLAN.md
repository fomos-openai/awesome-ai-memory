# 20260618 Agent Memory Update Plan v1.0

This plan defines a repeatable update process for keeping this repository current.

## Update Cadence

| Cadence | Task | Output |
|---|---|---|
| Daily lightweight scan | Check arXiv and GitHub for new high-signal "agent memory" entries. | Short candidate list or no-op. |
| Weekly curation | Score new papers/projects, deduplicate, update tables, and note rejected boundary items. | Pull request or commit with scored entries. |
| Monthly audit | Re-score top 30 papers and projects for changed evidence, code releases, benchmarks, and maintenance status. | Score delta notes in relevant README files. |
| Quarterly taxonomy review | Revisit categories, weighting, and source confidence rules. | New scoring standard version if needed. |

## Daily Search Queries

Use these exact query families across arXiv, Google Scholar, Semantic Scholar, GitHub, and web search:

- `"agent memory" "LLM agents"`
- `"long-term memory" "LLM agents"`
- `"agentic memory" "LLM"`
- `"memory agents" benchmark`
- `"persistent memory" "AI agents"`
- `"temporal knowledge graph" "agent memory"`
- `"episodic memory" "LLM agents"`
- `"selective forgetting" "LLM agents"`
- `"memory management" "LLM agents" reinforcement learning`
- `"LongMemEval" OR "MemoryAgentBench" OR "MemGym" OR "GroupMemBench" OR "EvoMemBench"`

## High-Priority Academic Sources

| Source | URL | Why monitor |
|---|---|---|
| arXiv cs.AI | https://arxiv.org/list/cs.AI/recent | Fastest source for new agent-memory preprints. |
| arXiv cs.CL | https://arxiv.org/list/cs.CL/recent | Conversational memory, evaluation, and language-agent work. |
| arXiv cs.LG | https://arxiv.org/list/cs.LG/recent | Learned memory policies and RL-trained memory agents. |
| ACL Anthology | https://aclanthology.org/ | Peer-reviewed NLP memory and agent papers. |
| ACM Digital Library | https://dl.acm.org/ | HCI, systems, and TOIS versions of memory-agent work. |
| OpenReview | https://openreview.net/ | ICLR, NeurIPS, ICML workshop and conference submissions. |
| Papers With Code | https://paperswithcode.com/ | Code, datasets, and benchmark tracking. |
| Semantic Scholar | https://www.semanticscholar.org/ | Citation trails and related-work expansion. |

## High-Priority GitHub and List Sources

| Source | URL | Why monitor |
|---|---|---|
| LLM Agent Memory Survey | https://github.com/nuster1128/LLM_Agent_Memory_Survey | Targeted memory mechanism survey companion repo. |
| VoltAgent awesome AI agent papers | https://github.com/VoltAgent/awesome-ai-agent-papers | Weekly-style 2026 agent paper discovery, including memory and RAG. |
| WooooDyy LLM Agent Paper List | https://github.com/WooooDyy/LLM-Agent-Paper-List | Broad historical agent-paper source with memory subsection. |
| kyrolabs awesome-agents | https://github.com/kyrolabs/awesome-agents | Project discovery, especially emerging memory runtimes. |
| GitHub topic search | https://github.com/search?q=agent+memory&type=repositories | Finds new projects before papers appear. |
| GitHub code search | https://github.com/search?q=%22long-term+memory%22+%22agent%22&type=repositories | Finds framework integrations and implementation examples. |

## High-Priority Project Sources

| Project | URL | Monitor for |
|---|---|---|
| Mem0 | https://github.com/mem0ai/mem0 | Benchmark updates, OpenMemory, SDK changes, server/platform changes. |
| Zep | https://github.com/getzep/zep | Platform updates, Graphiti references, enterprise memory APIs. |
| Graphiti | https://github.com/getzep/graphiti | Temporal graph features, ontology support, retrieval changes, MCP server. |
| Letta | https://github.com/letta-ai/letta | Memory block APIs, self-improvement features, cloud/local split. |
| LangMem | https://github.com/langchain-ai/langmem | LangGraph integration, memory manager changes, prompt optimization. |
| LangGraph | https://github.com/langchain-ai/langgraph | Persistent memory store and stateful-agent capabilities. |
| CrewAI Memory | https://docs.crewai.com/en/concepts/memory | Unified memory API, scopes, composite scoring, consolidation. |
| AutoGen Memory | https://microsoft.github.io/autogen/stable/user-guide/agentchat-user-guide/memory.html | Memory protocol and vector memory integrations. |
| Cognee | https://github.com/topoteretes/cognee | Knowledge-graph memory, agent hooks, cloud/local memory changes. |
| LlamaIndex | https://github.com/run-llama/llama_index | Chat memory, agent memory, persistence, indexing APIs. |
| Semantic Kernel | https://github.com/microsoft/semantic-kernel | Enterprise semantic memory and connector changes. |
| Supermemory | https://github.com/supermemoryai/supermemory | Memory API maturity and agent-specific features. |
| Memobase | https://github.com/memodb-io/memobase | User-profile memory and chatbot memory evidence. |
| Memary | https://github.com/kingjulio8238/Memary | Autonomous-agent memory maintenance status. |

## Benchmark Watchlist

| Benchmark family | Current role |
|---|---|
| LongMemEval | Long-term interactive chat memory. |
| LongMemEval-V2 | Environment-specific web-agent experience memory. |
| MemoryAgentBench | Incremental multi-turn memory agents across retrieval, learning, long-range understanding, and forgetting. |
| GroupMemBench | Multi-party and speaker-grounded group memory. |
| EvoMemBench | Self-evolving memory over in-episode/cross-episode and knowledge/execution axes. |
| MemGym | Memory-isolated scoring across tool-use dialogue, deep research, coding, and computer-use regimes. |
| LOCOMO | Long-term conversational memory baseline family used by production memory papers. |
| Deep Memory Retrieval | Historical MemGPT/Zep-style memory retrieval benchmark. |

## Weekly Workflow

1. Pull the latest main branch.
2. Run source scans using the daily query list.
3. Add candidates to a scratch list with title, URL, source type, and one-sentence relevance.
4. Apply the inclusion gate from `score/README.md`.
5. Deduplicate against existing paper/project aliases.
6. Score each accepted entry using the correct paper or project rubric.
7. Insert entries into sorted tables.
8. Update taxonomy inverted indexes.
9. Update year quick lookup tables in `README.md`.
10. Run link and markdown checks.
11. Commit with a message such as `docs: update agent memory index YYYYMMDD`.

## Candidate Acceptance Checklist

- The source is primary or clearly marked as secondary.
- The entry has a stable URL.
- The memory mechanism is agent-relevant, not generic storage only.
- The taxonomy code is assigned.
- The score can be defended from the rubric.
- Duplicates and aliases are noted.
- Boundary items are not promoted above dedicated memory work.

## Rejection Reasons

Use these standard labels in future update notes:

- `generic-rag`: retrieval project without agent memory operations.
- `generic-vector-db`: storage substrate only.
- `long-context-only`: no external memory or agent memory flow.
- `agent-only`: agent framework with no meaningful persistent memory.
- `survey-duplicate`: survey does not add taxonomy or coverage.
- `marketing-only`: product claim lacks technical detail or public docs.
- `inactive`: project appears abandoned or unmaintained.

## Release Versioning

Use the naming pattern:

`YYYYMMDD <document name> v<major>.<minor>`

Examples:

- `20260618 Agent Memory Scoring Standard v1.0`
- `20260618 Agent Memory Academic Papers v1.0`
- `20260618 Agent Memory Projects v1.0`

Increment minor versions for source additions and score changes. Increment major versions when the taxonomy or scoring weights change.
