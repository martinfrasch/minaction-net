---
layout: default
title: Origins
permalink: /origins/
description: How the minAction.net research programme came together — from the 2023 NAS seed paper to the 2026 four-domain validation.
lead: The framework didn't arrive in one paper. It emerged from a 2023 neuroscience-led question and was reformulated three times as the empirical scope expanded.
---

## 2023 — The seed paper

*Brain development dictates energy constraints on neural architecture search: cross-disciplinary insights on optimization strategies* — [arXiv:2310.03042](https://arxiv.org/abs/2310.03042).

The starting question was practical: AI's neural-architecture-search community was treating prediction error as the optimisation target, but developmental neuroscience suggests that real brains optimise *energy* first and prediction second. Could energy-first NAS beat prediction-error-first NAS?

## 2025 — Philosophical formulation

*Causal Thinking in Physiology: A Search for Vertically Organizing Principles* — [PhilSci archive 26949](https://philsci-archive.pitt.edu/26949/).

The neuroscience question generalised: if energy-first optimisation is the rule for biological networks, the same principle should apply to any system extremising a functional that includes connectivity cost. Schöner and Kelso's dynamic-coordination theory (1988) provided the mathematical bridge — a network-weighted action could subsume both the biological and the engineered cases.

## 2026 — Quantitative validation

Four papers in 2026 operationalise and test the framework:

- *Causal thinking in physiology* (Frasch 2026a, *J Physiol*, DOI&nbsp;[10.1113/JP290762](https://doi.org/10.1113/JP290762)) — formal framework + multi-scale unification. **[Read →]({{ '/validation/physiology/' | relative_url }})**
- *Minimum-Action Learning* (Frasch 2026b, [arXiv:2603.16951](https://arxiv.org/abs/2603.16951)) — physics-law discovery at reduced training energy. **[Read →]({{ '/validation/physics/' | relative_url }})**
- *minAction.net: Energy-First Neural Architecture* (Frasch 2026c, [arXiv:2604.24805](https://arxiv.org/abs/2604.24805)) — 2,203-experiment validation at the architecture-design scale. **[Read →]({{ '/validation/neural-architecture/' | relative_url }})**
- *Modularity Emerges from Action-Functional Constraints* (Frasch 2026d, [arXiv:2605.05254](https://arxiv.org/abs/2605.05254)) — biology-scale validation in marine metagenomic networks. Code and data: [github.com/martinfrasch/tara-modularity](https://github.com/martinfrasch/tara-modularity). **[Read →]({{ '/validation/biology/' | relative_url }})**

The site reflects this arc: the same framework, four independent tests, each making the case for the architectural-modularity prediction in its own domain.
