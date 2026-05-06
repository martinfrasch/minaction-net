---
layout: default
title: "Validation: Physics"
permalink: /validation/physics/
description: Minimum-Action Learning — energy-constrained symbolic model selection for physical law identification from noisy data. Frasch 2026b.
lead: Frasch (2026b). Minimum-Action Learning — Energy-Constrained Symbolic Model Selection for Physical Law Identification from Noisy Data. <a href="https://arxiv.org/abs/2603.16951">arXiv:2603.16951</a>.
---

## The claim

If NWAP is a genuine principle of efficient learning, then a learning system that explicitly extremises the network-weighted action should discover physical laws *more efficiently* than systems that minimise prediction error alone.

## Method

A *Triple-Action functional* combining trajectory reconstruction, architectural sparsity, and energy-conservation enforcement is implemented as a training objective for symbolic regression. The functional is the discrete-time, finite-system analogue of $S_{\text{NW}}$.

Test problems are inverse problems with known ground truth — recovering Newton's law of gravitation from two-body trajectories, recovering Hooke's law from spring–mass oscillations — under varying noise levels.

## The result

The Triple-Action objective recovers Kepler's gravitational-force law and Hooke's law from noisy observational data **at order-of-magnitude reduced training energy** compared with prediction-error-only baselines. Recovered symbolic forms are identical; the saving is in the search.

## What this domain adds to the programme

It demonstrates that NWAP is operationally useful as a *training-time* objective — not only a post-hoc descriptive principle. A learning system explicitly extremising the network-weighted action discovers physics-grade laws faster than one that does not. **This is the first non-physiology, non-biology test of the framework, and the first to produce engineering value.**

![Trajectory reconstruction and Hamiltonian conservation under the Triple-Action functional]({{ '/assets/img/2603-16951-headline.png' | relative_url }})

*Headline figures from [Frasch 2026b (arXiv:2603.16951)](https://arxiv.org/abs/2603.16951). Top: trajectory reconstruction comparing the recovered force law to the ground-truth orbit. Bottom: soft-to-discrete architectural crystallisation under the Triple-Action functional — the gate distribution converges on a single basis (the true law) under temperature annealing.*

<div class="see-also">
  <h3>See also — other validation domains</h3>
  <ul>
    <li><a href="{{ '/validation/physiology/' | relative_url }}">Physiology — vertically organising principles</a></li>
    <li><a href="{{ '/validation/neural-architecture/' | relative_url }}">Neural architecture — energy-first NAS</a></li>
    <li><a href="{{ '/validation/biology/' | relative_url }}">Biology — marine metabolic networks</a></li>
  </ul>
</div>
