---
title: Edge LLM Inference via Chain of Agents
summary: Memory-efficient local LLM inference using a Chain-of-Agents approach.
date: 2026-06-01
tags:
  - LLM Agents
  - Edge AI
  - Inference Optimization
---

A Chain-of-Agents approach to memory-efficient large language model inference on
resource-constrained edge devices. Accepted as a poster at the NeurIPS 2026
Workshop on Machine Learning for Systems (MLForSys): *Persistent Memory in
Multi-Agent LLM Inference: What It Costs, What It Buys, and When You Can Tell*.
Agent decomposition bounds peak KV cache per query about 60% below single-pass
and RAG baselines at accuracy parity; the persistent memory tier costs a little
cache and buys no measurable accuracy on single-question benchmarks.
