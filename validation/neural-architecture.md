---
layout: default
title: "Validation: Neural architecture"
permalink: /validation/neural-architecture/
description: Energy-first neural architecture design — from biological principles to systematic validation. Frasch 2026c.
lead: Frasch (2026c). minAction.net — Energy-First Neural Architecture Design — From Biological Principles to Systematic Validation. <a href="https://arxiv.org/abs/2604.24805">arXiv:2604.24805</a>.
---

## The claim

If NWAP describes how biological neural systems organise, then artificial neural networks regularised by the same principle should train more efficiently and generalise better than prediction-error-only baselines, in ways that scale with the energy term.

## Method

The energy-regularised objective

$$
\mathcal{L} \;=\; \mathcal{L}_{\mathrm{CE}} \;+\; \lambda\, E(\theta, x)
$$

is implemented across **2,203 experiments** spanning vision (CIFAR, ImageNet subsets), text (small language modelling), neuromorphic (spiking-net benchmarks), and physiological time-series datasets.

The energy term $E(\theta, x)$ approximates the metabolic-cost analogue for an artificial network: a function of activation magnitude, weight density, and forward-pass FLOPs. Sweeps over $\lambda$ identify the regime in which the regulariser contributes a measurable benefit.

## The result

Across the 2,203 experiments, the energy-regularised objective produces:

1. **Faster convergence** at fixed accuracy.
2. **Sparser learned architectures** with retained accuracy.
3. **Better generalisation** on out-of-distribution test sets.

The benefit is largest for biologically-inspired tasks (physiological time series, neuromorphic) and smallest for synthetic tasks where the data distribution is artificial.

## What this domain adds to the programme

This is the *architectural*-scale test. It establishes that NWAP is not only a descriptive principle of natural biological networks but a **constructive principle for designing artificial ones**. The graded benefit by task biological-realism is itself a falsifiable prediction of the framework: the more the data are drawn from a biological process, the more an explicit energy term should help.

![Energy-first neural architectures: BimodalTrue and Physics-Lagrangian]({{ '/assets/img/2604-24805-headline.png' | relative_url }})

*Figure&nbsp;1 from [Frasch 2026c (arXiv:2604.24805)](https://arxiv.org/abs/2604.24805). The two energy-first architectures evaluated across 2,203 experiments: BimodalTrue (top), implementing dual-pathway processing inspired by neuron–glia metabolic specialisation; and Physics-Lagrangian (bottom), decomposing the forward pass into kinetic ($T$), potential ($V$), and constraint ($C$) pathways.*

<div class="see-also">
  <h3>See also — other validation domains</h3>
  <ul>
    <li><a href="{{ '/validation/physiology/' | relative_url }}">Physiology — vertically organising principles</a></li>
    <li><a href="{{ '/validation/physics/' | relative_url }}">Physics — physical-law discovery</a></li>
    <li><a href="{{ '/validation/biology/' | relative_url }}">Biology — marine metabolic networks</a></li>
  </ul>
</div>
