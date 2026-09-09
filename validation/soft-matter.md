---
layout: default
title: "Validation: Soft matter (controlled test)"
permalink: /validation/soft-matter/
description: A controlled physical test of the antisymmetric-sector hypothesis in a nonreciprocal colloidal model — the first intervention experiment in the programme, and the first in which a prediction failed cleanly. Frasch 2026e.
lead: Frasch (2026e). Isolating the antisymmetric sector of a nonreciprocal colloidal model — kinetic unjamming, transient arrested coarsening, and irreversibility without coarse-grained circulation. Submitted to arXiv 9 September 2026; code and data at <a href="https://github.com/martinfrasch/nonrecip-modularity">github.com/martinfrasch/nonrecip-modularity</a>.
---

## The claim

The four validations above are observational or computational. This one is an intervention. The
hypothesis under test is a *directed-graph extension* of NWAP, formulated for this study and not
published elsewhere: a nonreciprocal coupling can be split into a **symmetric sector** that selects
structure by energy minimisation and an **antisymmetric sector** that adds circulation on top
without disturbing it. Three consequences follow. The antisymmetric sector should leave equal-time
structure untouched (solenoidality); its signature should appear as circulation in probability
currents; and, carried over from the biology paper, it should leave a sustained modularity excess in
the contact network. A fourth, weaker prediction is that cluster statistics should be controlled by
the antisymmetric-to-symmetric ratio.

## Method

The agent-based colloid model of Hara et al. (*Phys. Rev. Lett.* **137**, 068302, 2026): size-asymmetric
colloids driven by electrohydrodynamic flows, which exert unequal forces on each other. A
**reciprocity mixing parameter χ** scales the antisymmetric part of the pair force while leaving the
symmetric part bit-for-bit unchanged; χ = 0 restores Newton's third law exactly and χ = 1 recovers
the published law. Particles, packing, noise stream and symmetric attraction are held fixed, so any
difference between χ values is attributable to the antisymmetric sector alone. Four predictions were
pre-registered with pass/fail thresholds before any χ run. 113 blocked-design runs at five system
sizes from 10³ to 2.2 × 10⁴ particles, extended by continuations, committor relaunches,
fluctuation–response twins and small-timestep calibrations.

## The result

The mechanism the hypothesis assigned to the antisymmetric sector fails on all three counts, and the
structural control holds.

- **Solenoidality — refuted.** Scaling the antisymmetric sector alone changes the cluster count by an
  order of magnitude, and the added drift demonstrably does not preserve the reciprocal stationary
  density. The sector *restructures* rather than circulating on top of a structure it leaves alone.
- **Circulation — refuted in every projection examined.** The dynamics are irreversible, with a
  resolved excess dissipation, yet no circulation is detectable in any coarse observable: signed-area
  rates in observable planes, the cluster-size coordinate, an all-pairs lag test. The antisymmetric
  pair law is itself predominantly gradient on the contact graph.
- **Modularity excess — refuted with inverted sign.** Newman modularity is degenerate on these
  two-dimensional contact networks, and its excess over a degree-preserving null is *largest in the
  reciprocal reference* and decreases with nonreciprocity.
- **Structural control by the ratio — confirmed, non-monotonically.** Weak nonreciprocity unjams the
  reciprocal gel (fivefold fewer clusters), strong nonreciprocity fragments it (two orders of magnitude
  more). No proposed functional predicts the dip; a balance of kinetic rates describes it.

What the antisymmetric sector measurably does: it unjams a kinetically arrested reciprocal gel; it
sustains a fragment population whose channel pairs — shedding and reabsorption, fission and fusion,
nucleation and dissolution — are each approximately balanced; the fragmented state is a long-lived
transient whose condensation time scales linearly with system size; the selected scale of 8–10
particles is a critical-size crossover with a horizon-converged committor of one half; and its
dissipation switches on across the same structural crossover at which the symmetric forces stop
cancelling it (87–91 % of the unopposed contribution is cancelled above the crossover, all of it
within error below). On single-particle coordinates one effective temperature, equal to the bath's,
is shared by both species over a short-lag window that shrinks with drive.

## What this domain adds to the programme

This is the discriminating test that the [future-work page]({{ '/future-work/' | relative_url }})
asked for: a laboratory-style perturbation with a single knob, in which a prediction could fail
cleanly. It did. The **decomposition survives as an instrument** — constructing the split is what made
every measurement possible, and the sector it isolates has real, measurable consequences — but the
**mechanism assigned to it does not**, and the modularity-excess signature of the biology paper does
not transfer to two-dimensional contact networks at this density (a diagnosis specific to those
networks; it says nothing about the bipartite metabolic networks of Frasch 2026d, where the excess is
measured against a different null on a different topology).

The programme learns three things. First, "some variational principle applies" forbids nothing; what
makes a tier claim falsifiable is that each tier carries a measurable signature, and measuring one
honestly is harder than the taxonomy suggests — two of three commonly invoked near-equilibrium
diagnostics were defeated by their own construction. Second, whatever variational account applies to
this system covers at most its dynamics at fixed structure within a short-lag window; **structure
selection itself is a kinetic balance that no functional tested here reproduces**. That balance is the
concrete thing a functional for structure selection would have to reproduce, and it is the sharpest
target the programme now has. Third, the framework's author tested his own hypothesis and reports its
failure; that is the register the programme intends to keep.

## Code & data

- **GitHub:** [martinfrasch/nonrecip-modularity](https://github.com/martinfrasch/nonrecip-modularity)
  — model, all measurements, per-run summaries, the pre-registered protocol and the manuscript source.
- **Pre-registration:** `paper/EXPERIMENT.md` in the repository, thresholds committed before any χ run;
  outcomes tabulated in the paper's Section 5.1.
- **arXiv:** submitted 9 September 2026; identifier to follow.

<div class="see-also">
  <h3>See also — other validation domains</h3>
  <ul>
    <li><a href="{{ '/validation/physiology/' | relative_url }}">Physiology — vertically organising principles</a></li>
    <li><a href="{{ '/validation/physics/' | relative_url }}">Physics — physical-law discovery</a></li>
    <li><a href="{{ '/validation/neural-architecture/' | relative_url }}">Neural architecture — energy-first NAS</a></li>
    <li><a href="{{ '/validation/biology/' | relative_url }}">Biology — marine metabolic networks</a></li>
  </ul>
</div>
