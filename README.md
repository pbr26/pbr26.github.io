# Pramod B R — Quantitative Pharmacology Portfolio

Professional Quarto portfolio for **pharmacokinetics, pharmacometrics, PK/PD, PBPK, DMPK/TK, R, Python, data science and scientific AI**.

Live site: <https://pbr26.github.io/>

## Local preview / render

```bash
quarto preview     # local live preview
quarto render      # build the site into _site/
quarto check       # verify the Quarto installation
```

## Structure

```text
_quarto.yml                 # site config, navbar, footer, SEO, favicon, OpenGraph
styles.css                  # premium scientific design system
index.qmd                   # homepage (hero, stats, cards, featured projects)
projects.qmd                # projects index
pharmacometrics.qmd         # methods & workflow
data-science.qmd            # R / Python toolkit (tiered by experience)
ai.qmd                      # generative AI (human-in-the-loop)
research.qmd                # research interests
about.qmd                   # professional profile
cv.qmd                      # CV (source of truth: assets/cv/*.pdf)
contact.qmd                 # contact
projects/                   # warfarin, theophylline, caffeine-pbpk,
                            #   acetaminophen-mbma, midazolam
assets/
  favicon.svg               # PB monogram + PK-curve favicon
  og-image.png              # 1200x630 social preview
  cv/Pramod_BR_Resume.pdf   # downloadable CV
  figures/<project>/*.png   # real analysis outputs from public repos
.github/workflows/publish.yml
```

## Deployment (GitHub Pages)

`.github/workflows/publish.yml` renders the site and publishes it to the `gh-pages`
branch on every push to `main`.

**GitHub → Settings → Pages → Build and deployment**

- Source: **Deploy from a branch**
- Branch: **gh-pages** · Folder: **/ (root)**

Project figures are self-hosted copies of outputs from the public analysis
repositories under [github.com/pbr26](https://github.com/pbr26).
