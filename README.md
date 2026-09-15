## Simhaa T. T.

Research student, Department of Electrical & Electronics Engineering,
**SSN College of Engineering, Chennai**. I work on machine learning for physical
and remote-sensing data, with a bias toward methods that are *reproducible by a
stranger*: frozen configs, deposited artifacts, and a one-command check that the
numbers in the paper are the numbers the code produces.

- **Interests:** hyperspectral imaging · graph-based and training-free methods ·
  survival and reliability modelling · uncertainty quantification
- **Currently:** four manuscripts under review, each with its code and results
  archived on Zenodo before submission
- **Reach me:** [ORCID 0009-0006-9041-1103](https://orcid.org/0009-0006-9041-1103)

---

## Research code

Every repository below is a reproducibility package for a specific manuscript.
Each ships the frozen configurations and curated results the paper reports, and
regenerates its tables and figures from deposited artifacts — on CPU, in minutes,
without redistributing third-party data. The DOI badge is the concept DOI, so it
always resolves to the current version.

### Hyperspectral imaging

| Project | What it is | Artifact |
| --- | --- | --- |
| **[Graph-RMS](https://github.com/Simhaatt/Graph-RMS)** | Training-free, class-count-free spectral–spatial region discovery. Sparse reciprocal graph → damped diffusion → robust mean-shift modes → reference-free consolidation. Nine scenes, Trento held out; Leiden on the same graph is reported as competitive. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21876447.svg)](https://doi.org/10.5281/zenodo.21876447) |
| **[greenhyperspectra-compact-ssl](https://github.com/Simhaatt/greenhyperspectra-compact-ssl)** | Band- and label-efficient plant-trait prediction. **30 trait-specific bands beat all 1,721** (mean R² 0.624 vs 0.538), and self-supervised pretraining turns out to be complementary rather than superior. Includes the negative result: zero-shot transfer to a new acquisition source fails, and a 10–20% local calibration set only partly recovers it. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22755275.svg)](https://doi.org/10.5281/zenodo.22755275) |

### Reliability and survival modelling

| Project | What it is | Artifact |
| --- | --- | --- |
| **[battery-moo-recursive-forecasting](https://github.com/Simhaatt/battery-moo-recursive-forecasting)** | Recursive LSTM forecasting of capacity and resistance under a matched-budget NSGA-II / NSGA-III / random-search comparison. Headline: **92.5% fewer parameters at statistically indistinguishable accuracy** — a parameter result, not an accuracy breakthrough. 12,600-trial search log included. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22057383.svg)](https://doi.org/10.5281/zenodo.22057383) |
| **[discret-hazard](https://github.com/Simhaatt/discret-hazard)** | Where discrete-time hazard models stop being valid for lithium-ion reliability: link choice against interval width, the spread of effective sample size, and first-passage against hazard models. `RESULTS.md` is generated from `results/`, so the prose and the numbers cannot drift apart. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22664399.svg)](https://doi.org/10.5281/zenodo.22664399) |
| **[grouped-ph-reproducibility](https://github.com/Simhaatt/grouped-ph-reproducibility)** | Separates the information lost by grouping survival times from the effects of reconstructing a Cox baseline after estimating coefficients: an exact finite-grid information-loss identity, a small-bin expansion, and 34 frozen configurations across eight cohorts. With Sudheesh Kumar Kattumannil. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22347055.svg)](https://doi.org/10.5281/zenodo.22347055) |

### Uncertainty quantification in computational imaging

| Project | What it is | Artifact |
| --- | --- | --- |
| **[operator-mismatch-microscopy](https://github.com/Simhaatt/operator-mismatch-microscopy)** | Do calibrated reconstruction-error bounds survive when the microscope's real optics differ from the ones the model assumed? Two instruments, four reconstruction methods, two photon regimes. Severe Zernike mismatch raises reconstruction error up to fivefold **while the data-consistency residual goes down**, and nominal 90% coverage falls to 0.31 — but the one-sided coverage inequality holds in every evaluated cell. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22750126.svg)](https://doi.org/10.5281/zenodo.22750126) |

## Applied / systems work

| Project | What it is |
| --- | --- |
| **[money_muling_detection](https://github.com/Simhaatt/money_muling_detection)** | Graph-based fraud detection over transaction networks — PageRank, betweenness, cycle detection, Louvain communities and temporal smurfing windows behind a FastAPI + React app. [Live demo](https://money-muling-detection-backend.onrender.com/). |
| **[ocr](https://github.com/Simhaatt/ocr)** | Document OCR, field mapping and fuzzy verification (PaddleOCR + FastAPI) wired to a MOSIP pre-registration flow. |

## Toolbox

`Python` · `PyTorch` · `NumPy / SciPy` · `scikit-learn` · `NetworkX` ·
`survival analysis` · `conformal prediction` · `NSGA-II / NSGA-III` · `FastAPI` ·
`TypeScript / React` · `pytest` · `LaTeX`

<!--
Keep this file honest and short. Update it when a paper lands or a repo changes
status; a stale profile README is worse than none.
-->
