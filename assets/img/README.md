# Image inventory

Each markdown page has a blockquoted *"Embed X..."* placeholder where a
figure belongs. To make the site show those figures, drop the source
files into this directory using the filenames listed below — the
markdown is already wired to render them once the files exist.

## Required files

| Filename | Source | Used on page |
|---|---|---|
| `causal-problem.png` | export from your existing Google Sites diagram | `index.md` (Home — *The causal problem*) |
| `edge-of-chaos.png` | Frasch 2026a (J&nbsp;Physiol) Figure&nbsp;1 panel&nbsp;B, OR your existing Google Sites *"life at edge of chaos"* visual | `index.md` and `framework.md` |
| `nwap-scales.png` | Frasch 2026a Figure&nbsp;1 panel&nbsp;C | `framework.md` |
| `modularity-evidence.png` | the modularity-emerges-from-cost-minimisation animation/figure on your existing Google Sites page | `index.md` |
| `modularity-from-cost.png` | Frasch 2026a Figure&nbsp;1 panel&nbsp;D | `framework.md` |
| `framework-convergence.png` | Frasch 2026a Figure&nbsp;1 panel&nbsp;E (the Venn-style overlap with **"meaning"**) | `index.md` and `framework.md` |
| `jphysiol-fig1.png` | full Figure&nbsp;1 from Frasch 2026a (panels A–E together) | `validation/physiology.md` |
| `2603-16951-headline.png` | the load-bearing figure from arXiv:2603.16951 | `validation/physics.md` |
| `2604-24805-headline.png` | the load-bearing figure from arXiv:2604.24805 | `validation/neural-architecture.md` |
| `tara-fig7-nullmodels.png` | Figure&nbsp;7 from the TARA biology paper (the four-null comparison) | `validation/biology.md` |

## How to drop them in

1. Export each visual from its source as a 2× resolution PNG (1600&nbsp;px wide is plenty).
2. Save with the filename above into this `/assets/img/` directory.
3. Open the page where the figure should appear and replace the blockquoted placeholder

   ```markdown
   > **Embed Figure X from ...** Save as `/assets/img/foo.png` ...
   ```

   with a standard markdown image tag

   ```markdown
   ![Caption text]({{ '/assets/img/foo.png' | relative_url }})
   ```

   The `{{ '...' | relative_url }}` Liquid expression is what makes the
   path resolve correctly under both the staging URL
   (`martinfrasch.github.io/minaction-net/`) and the eventual custom
   domain (`minaction.net`).

4. Commit and push. GitHub Pages rebuilds in ~30&nbsp;seconds.

## Licence note

Frasch 2026a (J&nbsp;Physiol) is published under CC&nbsp;BY (open access).
You can re-use Figure&nbsp;1 panels on this site with citation. Frasch
2026b/c are arXiv preprints under your own copyright; you can use any
figure freely. The Tara biology paper figures are likewise yours.

The Google Sites visuals are also yours; export them at full resolution
before the site is retired.
