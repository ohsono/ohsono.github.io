---
title: 'Persistent Memory in Multi-Agent LLM Inference: What It Costs, What It Buys, and When You Can Tell'

authors:
  - me
  - Kyungdoe Han
  - Jaehan Koh
  - Xiaowu Dai
  - Wenlu Xu
  - Guang Cheng

author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

date: '2026-09-30T00:00:00Z'
publishDate: '2026-10-05T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: "The 10th Machine Learning for Systems Workshop (MLForSys) at NeurIPS 2026, Sydney, Australia — poster"
  short_name: "NeurIPS 2026 MLForSys"

peer_reviewed: true

abstract: >-
  Decomposing long-context inference across cooperating agents bounds the
  key-value cache that each call holds, rather than the total evidence, which
  matters when cache memory is the binding limit. Many such systems add a
  persistent tier that stores and recalls reasoning traces, and an ablation
  that reports an accuracy gain usually supports that tier. We measure both on
  one three-tier agent architecture. Decomposition delivers a peak key-value
  working set of 14.3 MiB per query, against 35.5 and 35.3 MiB for the
  single-pass and retrieval-augmented baselines. The persistent tier does not.
  Across eight controlled dataset pairs at n=100 questions per arm, it costs
  +0.368 MiB [+0.167, +0.590] of peak cache and produces no detectable accuracy
  change (+0.015, 95% confidence interval [−0.011, +0.046]). We argue that this
  null result is structural. Single-question benchmarks supply each item with
  its own evidence and score it independently, and a correct measurement resets
  stored traces between conditions, so recall has nothing informative to
  retrieve. Reaching this result took four measurement corrections, and none
  was visible in the results table. Three inflated the apparent benefit, and
  the fourth made an effect of that size look resolvable. We give the
  conditions that an agent-memory ablation must satisfy, with detection
  procedures that need no knowledge of the specific defect.

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

links:
  - type: pdf
    url: https://arxiv.org/pdf/2610.07782
  - type: source
    url: https://arxiv.org/abs/2610.07782

projects:
  - edge-llm-inference
---
