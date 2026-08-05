---
title: 'SYNTHONY: A Stress-Aware, Intent-Conditioned Agent for Deep Tabular Generative Models Selection'

authors:
  - me
  - Xiaofeng Lin
  - Jason Ni
  - Guang Cheng

date: '2026-03-31T00:00:00Z'
publishDate: '2026-03-31T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: "ICLR 2026 Workshop on Deep Learning for Tabular Data (DeLTA)"
  short_name: "ICLR 2026 DeLTA"

peer_reviewed: true

abstract: >-
  Deep generative models for tabular data perform inconsistently across
  datasets. We propose "stress profiling," a method to characterize dataset
  difficulty along four dimensions, and introduce SYNTHONY — a framework that
  matches stress profiles against a calibrated capability registry of
  synthesizer families. Across 7 datasets, 10 synthesizers, and 3 user intents,
  our stress-based approach substantially outperforms random selection and
  zero-shot language-model baselines at identifying the best-fit synthesizer.

summary: >-
  Stress-aware, intent-conditioned agent that recommends the best-fit tabular
  generative model for a dataset instead of defaulting to one architecture.

tags:
  - Generative AI
  - Synthetic Data
  - LLM Agents
  - Tabular Data

featured: true

links:
  - type: pdf
    url: https://arxiv.org/pdf/2604.00293
  - type: source
    url: https://arxiv.org/abs/2604.00293
  - type: code
    url: https://github.com/UCLA-Trustworthy-AI-Lab/Synthony

projects:
  - synthony

image:
  caption: ''
  focal_point: ''
  preview_only: false
---

**SYNTHONY** treats synthesizer selection as a matching problem: it profiles a
dataset's "stress" — privacy sensitivity, class imbalance, cardinality, and
sample size — and matches that profile against a calibrated capability registry
of synthesizer families (GAN, VAE, Diffusion, DP-based, Bayesian, Normalizing
Flow). It supports rule-based, LLM-based, and hybrid ranking with explainable
tie-breaking and benchmark-driven comparison.
