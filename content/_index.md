---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-08-03
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: markdown
    content:
      title: '🔬 Research Focus'
      subtitle: ''
      text: |-
        I work the gap between GenAI/LLM research and the systems that have to
        run it in production. Concretely: agentic, intent-conditioned tooling for
        generative-model selection (**Synthony**), the training/evaluation
        infrastructure that supports it at scale (**table-synthesizers**), and the
        database, SRE, and DevOps foundation that makes either one reliable.

        My thesis direction extends this into applying LLM-driven reasoning — RAG
        and **Chain-of-Agents (COA)** orchestration — to systems-engineering
        decisions, treating "which model," "which architecture," and "which infra
        tradeoff" as the same class of problem: a research-to-production gap that
        needs both ML judgment and engineering rigor to close.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Publications
      filters:
        folders:
          - publications
    design:
      view: citation
---
