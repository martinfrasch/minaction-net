---
layout: default
title: Future work
permalink: /future-work/
description: Open questions across the validation programme — discriminating tests, scale-up, structure selection after the colloid test, and the speculative payoff of "meaning".
lead: Open questions across the 2026 papers, organised by what each domain leaves unresolved and where they point next — including what the first controlled physical test (Frasch 2026e) changed.
---

The four 2026 validation papers establish that the Network-Weighted Action Principle is consistent with the empirical signature it predicts in physiology, physics, neural architecture, and biology. A fifth paper (Frasch 2026e, the [soft-matter test]({{ '/validation/soft-matter/' | relative_url }})) is the programme's first intervention experiment, and its outcome reshapes the open questions: the mechanism a directed-graph extension of NWAP assigned to the antisymmetric sector of a nonreciprocal coupling is refuted, the modularity-excess signature fails with inverted sign on two-dimensional contact networks, and structure selection turns out to be a kinetic balance that no functional tested there reproduces. This page consolidates what remains open.

{% include diagram-future-work.html %}

## I. Discrimination among neighbouring variational principles

The strongest unanswered question. The free-energy principle (Friston 2010), dissipative adaptation (England 2013), constructal theory (Bejan 2000), and the Network-Weighted Action all predict similar architectural signatures — modularity emergence, energy-cost minimisation, scale-invariant organisation. Across the current four papers we have shown that NWAP is *consistent with* the data; we have **not** shown that the data *discriminate for* NWAP against these alternatives.

The colloid test (Frasch 2026e) is the first such experiment. It discriminated — but against the framework's own directed-graph extension rather than for NWAP over its neighbours: the intervention (scaling the antisymmetric sector alone) produced a clean failure of solenoidality, circulation and the modularity signature, and a non-monotonic structural response that no proposed functional, NWAP's included, predicts. That is the outcome an intervention is for. What it did not do is separate NWAP from the free-energy principle or dissipative adaptation, because the boundary it found — a variational account can cover the dynamics at fixed structure, and structure selection is a separate, kinetic problem — applies to all three.

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

## III. Structure selection after the colloid test

The sharpest target the programme now has is concrete. In the colloid model the fragment
population is a steady kinetic balance — condensate shedding against reabsorption, fission against
fusion, nucleation against dissolution, each pair approximately balanced — and the non-monotonic
cluster count follows from the two condensate rates switching on at different drives. Newman
modularity does not see any of this. A functional for structure selection would have to reproduce
that balance, and the candidates are the nonequilibrium quasipotential and large-deviation
constructions, none of which the colloid paper tested. Three narrower items follow from the same
paper: a frequency-resolved fluctuation–response measurement (correlation and dissipative response
spectra, the Harada–Sasa sum rule) to turn the measured short-lag agreement window into a spectral
statement; the physical analogue of the mixing parameter, the electrohydrodynamic radius contrast,
swept with compensation of the symmetric coupling; and many-body hydrodynamics, the one ingredient of
the source experiment the agent-based model omits and the one that could stabilise finite clusters.

## IV. The "meaning" question

The J Physiol paper (Frasch 2026a) closes by speculating that *meaning*, operationally defined as successful uncertainty reduction through efficient action, sits at the intersection of the four neighbouring variational frameworks. None of the four 2026 papers tests this directly. It is the conceptual payoff of the programme, and the most provocative open question.

Two paths suggest themselves:

- **Cross-domain dataset crossover.** Take the same dataset (a physiological signal, a microbiome, a learning curve) and analyse it under the four lenses simultaneously. If the four frameworks converge on identical *operational* readings of "meaning" — same effective-coupling parameter, same modularity excess, same entropy production — the convergence itself becomes evidence that "meaning" is a measurable, framework-invariant quantity.
- **Synthetic-system construction.** Build a small artificial system (a few-neuron network, a synthetic-biology pathway, a constrained-optimisation toy problem) in which the four frameworks each predict different "meaningful" outputs. Whichever framework's prediction matches reality picks out the operational definition of meaning that nature appears to use.

Both are speculative. Neither is in the four-paper programme. Both are in the natural extension of the framework's central conjecture.

## V. Engineering applications under active development

A short list, mostly downstream of the neural-architecture paper, that the framework's training-time formulation makes available:

- **Energy-first NAS for edge and biomedical inference.** Devices with hard energy budgets (implantables, wearables, embedded biomedical sensors) benefit measurably from architectures trained under $\mathcal{L}_{\mathrm{CE}} + \lambda E(\theta,x)$. Quantification of this benefit on real device-constrained workloads is in progress.
- **Disease-associated dysbiosis as a modularity-excess signature.** If the modularity excess is the constrained-optimum signature of a healthy metabolic ensemble (biology paper, Discussion §4.6), then loss of excess under environmental, antibiotic, or pathological perturbation should be a quantitatively measurable signature of dysbiosis. Tractable in human-microbiome cohort data.
- **Symbolic-regression with action-functional regularisation.** The Triple-Action approach (Frasch 2026b) generalises beyond Kepler and Hooke. Fluid-dynamic equations, biological dose-response curves, and economic-time-series regularities are candidate next benchmarks.

---

The four validation papers are the *baseline*, and the colloid test is the first result on the other side of the ledger. These classes of question — discrimination, scale-up, structure selection, and the meaning conjecture — are where the framework becomes either a quantitative theory of biological-and-learning organisation or a falsified hypothesis. The colloid paper shows what the second outcome looks like for one specific extension, and the programme reports it in the same place as the confirmations.
