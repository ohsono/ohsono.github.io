---
title: table-synthesizers
summary: Synthetic tabular data generation library & evaluation pipeline (16 architectures).
date: 2026-01-15
tags:
  - Synthetic Data
  - Generative AI
  - MLOps
links:
  - icon_pack: fab
    icon: github
    name: Code
    url: https://github.com/UCLA-Trustworthy-AI-Lab/table-synthesizers
  - icon: hero/academic-cap
    name: Thesis
    url: /publications/auto-synthesizer-thesis/
---

Unified 16 synthesizer architectures (CTGAN, TVAE, TabDDPM, AutoDiff, TabSyn,
AIM, PATECTGAN, DPCART, Bayesian Network, ARF, NFlow, GREAT, and more) behind a
single factory interface with per-model production configs. Built the
end-to-end training → generation → evaluation loop, integrating with
alfred-analytica for fidelity and machine-learning-efficacy scoring against real
data. Deployed distributed training on NCSA DeltaAI (SLURM, H100 GPU nodes) with
reproducible experiment tracking and versioned experiment outputs.

Table-Synthesizers is the generation and measurement substrate of my Master's
thesis, [*Toward an Auto-Synthesizer: Stress-Aware Selection and Recommendation of
Deep Tabular Generative Models*](/publications/auto-synthesizer-thesis/).
