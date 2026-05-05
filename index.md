---
layout: default
title: minAction.net
description: A vertically organising principle for biological and learning systems.
permalink: /
---

## Living and learning systems organise toward a single functional.

The **Network-Weighted Action Principle (NWAP)** proposes that biological networks, neural architectures, and physical-law-discovery systems all extremise the same quantity — a balance of energy minimisation, information maximisation, and connection-cost penalty:

$$
S_{\text{NW}} \;=\; \int (E - I + A\!\cdot\!C)\,dt.
$$

The empirical prediction is sharp and falsifiable: networks under these constraints organise toward **high modularity**, with the modularity *excess* over appropriate null models scaling with optimisation pressure, and the *training-energy* required to learn falling under the same objective in engineered systems.

Over 2023–2026 we tested this prediction in four independent domains — **physiology**, **physics**, **neural architecture**, and **biology** — and the modularity-excess and energy-efficiency signatures appear in each. This site is the integrated record of that programme.

## The causal problem

The classical view in biology and machine learning is **horizontal**: each scale has its own mechanism, identified by within-scale interventions. Modern physiology has worked this way for a century; machine learning has worked this way since prediction error became the dominant optimisation target. But neither tradition has produced a *vertically organising principle* — a law that connects scales, that predicts what kind of structure should emerge under shared constraints.

NWAP is proposed as such a principle. It does not replace within-scale mechanisms; it predicts the *architectural target* that within-scale mechanisms converge on under the dual constraint of energy and information.

> **Embed the *causal problem* schematic** from <https://sites.google.com/frasch.ca/minaction-net/> — the diagram showing horizontal vs vertical causality across scales (organism → organ → tissue → cellular → molecular). Save as `/assets/img/causal-problem.png` and replace this block with `![The causal problem]({{ '/assets/img/causal-problem.png' | relative_url }})`.

## Life at the edge of chaos

Living systems sit in a narrow phase-transition zone between rigid order (crystals, ischaemia) and dissipative chaos (asthma, hyperinflammation). NWAP picks out this zone as the equilibrium of the action functional — neither pure energy minimisation nor pure information maximisation, but the joint extremum that admits both stability and adaptability.

> **Embed the *life at the edge of chaos* visual** from <https://sites.google.com/frasch.ca/minaction-net/>. Save as `/assets/img/edge-of-chaos.png`.

## Key evidence — modularity emerges from cost minimisation

Connection-cost minimisation, formally derived by Clune et al. (2013) and shown in [Frasch 2026a, Figure&nbsp;1D](https://doi.org/10.1113/JP290762), produces **modularity** as the structural signature: networks partition into densely-connected communities with sparse inter-module connections. The 2026 papers test this prediction in their respective domains.

> **Embed the *modularity-from-cost-minimisation* animation/figure** from <https://sites.google.com/frasch.ca/minaction-net/> — the inverse relationship between connection cost and modularity. Save as `/assets/img/modularity-evidence.png` (or the original GIF).

## "Meaning" — the speculative payoff

At the intersection of the four neighbouring variational frameworks (free-energy, dissipative adaptation, constructal theory, and the Network-Weighted Action) sits a thought-provoking conceptual target: **meaning**, operationally defined as successful uncertainty reduction through efficient action. Each framework captures one aspect of this convergence; NWAP is unique in carrying it as a measurable architectural prediction. We treat this as an open question worth posing, even if the current data cannot yet discriminate among the four accounts.

> **Embed Figure&nbsp;1 panel E** from [Frasch 2026a (J Physiol)](https://doi.org/10.1113/JP290762) — the Venn-style overlap with **"meaning"** at the centre. Save as `/assets/img/framework-convergence.png`.

## The four-domain validation, at a glance

<div class="domain-grid" markdown="0">
  <a class="domain-card" href="{{ '/validation/physiology/' | relative_url }}">
    <h3>Physiology</h3>
    <p>Vertically organising principles unify multi-scale causation; modularity is the architectural substrate. The theoretical anchor.</p>
    <span class="paper-ref">Frasch 2026a, <em>J Physiol</em></span>
  </a>
  <a class="domain-card" href="{{ '/validation/physics/' | relative_url }}">
    <h3>Physics</h3>
    <p>Triple-Action functional recovers Kepler &amp; Hooke laws from noisy data at order-of-magnitude reduced training energy.</p>
    <span class="paper-ref">Frasch 2026b, arXiv:2603.16951</span>
  </a>
  <a class="domain-card" href="{{ '/validation/neural-architecture/' | relative_url }}">
    <h3>Neural architecture</h3>
    <p>Energy-regularised objective improves training across 2,203 experiments. The strongest engineering proof of the programme.</p>
    <span class="paper-ref">Frasch 2026c, arXiv:2604.24805</span>
  </a>
  <a class="domain-card" href="{{ '/validation/biology/' | relative_url }}">
    <h3>Biology</h3>
    <p>Marine metabolic networks show a robust modularity excess (ΔQ ≈ 0.40) over bipartite-aware nulls; recurrent communities map to known functional units.</p>
    <span class="paper-ref">Frasch 2026d, <em>Tara Oceans</em> (in submission)</span>
  </a>
</div>

[Read the framework paper →]({{ '/framework/' | relative_url }}) &nbsp;·&nbsp; [Browse the four validations →]({{ '/validation/' | relative_url }}) &nbsp;·&nbsp; [Future work →]({{ '/future-work/' | relative_url }})
