## Simhaa T. T.

**Scientific ML researcher.** I take a measurement problem from some corner of
science — a leaf's reflectance spectrum, a cell's discharge curve, a microscope's
point spread function — and work out what machine learning can *honestly* claim
about it.

The domain changes every time. What doesn't is the discipline: hold something
out, report the negative result, freeze the configuration, and ship code that
regenerates every number in the paper from deposited artifacts.

- **Currently:** Research student, Department of Electrical & Electronics
  Engineering, SSN College of Engineering, Chennai. Four manuscripts under
  review, each archived on Zenodo before submission.
- **Reach me:** [ORCID 0009-0006-9041-1103](https://orcid.org/0009-0006-9041-1103)

---

## Research

Six problems, five fields, one method: work out what the measurement can support,
then refuse to claim more than that.

| Field | Problem, and what came out of it | Artifact |
| --- | --- | --- |
| **Plant biochemistry**<br>[greenhyperspectra-compact-ssl](https://github.com/Simhaatt/greenhyperspectra-compact-ssl) | Predicting eight leaf traits from reflectance. **30 trait-specific bands beat all 1,721** (mean R² 0.624 vs 0.538) — and self-supervised pretraining, the fashionable answer, turned out to be complementary rather than superior. Reported with the failure: zero-shot transfer to a new acquisition source collapses, and 10–20% local labels only partly recover it. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22755275.svg)](https://doi.org/10.5281/zenodo.22755275) |
| **Optical physics**<br>[operator-mismatch-microscopy](https://github.com/Simhaatt/operator-mismatch-microscopy) | When a microscope's real optics drift from the ones a reconstruction model assumed, can you still bound the error? Two instruments, four reconstruction methods. Severe aberration raises true error up to **fivefold while the data-consistency residual goes down** — the diagnostic everyone trusts points the wrong way — and 90% coverage falls to 0.31. The one-sided coverage inequality survives every evaluated cell. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22750126.svg)](https://doi.org/10.5281/zenodo.22750126) |
| **Remote sensing**<br>[Graph-RMS](https://github.com/Simhaatt/Graph-RMS) | Finding coherent regions in hyperspectral scenes with no labels and no idea how many classes there are. Sparse reciprocal graph → damped diffusion → robust mean-shift modes → reference-free consolidation, held out on Trento. Reports that Leiden on the same graph is competitive, rather than claiming a universal win. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21876447.svg)](https://doi.org/10.5281/zenodo.21876447) |
| **Battery reliability**<br>[battery-moo-recursive-forecasting](https://github.com/Simhaatt/battery-moo-recursive-forecasting) | Forecasting capacity and resistance recursively, with architecture search given a matched budget against NSGA-II, NSGA-III and random search. **92.5% fewer parameters at statistically indistinguishable accuracy** — stated as a parameter result, not an accuracy breakthrough. 12,600-trial log included. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22057383.svg)](https://doi.org/10.5281/zenodo.22057383) |
| **Reliability statistics**<br>[discret-hazard](https://github.com/Simhaatt/discret-hazard) | Where discrete-time hazard models stop being valid for lithium-ion cells: link choice against interval width, effective sample size spanning two orders of magnitude, first-passage against hazard models. `RESULTS.md` is generated from `results/`, so the prose and the numbers cannot drift apart. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22664399.svg)](https://doi.org/10.5281/zenodo.22664399) |
| **Survival theory**<br>[grouped-ph-reproducibility](https://github.com/Simhaatt/grouped-ph-reproducibility) | Separating the information lost by grouping survival times from the error introduced by reconstructing a Cox baseline afterwards: an exact finite-grid information-loss identity, a small-bin expansion, 34 frozen configurations across eight cohorts. With Sudheesh Kumar Kattumannil. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22347055.svg)](https://doi.org/10.5281/zenodo.22347055) |

Every package regenerates its reported tables and figures from deposited
artifacts — CPU, minutes, no dataset download, no model retraining. Badges are
concept DOIs, so they always resolve to the current version.

## Systems

| Project | What it is |
| --- | --- |
| **[ocr](https://github.com/Simhaatt/ocr)** | 🏅 **National finalist — MOSIP hackathon, IIT Madras Shaastra 2025.** Document OCR, field mapping and fuzzy verification (PaddleOCR + FastAPI) wired into a MOSIP pre-registration flow: document-type-aware extraction, normalised fuzzy matching against the applicant's form, and per-field confidence a reviewer can correct. |
| **[money_muling_detection](https://github.com/Simhaatt/money_muling_detection)** | Money-mule detection over transaction graphs — PageRank, betweenness, cycle detection, Louvain communities and 72-hour smurfing windows behind a FastAPI + React app. [Live demo](https://money-muling-detection-backend.onrender.com/). |

## Toolbox

`Python` · `PyTorch` · `NumPy / SciPy` · `scikit-learn` · `NetworkX` ·
`conformal prediction` · `survival analysis` · `NSGA-II / NSGA-III` ·
`FastAPI` · `TypeScript / React` · `pytest` · `LaTeX`

<!--
Keep this file honest and short. Update it when a paper lands or a repo changes
status; a stale profile README is worse than none.
-->
