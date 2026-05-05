# Image inventory

This site has two kinds of figure:

1. **Inline HTML/CSS/SVG diagrams** ported from the earlier Google Sites
   page. These are rendered directly in the browser via Jekyll
   `{% raw %}{% include diagram-NAME.html %}{% endraw %}` — there is **nothing to upload** for
   them. They live in `/_includes/diagram-*.html`.
2. **Bitmap figures** from the four 2026 papers, which **do** need to
   be uploaded as PNGs into this directory.

## Inline diagrams (already wired)

| Diagram | Used on page | Source file |
|---|---|---|
| Causal problem (horizontal vs vertical causality) | `index.md` | `_includes/diagram-causal-problem.html` |
| Life at the edge of chaos | `index.md`, `framework.md` | `_includes/diagram-edge-of-chaos.html` |
| Modularity from cost minimisation (interactive) | `index.md`, `framework.md` | `_includes/diagram-modularity-animation.html` |
| "Meaning" cards (four-scale recasting) | `index.md` | `_includes/diagram-meaning-cards.html` |

These render automatically once the page loads. To edit them, open the
include file directly.

## Optional bitmap figures (upload to make them appear)

| Filename | Source | Used on page |
|---|---|---|
| `nwap-scales.png` | Frasch 2026a Figure&nbsp;1 panel&nbsp;C | `framework.md` (currently has no embed for this — add one if you want to include the panel) |
| `jphysiol-fig1.png` | full Figure&nbsp;1 from Frasch 2026a (panels A–E together) | `validation/physiology.md` |
| `2603-16951-headline.png` | the load-bearing figure from arXiv:2603.16951 | `validation/physics.md` |
| `2604-24805-headline.png` | the load-bearing figure from arXiv:2604.24805 | `validation/neural-architecture.md` |
| `tara-fig7-nullmodels.png` | Figure&nbsp;7 from the TARA biology paper (the four-null comparison) | `validation/biology.md` |

## How to drop a bitmap figure in

1. Export the figure from its source as a 2× resolution PNG (1600&nbsp;px wide is plenty).
2. Save with the filename above into this `/assets/img/` directory.
3. Open the page where the figure should appear and replace the blockquoted placeholder

   ```markdown
   > *Embed Figure X from ...*
   ```

   with a standard markdown image tag

   ```markdown
   ![Caption text]({% raw %}{{ '/assets/img/foo.png' | relative_url }}{% endraw %})
   ```

   The `{% raw %}{{ '...' | relative_url }}{% endraw %}` Liquid
   expression makes the path resolve correctly under both the staging
   URL (`martinfrasch.github.io/minaction-net/`) and the eventual
   custom domain (`minaction.net`).

4. Commit and push. GitHub Pages rebuilds in ~30&nbsp;seconds.

## Licence note

Frasch 2026a (J&nbsp;Physiol) is published under CC&nbsp;BY (open access).
You can re-use Figure&nbsp;1 panels on this site with citation. Frasch
2026b/c are arXiv preprints under your own copyright; you can use any
figure freely. The Tara biology paper figures are likewise yours.
