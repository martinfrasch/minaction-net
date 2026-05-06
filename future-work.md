---
layout: default
title: Future work
permalink: /future-work/
description: Open questions across the four-domain validation programme — discriminating tests, scale-up, cross-domain integration, and the speculative payoff of "meaning".
lead: Open questions across the four 2026 papers, organised by what each domain individually leaves unresolved and where the four together point next.
---

The four 2026 papers establish that the Network-Weighted Action Principle is consistent with the empirical signature it predicts in physiology, physics, neural architecture, and biology. The four together leave four substantive classes of question open. This page consolidates them.

{% include diagram-future-work.html %}

## I. Discrimination among neighbouring variational principles

The strongest unanswered question. The free-energy principle (Friston 2010), dissipative adaptation (England 2013), constructal theory (Bejan 2000), and the Network-Weighted Action all predict similar architectural signatures — modularity emergence, energy-cost minimisation, scale-invariant organisation. Across the current four papers we have shown that NWAP is *consistent with* the data; we have **not** shown that the data *discriminate for* NWAP against these alternatives.

What would discriminate:

- **Targeted predictions on which the four frameworks disagree.** Free-energy emphasises uncertainty reduction; dissipative adaptation emphasises entropy production; constructal theory emphasises flow geometry; NWAP emphasises connectivity-cost minimisation. Constructing a system in which the four predict *measurably different* modularity excess or energy-efficiency profiles is the most direct path to a discriminating test.
- **Intervention experiments.** Observational data (such as the Tara Oceans biology paper) cannot, in principle, discriminate among variational accounts that all explain the same observation. A laboratory perturbation — energy starvation, nutrient excess, antibiotic stress — that drives a measurable change in $\Delta Q$ in a *direction* predicted by NWAP and *not* by neighbouring frameworks would be the cleanest demonstration.
- **Cross-domain experiments.** The neural-architecture paper (Frasch 2026c) is the closest existing test, because it ablates the energy term $\lambda E(\theta, x)$ directly and measures the consequence. Extending this style of ablation to the other domains — explicitly removing the connectivity-cost term in synthetic biology, in physics-law discovery — would create a comparable engineering benchmark.

## II. Scale-up of each individual domain

Each of the four 2026 papers has a clean scale-up plan:

- **Physiology.** Move from theoretical synthesis to experimental tests: in vivo metabolic perturbation in model organisms, with $\Delta Q$ measured on KEGG-orthology networks reconstructed from the perturbed metaproteome. Cross-species: extend the framework's scale-invariant prediction across the 17 orders of magnitude that Kleiber's law spans.
- **Physics.** Extend the Triple-Action functional from gravitational and elastic-mechanics test problems (Kepler, Hooke) to electromagnetic, fluid-dynamic, and quantum-mechanical law-discovery benchmarks. The training-energy savings should scale, qualitatively, with the dimensionality and noise of the source data.
- **Neural architecture.** Scale the 2,203-experiment validation to billion-parameter regimes: language modelling with transformer-class architectures, multi-modal foundation models, and on-device biomedical-time-series models. The framework's prediction is that the relative benefit of the energy term should grow with task biological-realism — testable by comparing NAS efficiency across synthetic-data versus physiologically-grounded benchmarks.
- **Biology.** $n = 30$–$50$ Tara Oceans samples across the full latitudinal/depth gradient would tighten the modularity-excess confidence intervals and enable environment-dependent stratification. Cross-ecosystem replication (soil, gut, freshwater microbiomes) would test the universality of the bipartite-aware modularity-excess prediction. Cross-construction comparison (metabolite-flow vs FBA-derived vs pathway-membership networks) would isolate the construction-invariant signature of the constraint.

## III. The "meaning" question

The J Physiol paper (Frasch 2026a) closes by speculating that *meaning*, operationally defined as successful uncertainty reduction through efficient action, sits at the intersection of the four neighbouring variational frameworks. None of the four 2026 papers tests this directly. It is the conceptual payoff of the programme, and the most provocative open question.

Two paths suggest themselves:

- **Cross-domain dataset crossover.** Take the same dataset (a physiological signal, a microbiome, a learning curve) and analyse it under the four lenses simultaneously. If the four frameworks converge on identical *operational* readings of "meaning" — same effective-coupling parameter, same modularity excess, same entropy production — the convergence itself becomes evidence that "meaning" is a measurable, framework-invariant quantity.
- **Synthetic-system construction.** Build a small artificial system (a few-neuron network, a synthetic-biology pathway, a constrained-optimisation toy problem) in which the four frameworks each predict different "meaningful" outputs. Whichever framework's prediction matches reality picks out the operational definition of meaning that nature appears to use.

Both are speculative. Neither is in the four-paper programme. Both are in the natural extension of the framework's central conjecture.

## IV. Engineering applications under active development

A short list, mostly downstream of the neural-architecture paper, that the framework's training-time formulation makes available:

- **Energy-first NAS for edge and biomedical inference.** Devices with hard energy budgets (implantables, wearables, embedded biomedical sensors) benefit measurably from architectures trained under $\mathcal{L}_{\mathrm{CE}} + \lambda E(\theta,x)$. Quantification of this benefit on real device-constrained workloads is in progress.
- **Disease-associated dysbiosis as a modularity-excess signature.** If the modularity excess is the constrained-optimum signature of a healthy metabolic ensemble (biology paper, Discussion §4.6), then loss of excess under environmental, antibiotic, or pathological perturbation should be a quantitatively measurable signature of dysbiosis. Tractable in human-microbiome cohort data.
- **Symbolic-regression with action-functional regularisation.** The Triple-Action approach (Frasch 2026b) generalises beyond Kepler and Hooke. Fluid-dynamic equations, biological dose-response curves, and economic-time-series regularities are candidate next benchmarks.

---

The four-paper programme is the *baseline*. These three classes of question — discrimination, scale-up, and the meaning conjecture — are where the framework becomes either a quantitative theory of biological-and-learning organisation or a falsified hypothesis. Both outcomes are useful.
