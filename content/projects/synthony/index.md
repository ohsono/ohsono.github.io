---
title: Synthony
summary: Stress-aware, intent-conditioned agent for generative model selection.
date: 2026-03-31
tags:
  - Generative AI
  - LLM Agents
  - Synthetic Data
links:
  - icon_pack: fab
    icon: github
    name: Code
    url: https://github.com/UCLA-Trustworthy-AI-Lab/Synthony
  - icon_pack: ai
    icon: arxiv
    name: Paper
    url: https://arxiv.org/abs/2604.00293
---

An agent that recommends the best-fit tabular generative model (GAN / VAE /
Diffusion / DP-based / Bayesian / Normalizing Flow) for a given dataset by
profiling its "stress" characteristics — privacy sensitivity, class imbalance,
cardinality, sample size — instead of defaulting to one architecture. Implements
rule-based, LLM-based, and hybrid ranking strategies with explainable
tie-breaking and benchmark-driven comparison. Published at ICLR 2026 DeLTA.
