# minaction-net

Source for [minaction.net](https://minaction.net), the public-facing site
for the **Network-Weighted Action Principle (NWAP)** research programme.

## Build

```bash
bundle install
bundle exec jekyll serve
# open http://127.0.0.1:4000
```

GitHub Pages builds the site automatically from the default branch — no
CI configuration needed.

## Structure

```
.
├── _config.yml                    # Site metadata, nav order, kramdown setup
├── _layouts/default.html          # The single layout (header/main/footer)
├── _includes/
│   ├── header.html                # Top navigation
│   └── footer.html                # Footer credits
├── assets/css/style.css           # Minimal academic theme
├── index.md                       # Home
├── framework.md                   # Formal explainer
├── validation/
│   ├── index.md                   # Four-domain landing
│   ├── physiology.md              # Frasch 2026a
│   ├── physics.md                 # Frasch 2026b (arXiv:2603.16951)
│   ├── neural-architecture.md     # Frasch 2026c (arXiv:2604.24805)
│   └── biology.md                 # Frasch 2026d (Tara Oceans, arXiv:2605.05254)
├── origins.md                     # 2023 → 2025 → 2026 arc
├── papers.md                      # Reference list, code, replication
├── about.md                       # Author, contact
└── CNAME                          # Custom-domain config (minaction.net)
```

## Adding a new validation paper

1. Drop a markdown file at `validation/<slug>.md` with `layout: default`
   front matter and the standard four-section template (claim → method →
   result → what this domain adds).
2. Add an entry to `validation_subpages` in `_config.yml`.
3. Append a new `.domain-card` block on `validation/index.md` and on
   `index.md`.
4. Cross-link from the four existing subpages' "see also" footers.

## Math

Equations render via [KaTeX](https://katex.org) (auto-render extension)
loaded from jsDelivr in `_layouts/default.html`. Use `$ ... $` for
inline and `$$ ... $$` for display. Kramdown is configured with
`math_engine: null` so it leaves the LaTeX raw for KaTeX to handle.

## Custom domain


## License

Content © Martin G. Frasch, CC&nbsp;BY&nbsp;4.0 unless noted. Code under MIT.
