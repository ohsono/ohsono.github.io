---
title: 'Persistent Memory in Multi-Agent LLM Inference: What It Costs, What It Buys, and When You Can Tell'

authors:
  - me
  - Kyungdoe Han
  - Jaehan Koh
  - Xiaowu Dai
  - Wenlu Xu
  - Guang Cheng

date: '2026-09-30T00:00:00Z'
publishDate: '2026-10-05T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: "NeurIPS 2026 Workshop on Machine Learning for Systems (MLForSys), poster"
  short_name: "NeurIPS 2026 MLForSys"

peer_reviewed: true

abstract: >-
  Decomposing long-context inference across cooperating agents bounds the
  active KV cache per call rather than total evidence, which matters when
  KV-cache memory binds. Many such systems add a persistent tier storing and
  recalling reasoning traces, usually validated by an ablation reporting an
  accuracy gain. We measure both on one three-tier agent architecture.
  Decomposition delivers: peak KV working set of 14.3 MiB per query against
  35.5 and 35.3 MiB for single-pass and retrieval-augmented baselines. The
  persistent tier does not: across eight controlled dataset pairs at n=100 per
  arm it costs +0.368 MiB [+0.167, +0.590] of peak cache and produces no
  detectable accuracy change (+0.015, 95% CI [−0.011, +0.046]). We argue the
  null is structural: single-question benchmarks supply each item with its own
  evidence and score it independently, and correctness requires resetting
  stored traces between conditions, so recall has nothing informative to
  retrieve. Reaching it took four measurement corrections — three inflating the
  apparent benefit, the fourth making an effect that size look resolvable —
  none visible in the results table. We give the conditions an agent-memory
  ablation must satisfy and detection procedures that need no knowledge of the
  specific defect.

summary: >-
  Agent decomposition bounds peak KV cache 2.5× below single-pass and RAG
  baselines; the persistent memory tier such systems are usually paired with
  costs cache and buys no measurable accuracy.

tags:
  - LLM Inference
  - KV Cache
  - LLM Agents
  - Chain-of-Agents
  - Reproducibility

featured: true

# TODO: add the arXiv link once the ID is known, e.g.
#   - type: preprint
#     provider: arxiv
#     id: '26xx.xxxxx'
links: []

projects:
  - edge-llm-inference
---
