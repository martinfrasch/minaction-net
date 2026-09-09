---
layout: default
title: Papers & Code
permalink: /papers/
description: Canonical reference list, code repositories, and replication details for the minAction.net programme.
---

## Framework papers

- Frasch, M.&nbsp;G. (2023). *Brain development dictates energy constraints on neural architecture search: cross-disciplinary insights on optimization strategies.* [arXiv:2310.03042](https://arxiv.org/abs/2310.03042).

- Frasch, M.&nbsp;G. (2025). *Causal Thinking in Physiology: A Search for Vertically Organizing Principles.* [PhilSci archive 26949](https://philsci-archive.pitt.edu/26949/).

## Four-domain validation (2026)

- Frasch, M.&nbsp;G. (2026a). *Causal thinking in physiology: A search for vertically organising principles.* The Journal of Physiology. DOI:&nbsp;[10.1113/JP290762](https://doi.org/10.1113/JP290762).

- Frasch, M.&nbsp;G. (2026b). *Minimum-Action Learning: Energy-Constrained Symbolic Model Selection for Physical Law Identification from Noisy Data.* [arXiv:2603.16951](https://arxiv.org/abs/2603.16951).

- Frasch, M.&nbsp;G. (2026c). *minAction.net: Energy-First Neural Architecture Design — From Biological Principles to Systematic Validation.* [arXiv:2604.24805](https://arxiv.org/abs/2604.24805).

- Frasch, M.&nbsp;G. (2026d). *Modularity Emerges from Action-Functional Constraints in Marine Metabolic Networks: A Biology-Scale Validation of the Network-Weighted Action Principle.* [arXiv:2605.05254](https://arxiv.org/abs/2605.05254).

## Controlled physical test (2026)

- Frasch, M.&nbsp;G. (2026e). *Isolating the antisymmetric sector of a nonreciprocal colloidal model: kinetic unjamming, transient arrested coarsening, and irreversibility without coarse-grained circulation.* Submitted to arXiv 9 September 2026; identifier to follow. Tests a directed-graph extension of NWAP by intervention and reports its failure. **[Read →]({{ '/validation/soft-matter/' | relative_url }})**

## Code & data

- **TARA biology paper code & data:** [github.com/martinfrasch/tara-modularity](https://github.com/martinfrasch/tara-modularity). Compiles end-to-end in &asymp;30&nbsp;s on an Apple M2 Max from a clean clone (after pulling annotations).
- **Nonreciprocal-colloid code, data summaries and manuscript (Frasch 2026e):** [github.com/martinfrasch/nonrecip-modularity](https://github.com/martinfrasch/nonrecip-modularity) — model, every measurement, the pre-registered protocol with thresholds committed before running, and the manuscript source.
- **eggNOG annotations:** `gs://minaction-tara-gauge-backup/annotations/latest/` &mdash; public read, no authentication.
- **Zenodo DOI:** *to be added at acceptance of the biology paper.*
- **Physics law-discovery code (Frasch 2026b):** see the *Code Availability* section of [arXiv:2603.16951](https://arxiv.org/abs/2603.16951) for the canonical repository link.
- **Energy-first NAS code (Frasch 2026c):** see the *Code Availability* section of [arXiv:2604.24805](https://arxiv.org/abs/2604.24805) for the canonical repository link.

## Replication

The nonreciprocal-colloid repository runs from a clean clone with `python -m` module invocations documented in its README; simulations take about 700 s per 10⁶ steps at 1,000 particles per core. The TARA biology paper compiles end-to-end in approximately 30&nbsp;seconds on an Apple M2 Max from a clean clone, after pulling the seven eggNOG annotations from the GCS bucket. The repository's README walks through the pipeline. The physics and NAS papers each include their own replication scripts in their respective repositories.

## How to cite the programme

> Frasch, M.&nbsp;G. (2026). *minAction.net: A four-domain validation of the Network-Weighted Action Principle.* Series of preprints and peer-reviewed papers. https://minaction.net.

Or cite the individual papers above.
