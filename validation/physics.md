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

> *Embed key figure from the arXiv paper at `/assets/img/2603-16951-headline.png`.*

<div class="see-also">
  <h3>See also — other validation domains</h3>
  <ul>
    <li><a href="/validation/physiology/">Physiology — vertically organising principles</a></li>
    <li><a href="/validation/neural-architecture/">Neural architecture — energy-first NAS</a></li>
    <li><a href="/validation/biology/">Biology — marine metabolic networks</a></li>
  </ul>
</div>
