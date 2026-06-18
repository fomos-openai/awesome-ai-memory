# 20260618 Agent Memory Scoring Standard v1.0

This document defines **Agent Memory Scoring Standard v1.0**, a practical weighting model for evaluating academic papers and industry projects related to agent memory.

The goal is not to produce a universal truth score. The goal is to make curation decisions explicit, reproducible, and easy to revise as the field changes.

## Scope

An item is in scope when memory is a first-class part of an LLM-based agent system. The memory component should support one or more of the following:

- Persistent recall across turns, sessions, users, tasks, environments, or agents.
- Write, update, delete, consolidate, summarize, reflect, or forget operations.
- Memory-aware planning, personalization, tool use, workflow adaptation, or agent self-improvement.
- Evaluation of long-term memory, agentic memory, temporal reasoning, update handling, or selective forgetting.
- Production infrastructure for agent memory: storage, retrieval, governance, observability, privacy, latency, cost, or fleet management.

Out of scope unless used as a substrate for an actual agent-memory system:

- Generic RAG libraries.
- Generic vector databases.
- Long-context model papers with no agent memory mechanism.
- Agent papers where "memory" means only the current prompt or scratchpad.
- Product claims with no technical detail, documentation, benchmark, or reproducible artifact.

## Source Confidence

| Confidence | Evidence pattern | Use in scoring |
|---|---|---|
| A | Peer-reviewed paper, arXiv paper with detailed experiments, official benchmark, or active GitHub repository with docs | Eligible for high scores |
| B | Official product docs, official blog, technical report, or well-maintained curated GitHub list | Eligible for medium to high scores with caveats |
| C | Industry blog, news article, secondary list, README-only repository, or sparse public detail | Eligible for medium or low scores |
| D | Unverified marketing claim, inactive project, or unclear source | Mention only as watchlist unless strategically important |

## Academic Paper Rubric

Total: 100 points.

| Dimension | Weight | What earns high marks |
|---|---:|---|
| Agent-memory relevance | 25 | Memory is central to the agent architecture, not a side feature. |
| Technical novelty | 15 | Introduces a new mechanism, taxonomy, benchmark, policy, representation, or system characterization. |
| Evaluation strength | 15 | Uses relevant benchmarks, ablations, baselines, latency/cost analysis, or real agent tasks. |
| Mechanism clarity | 12 | Clearly defines memory write, manage, read, update, forget, or reflect flows. |
| Artifact and reproducibility | 10 | Provides code, data, benchmark, prompts, or enough details to reproduce. |
| Field influence | 8 | Cited by follow-on work, used by projects, or establishes a recurring vocabulary. |
| Production relevance | 7 | Addresses deployment constraints such as freshness, governance, latency, cost, privacy, or scale. |
| Timeliness | 5 | Current and relevant to the state of agent memory as of the review date. |
| Source confidence | 3 | Strong primary source and stable public access. |

### Paper Score Bands

| Score | Meaning |
|---:|---|
| 90-100 | Core reference. Read first. Strong direct relevance and durable value. |
| 80-89 | High-value paper. Important for a taxonomy branch or benchmark family. |
| 70-79 | Useful supporting paper. Include for coverage, history, or adjacent mechanisms. |
| 60-69 | Boundary item. Mention only if it clarifies exclusions or origins. |
| <60 | Exclude from the main table unless the update plan is tracking it. |

## Industry Project Rubric

Total: 100 points.

| Dimension | Weight | What earns high marks |
|---|---:|---|
| Agent-memory fit | 20 | The project is explicitly built for persistent agent memory. |
| Functional completeness | 15 | Supports write, retrieve, update/consolidate, delete/forget, metadata, and multi-session behavior. |
| Engineering maturity | 15 | Active repository, releases, tests, docs, deployment path, and stable APIs. |
| Integration surface | 12 | Works with agent frameworks, SDKs, MCP, cloud APIs, self-hosting, or multiple languages. |
| Adoption and ecosystem signal | 12 | Stars, forks, community, customer evidence, integrations, or known deployments. |
| Evaluation evidence | 10 | Benchmarks, papers, reproducible evals, latency/cost claims, or regression harnesses. |
| Governance and safety | 8 | Privacy, tenant isolation, provenance, auditability, deletion, access control, or compliance support. |
| Operability | 5 | Clear installation, observability, persistence backend, scaling, and recovery story. |
| Timeliness | 3 | Maintained or newly relevant as of the review date. |

### Project Score Bands

| Score | Meaning |
|---:|---|
| 90-100 | Primary project. Strong candidate for implementation or close study. |
| 80-89 | Strong project. Useful, credible, but narrower or less proven. |
| 70-79 | Supporting project. Relevant but incomplete, research-only, or adjacent. |
| 60-69 | Watchlist. Track, but do not treat as a leading option. |
| <60 | Exclude from the main project table. |

## Taxonomy

| Code | Category | Description |
|---|---|---|
| T1 | Surveys and theory | Definitions, taxonomies, position papers, system implications |
| T2 | Persistent conversational memory | Multi-session chat, user profiles, assistant personalization |
| T3 | Agentic memory management | Agent decides what to add, update, retrieve, delete, or ignore |
| T4 | Reflective and experiential memory | Lessons, trial feedback, self-reflection, reusable experience |
| T5 | Embodied and environment memory | Web, coding, Minecraft, game, robotics, or environment memories |
| T6 | Structured, graph, and database memory | Temporal KGs, symbolic stores, topic docs, governed memory states |
| T7 | Benchmarks and evaluation | Memory-specific benchmark or evaluation harness |
| T8 | Learned memory policies | RL/SFT-trained memory managers, compression controllers, reward models |
| T9 | Framework and production systems | Production memory layers, SDKs, frameworks, managed services |
| T10 | Boundary/general-agent work | Important adjacent work where memory is secondary |

Project-specific categories:

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

## Deduplication Rules

1. Treat a paper, project, and benchmark from the same team as separate entries only if each has a distinct use.
2. Prefer the most complete canonical source:
   - peer-reviewed page over arXiv if both exist and content is equivalent;
   - official GitHub repository over secondary list;
   - project documentation over marketing post.
3. Merge survey duplicates unless the newer survey materially changes taxonomy, date coverage, or benchmark analysis.
4. Keep original foundational work even when a project is renamed. Example: MemGPT remains a paper/project lineage even though Letta is the current platform.
5. Mark broad agent frameworks as boundary entries if memory is only a module, not the main project.

## Re-Scoring Policy

Re-score an entry when one of the following changes:

- A peer-reviewed version appears.
- Code, data, or benchmark results are released.
- The project changes license, maintenance status, or deployment model.
- A new benchmark changes relative standing.
- A product adds or removes deletion, provenance, multi-tenant isolation, or agent memory APIs.
- A survey introduces a better taxonomy or finds a serious flaw in prior memory claims.

## Minimum Metadata

Each curated record should include:

- Title or project name.
- Year or release era.
- Source type.
- Canonical URL.
- Taxonomy code.
- Score.
- One-sentence reason for inclusion.
- Notes on duplicates, aliases, or related projects.
