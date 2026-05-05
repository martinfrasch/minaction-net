---
layout: default
title: Framework
permalink: /framework/
description: The Network-Weighted Action Principle, formally stated, with the modularity-excess prediction across physiology, physics, neural architecture, and biology.
lead: The Network-Weighted Action Principle, formally stated, with one shared architectural prediction tested across four domains.
---

## A dual constraint that runs through living and learning systems

The minAction.net programme starts from a simple observation: **complex biological and learning systems face a dual constraint**. They must minimise the energetic cost of operation, while simultaneously maximising the diversity of information they can process or represent. Either pole alone is degenerate — pure energy minimisation collapses to a static crystal; pure information maximisation diverges into noise. The systems we care about — brains, metabolic networks, evolved ecosystems, trained models — sit at the *edge of chaos* between these limits, and the equilibria they pick are structured.

> **Embed Figure 1 panel B** from [Frasch 2026a (J Physiol)](https://doi.org/10.1113/JP290762) — *Life at the Edge of Chaos* — showing the narrow phase-transition zone where systems are simultaneously ordered and adaptable. The figure is openly accessible at the paper's DOI. Save as `/assets/img/edge-of-chaos.png` and replace this block with `![Edge of chaos](/assets/img/edge-of-chaos.png)`.

## The Network-Weighted Action

The Network-Weighted Action Principle proposes that the equilibrium is the extremum of

$$
S_{\text{NW}} \;=\; \int (E - I + A\!\cdot\!C)\,dt
$$

where $E$ is energy or operational cost, $I$ is the system's information / diversity, $A$ is a connectivity weight, and $C$ is the cost of forming and maintaining connections. The action $S_{\text{NW}}$ generalises classical Hamiltonian and Lagrangian formulations of physics to systems where *connectivity itself is a state variable* — as it is in biological and neural networks.

The integral is taken over network ensembles at any chosen scale — molecular to organismal, neuron to network, model to architecture — without reformulation. Noble's principle of biological relativity becomes a property of the action, not an external constraint.

> **Embed Figure 1 panel C** from [Frasch 2026a (J Physiol)](https://doi.org/10.1113/JP290762) — *Network-Weighted Action across scales* — showing the action functional operating over physical, cellular, tissue, organ, and organism networks. Save as `/assets/img/nwap-scales.png`.

## One architectural prediction, tested four ways

The action does not just predict that systems organise: it predicts *how*. Connection-cost minimisation, formally derived in Clune et al. (2013), produces **modularity** as a structural signature: networks partition into densely-connected communities with sparse inter-module connections.

This is the load-bearing prediction of the framework, because modularity is measurable. It is also testable in **engineered systems** as a *training-time constraint*: an artificial network that explicitly extremises the action should learn more efficiently and generalise better than one that minimises prediction error alone.

The four-domain programme reduces to asking the same question, expressed in each domain's native variables:

> *Does the system the framework points us at exhibit the architectural and energetic signature the framework predicts?*

| Domain | Native variable | Empirical test |
|---|---|---|
| **Physiology** | scale-invariant integration | Modularity of biological networks (Clune 2013) recovered from a single action principle that also reproduces Kleiber's $3/4$ scaling. |
| **Physics** | training-data efficiency | Triple-Action functional recovers Kepler's law and Hooke's law from noisy data at order-of-magnitude reduced training energy. |
| **Neural architecture** | training efficiency + generalisation | Energy-regularised objective $\mathcal{L}_{\mathrm{CE}} + \lambda E(\theta,x)$ improves training across 2,203 experiments, with the benefit graded by task biological-realism. |
| **Biology** | modularity excess on metabolic-network ensembles | Marine metagenomic networks exhibit $\Delta Q \approx 0.40$ over a bipartite-aware null; recurrent communities map to known functional units. |

The signature is the **same prediction** in four very different empirical settings. None of the four tests, taken alone, would falsify or uniquely confirm the framework. **Together** they form a multi-domain pattern: the same architectural target — modular, sparsely-connected, energy-conserving organisation — appears wherever the framework points.

> **Embed Figure 1 panel D** from [Frasch 2026a (J Physiol)](https://doi.org/10.1113/JP290762) — *Emergence of modularity from cost minimisation* — showing the inverse relationship between connection cost and modularity, the testable architectural signature. Save as `/assets/img/modularity-from-cost.png`.

## Why this is not just another variational principle

Variational principles in biology are not new. The **free-energy principle** (Friston, 2010), **dissipative adaptation** (England, 2013), and **constructal theory** (Bejan, 2000) all propose that living systems extremise some quantity. Each predicts modularity emergence, qualitatively. NWAP differs in two respects:

1. **It is multi-scale by construction.** A single action covers physiology and machine learning without reformulation, because connectivity cost $A\!\cdot\!C$ enters the action symmetrically with $E$ and $I$.

2. **It makes a quantitative architectural prediction at *training* time.** Modularity excess $\Delta Q$ over bipartite-aware nulls *and* training-energy efficiency are both load-bearing observables. The neural-architecture paper (Frasch 2026c) operationalises the second; the biology paper (Frasch 2026d) operationalises the first; the physics paper (Frasch 2026b) shows both can hold simultaneously in a controlled test.

Discriminating tests against the neighbouring variational frameworks remain future work — see the [Future work](/future-work/) tab. The current programme establishes that NWAP is **consistent with** the empirical signature in every domain tested so far, and uniquely useful as a *constructive* training objective in domains where engineering verification is possible.

## The convergence diagram

> **Embed Figure 1 panel E** from [Frasch 2026a (J Physiol)](https://doi.org/10.1113/JP290762) — *Convergence of theoretical frameworks* — the Venn-style overlap of free-energy principle, dissipative adaptation, network-weighted action, and phase transitions, with **"meaning"** at the centre. Save as `/assets/img/framework-convergence.png`.

"Meaning" — operationally defined in the J Physiol paper as successful uncertainty reduction through efficient action — sits at the intersection of the four neighbouring accounts. It is the speculative payoff of the programme: a framework that connects measurable architectural signatures (modularity excess, training-energy efficiency) to a higher-level concept that has otherwise resisted quantification. We treat this as the open conceptual question, addressed from each side by the four 2026 papers and explicitly listed under [Future work](/future-work/).
