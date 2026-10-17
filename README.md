## Simhaa T. T.

**Scientific ML researcher.** I take a measurement problem from some corner of
science, a leaf's reflectance spectrum, a cell's discharge curve, a microscope's
point spread function and work out what machine learning can *honestly* claim
about it.

The domain changes every time. What doesn't is the discipline: hold something
out, report the negative result, freeze the configuration, and ship code that
regenerates every number in the paper from deposited artifacts.

- **Currently:** Final-year B.E. in Electrical & Electronics Engineering at SSN
  College of Engineering, Chennai, and Diploma in Data Science and Applications
  at IIT Madras. Graduating 2027. Several manuscripts under review.
- **Reach me:** [simhaatt2006@gmail.com](mailto:simhaatt2006@gmail.com) ·
  [ORCID 0009-0006-9041-1103](https://orcid.org/0009-0006-9041-1103)

---

## Research

| Field | Problem → result | Artifact |
| --- | --- | --- |
| **Plant biochemistry**<br>[greenhyperspectra-compact-ssl](https://github.com/Simhaatt/greenhyperspectra-compact-ssl) | Eight leaf traits from reflectance. **30 trait-specific bands beat all 1,721** (mean R² 0.624 vs 0.538); zero-shot transfer to a new source collapses. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22755275.svg)](https://doi.org/10.5281/zenodo.22755275) |
| **Optical physics**<br>[operator-mismatch-microscopy](https://github.com/Simhaatt/operator-mismatch-microscopy) | Bounding reconstruction error when a microscope's optics drift from the model. Severe aberration raises true error **up to fivefold while the residual goes down**. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22750126.svg)](https://doi.org/10.5281/zenodo.22750126) |
| **Remote sensing**<br>[Graph-RMS](https://github.com/Simhaatt/Graph-RMS) | Unsupervised region discovery in hyperspectral scenes, with no class count given. Held out on Trento; Leiden on the same graph is reported as competitive. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21876447.svg)](https://doi.org/10.5281/zenodo.21876447) |
| **Battery reliability**<br>[battery-moo-recursive-forecasting](https://github.com/Simhaatt/battery-moo-recursive-forecasting) | Recursive capacity and resistance forecasting under matched-budget NSGA-II/III search. **92.5% fewer parameters** at statistically indistinguishable accuracy. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22057383.svg)](https://doi.org/10.5281/zenodo.22057383) |
| **Battery health**<br>[sparse-checkup-capacity-forecasting](https://github.com/Simhaatt/sparse-checkup-capacity-forecasting) | Capacity forecasts from sparse checkups: a square-root fade prior plus a gradient-boosted residual, tested on 308 cells and moved to new cell formats with no target labels. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23264760.svg)](https://doi.org/10.5281/zenodo.23264760) |
| **EV field data**<br>[DB-PatchKAN](https://github.com/Simhaatt/DB-PatchKAN) | Driver-aware battery stress and capacity forecasting on 191 real vehicles. Persistence-anchored KAN cuts MAE by 0.009 Ah over persistence (post-hoc). With A. B. Raj and K. V. Shihabudheen. | DOI pending |
| **Reliability statistics**<br>[discret-hazard](https://github.com/Simhaatt/discret-hazard) | Where discrete-time hazard models stop being valid for lithium-ion cells: link choice, interval width, sample size. Results report generated from the data. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22664399.svg)](https://doi.org/10.5281/zenodo.22664399) |
| **Survival theory**<br>[grouped-ph-reproducibility](https://github.com/Simhaatt/grouped-ph-reproducibility) | Separating information lost by grouping survival times from Cox baseline reconstruction error. Exact finite-grid identity; 34 frozen configurations. With S. K. Kattumannil. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22347055.svg)](https://doi.org/10.5281/zenodo.22347055) |
| **Survival modelling**<br>[nestkan](https://github.com/Simhaatt/nestkan) | A discrete-time hazard model that nests grouped Cox, an additive spline model and a gated KAN surface. Every benchmark stage pre-registered. With S. K. Kattumannil. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23434870.svg)](https://doi.org/10.5281/zenodo.23434870) |

Archived packages regenerate their tables and figures from deposited artifacts on
a CPU in minutes. Badges are concept DOIs, so they resolve to the current version.

## Systems

| Project | What it is |
| --- | --- |
| **[SONA](https://github.com/Simhaatt/SONA)** | **Final-year project, Phase I complete.** Offline speech noise removal: a 722k-parameter GTCRN, about 10× faster than real time on one CPU core, +9.93 dB SI-SDR on VoiceBank-DEMAND. Phase II moves it onto an embedded device. |
| **[ocr](https://github.com/Simhaatt/ocr)** | 🏅 **National finalist, MOSIP hackathon, IIT Madras Shaastra 2025.** Document OCR and fuzzy field verification (PaddleOCR + FastAPI) for MOSIP pre-registration. |
| **[money_muling_detection](https://github.com/Simhaatt/money_muling_detection)** | Money-mule detection over transaction graphs (PageRank, cycles, Louvain, smurfing windows), FastAPI + React. [Live demo](https://money-muling-detection-backend.onrender.com/). |

## Toolbox

`Python` · `PyTorch` · `NumPy / SciPy` · `scikit-learn` · `NetworkX` ·
`Kolmogorov–Arnold networks` · `conformal prediction` · `survival analysis` ·
`gradient boosting` · `NSGA-II / NSGA-III` · `ONNX` ·
`FastAPI` · `TypeScript / React` · `pytest` · `LaTeX`

<!--
Keep this file honest and short. Update it when a paper lands or a repo changes
status; a stale profile README is worse than none.
-->
