# ExCellAtlas

**Live site: https://alex-chaoyang.github.io/ExCellAtlas/**

ExCellAtlas is the web portal that accompanies the manuscript

> Li, C. *A reproducible core of the cellular response to exercise and its confounding by sampling time.* Manuscript (2026).

It re-analyses every public single-cell and single-nucleus RNA-sequencing study of exercise with one pipeline (28 datasets, seven integrated tissues, mouse, human and pig), tests each dataset separately, and grades each cell-type–gene response by its consistency across independent studies.

## What the site offers

- **Overview** – the tissues in the atlas and the headline numbers.
- **Browse by tissue** – for each tissue and cell type, every graded gene with its pooled effect, heterogeneity and credibility tier.
- **Gene search** – for any of the 48,320 tested genes, where exercise raises or lowers it, pooled across studies and in each dataset.
- **Validation & time** – how the grades were tested on withheld datasets and on independent bulk-tissue meta-analyses, and how much of the response is attributable to the time of day at which tissue was sampled.
- **Biological meaning, exerkines, datasets, figures and methods.**

The interface is available in eleven languages: English, 简体中文, 繁體中文, 日本語, 한국어, العربية, Español, Français, Deutsch, Português and Русский.

## Repository contents

| Path | Content |
|---|---|
| `index.html` | the whole site (one page, no build step) |
| `data/excellatlas_portal_data.json` | graded tables, validation and sampling-time results |
| `data/genes/` | the gene index (`genes_meta.json`) and 200 shards with per-dataset results for every tested gene |
| `figs/` | figures of the manuscript |

The site is static: open `index.html` through any web server (for example `python -m http.server`) to run it locally.

## Data sources and licences

Expression data come from the Gene Expression Omnibus; the original studies are listed under *Datasets* on the site. The bulk-tissue references are from ExGrade (Li & Su, bioRxiv 2026, https://doi.org/10.64898/2026.11.06.764830). The body map is adapted from the EMBL-EBI Expression Atlas anatomogram (CC BY 4.0).

## Contact

Chaoyang Li, Beijing Sport University. Questions and corrections are welcome as issues in this repository.
