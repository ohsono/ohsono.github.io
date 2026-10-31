---
title: 'Toward an Auto-Synthesizer: Stress-Aware Selection and Recommendation of Deep Tabular Generative Models'

authors:
  - me

date: '2026-09-08T00:00:00Z'
publishDate: '2026-10-05T00:00:00Z'

publication_types: ['thesis']

publication:
  name: "Master's thesis, Applied Statistics & Data Science, University of California, Los Angeles"
  short_name: "UCLA Master's Thesis"

abstract: >-
  Deep generative models for tabular data — GANs, variational autoencoders,
  diffusion models, and LLM-based generators — exhibit highly non-uniform
  behavior across datasets: the best-performing family depends on
  distributional stressors such as long-tailed marginals, high-cardinality
  categoricals, Zipfian imbalance, and small-sample regimes. While automated
  machine learning resolved the analogous selection problem for supervised
  learning a decade ago, tabular synthesis still lacks an “Auto-Synthesizer”:
  its libraries standardize and benchmark generators but leave the question of
  which model to use to the practitioner, for whom evaluating every candidate —
  training, sampling, and scoring each under competing objectives of fidelity,
  privacy, and utility — is prohibitively expensive. This thesis studies
  intent-conditioned tabular synthesis selection and answers it with a
  two-system framework. Table-Synthesizers, the generation and measurement
  substrate, unifies 19 published generators behind a single interface and
  manufactures the empirical ground truth against which any selector must be
  judged. SYNTHONY, the selection layer, introduces stress profiling — a
  synthesis-specific, interpretable meta-feature representation quantifying
  dataset difficulty along four failure-mode-aligned dimensions — and matches
  stress profiles against a measurement-grounded, Bayesian-calibrated
  capability registry to rank candidates without training a single generator
  at inference time. Across a benchmark of 7 datasets, 10 synthesizers, and 3
  user intents, stress-based meta-features prove highly predictive of
  synthesizer performance: an oracle-informed nearest-neighbor reference
  attains 0.578 held-out Spearman rank correlation against intent-specific
  oracles, which this thesis independently reproduces (0.581) from the
  recovered evaluation matrix. The deployable zero-shot selector attains a
  reported 0.573 — within 0.005 of that reference at nine held-out pairs, a gap
  far smaller than the coarse granularity the sample size supports — while
  training no generator at inference time, remaining per-dimension inspectable
  and extensible to newly registered generators without benchmark reruns;
  independently reproducing that figure awaits recovery of the selector’s
  calibrated parameters from the original pipeline. Ablations show dataset
  stress profiling is the load-bearing component, and that freeing all
  registry parameters overfits at current ground-truth scale — motivating the
  framework’s re-runnable calibration pipeline. The reproduced selection signal
  is robust to the definition of the third intent, holding (Spearman
  0.52–0.58) whether downstream quality is measured by latency or a
  train-on-synthetic–test-on-real utility oracle. The thesis closes by
  specifying, at task granularity, the remaining distance to a closed-loop
  Auto-Synthesizer that executes, evaluates, and learns from its own
  recommendations.

summary: >-
  Master's thesis (UCLA): Table-Synthesizers (19 generators behind one interface)
  plus SYNTHONY's stress profiling, for selecting a tabular generative model
  without training every candidate.

tags:
  - Generative AI
  - Synthetic Data
  - Tabular Data
  - AutoML

featured: false

links:
  - type: custom
    label: eScholarship
    url: https://escholarship.org/uc/item/5nb9r7mc
  - type: custom
    label: Table-Synthesizers
    url: https://github.com/UCLA-Trustworthy-AI-Lab/table-synthesizers

projects:
  - synthony
  - table-synthesizers
---

Committee: Guang Cheng (chair), Fredric Schoenberg, Michael Tsiang.
