## Simhaa T. T.

**Scientific ML researcher.** I take a measurement problem from some corner of
science, a leaf's reflectance spectrum, a cell's discharge curve, a microscope's
point spread function and work out what machine learning can *honestly* claim
about it.

The domain changes every time. What doesn't is the discipline: hold something
out, report the negative result, freeze the configuration, and ship code that
regenerates every number in the paper from deposited artifacts.

- **Currently:** Research student, Department of Electrical & Electronics
  Engineering, SSN College of Engineering, Chennai. Several manuscripts under
  review, with code and results public on GitHub and Zenodo.
- **Reach me:** [ORCID 0009-0006-9041-1103](https://orcid.org/0009-0006-9041-1103)

---

## Research

Different fields, one method: work out what the measurement can support, then
refuse to claim more than that.

| Field | Problem, and what came out of it | Artifact |
| --- | --- | --- |
| **Plant biochemistry**<br>[greenhyperspectra-compact-ssl](https://github.com/Simhaatt/greenhyperspectra-compact-ssl) | Predicting eight leaf traits from reflectance. **30 trait-specific bands beat all 1,721** (mean R² 0.624 vs 0.538) — and self-supervised pretraining, the fashionable answer, turned out to be complementary rather than superior. Reported with the failure: zero-shot transfer to a new acquisition source collapses, and 10–20% local labels only partly recover it. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22755275.svg)](https://doi.org/10.5281/zenodo.22755275) |
| **Optical physics**<br>[operator-mismatch-microscopy](https://github.com/Simhaatt/operator-mismatch-microscopy) | When a microscope's real optics drift from the ones a reconstruction model assumed, can you still bound the error? Two instruments, four reconstruction methods. Severe aberration raises true error up to **fivefold while the data-consistency residual goes down** — the diagnostic everyone trusts points the wrong way — and 90% coverage falls to 0.31. The one-sided coverage inequality survives every evaluated cell. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22750126.svg)](https://doi.org/10.5281/zenodo.22750126) |
| **Remote sensing**<br>[Graph-RMS](https://github.com/Simhaatt/Graph-RMS) | Finding coherent regions in hyperspectral scenes with no labels and no idea how many classes there are. Sparse reciprocal graph → damped diffusion → robust mean-shift modes → reference-free consolidation, held out on Trento. Reports that Leiden on the same graph is competitive, rather than claiming a universal win. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21876447.svg)](https://doi.org/10.5281/zenodo.21876447) |
| **Battery reliability**<br>[battery-moo-recursive-forecasting](https://github.com/Simhaatt/battery-moo-recursive-forecasting) | Forecasting capacity and resistance recursively, with architecture search given a matched budget against NSGA-II, NSGA-III and random search. **92.5% fewer parameters at statistically indistinguishable accuracy** — stated as a parameter result, not an accuracy breakthrough. 12,600-trial log included. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22057383.svg)](https://doi.org/10.5281/zenodo.22057383) |
| **Battery health**<br>[sparse-checkup-capacity-forecasting](https://github.com/Simhaatt/sparse-checkup-capacity-forecasting) | Forecasting a cell's capacity when it is measured only at occasional checkups. A square-root fade prior is fitted to each cell, and a gradient-boosted learner trained on other cells corrects its future error. Benchmarked on 228 Luh–Blank and 80 Sandia cells, then moved with no target labels to 21700 and pouch formats. Ships the leakage audit that removed resistance from the benchmark: an earlier join had attached future impedance to past rows. A 15-second CPU check regenerates 19 tables and 68 manuscript numbers. With B. Sivakumar. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23264760.svg)](https://doi.org/10.5281/zenodo.23264760) |
| **EV field data**<br>[DB-PatchKAN](https://github.com/Simhaatt/DB-PatchKAN) | Driver-aware battery stress modelling and capacity forecasting from real vehicles: one Nissan Leaf, nine RWTH vehicles, 191 EVBattery vehicles. On 9,714 next-capacity transitions, persistence-anchored KAN beats plain persistence by 0.009 Ah vehicle-macro MAE (95% CI 0.007–0.011). Stated as post-hoc, and not as a KAN win: only the KAN head got the selective policy, and TSLANet has the lower RMSE. With Aswathy B. Raj and K. V. Shihabudheen. | Source snapshot; DOI pending |
| **Reliability statistics**<br>[discret-hazard](https://github.com/Simhaatt/discret-hazard) | Where discrete-time hazard models stop being valid for lithium-ion cells: link choice against interval width, effective sample size spanning two orders of magnitude, first-passage against hazard models. `RESULTS.md` is generated from `results/`, so the prose and the numbers cannot drift apart. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22664399.svg)](https://doi.org/10.5281/zenodo.22664399) |
| **Survival theory**<br>[grouped-ph-reproducibility](https://github.com/Simhaatt/grouped-ph-reproducibility) | Separating the information lost by grouping survival times from the error introduced by reconstructing a Cox baseline afterwards: an exact finite-grid information-loss identity, a small-bin expansion, 34 frozen configurations across eight cohorts. With Sudheesh Kumar Kattumannil. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22347055.svg)](https://doi.org/10.5281/zenodo.22347055) |
| **Survival modelling**<br>[nestkan](https://github.com/Simhaatt/nestkan) | A discrete-time hazard model whose complementary log-log predictor nests the grouped Cox model, an additive spline model and a gated Kolmogorov–Arnold surface in covariates and time, so each added layer of flexibility is tested against the one below it. Every benchmark stage was pre-registered (protocols v5–v8) before its results were seen. With Sudheesh Kumar Kattumannil. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23434870.svg)](https://doi.org/10.5281/zenodo.23434870) |

Archived packages regenerate their reported tables and figures from deposited
artifacts — CPU, minutes, no dataset download, no model retraining. Badges are
concept DOIs, so they always resolve to the current version. DB-PatchKAN is a
public source snapshot and has not been archived yet.

## Systems

| Project | What it is |
| --- | --- |
| **[ocr](https://github.com/Simhaatt/ocr)** | 🏅 **National finalist — MOSIP hackathon, IIT Madras Shaastra 2025.** Document OCR, field mapping and fuzzy verification (PaddleOCR + FastAPI) wired into a MOSIP pre-registration flow: document-type-aware extraction, normalised fuzzy matching against the applicant's form, and per-field confidence a reviewer can correct. |
| **[money_muling_detection](https://github.com/Simhaatt/money_muling_detection)** | Money-mule detection over transaction graphs — PageRank, betweenness, cycle detection, Louvain communities and 72-hour smurfing windows behind a FastAPI + React app. [Live demo](https://money-muling-detection-backend.onrender.com/). |
| **[SONA](https://github.com/Simhaatt/SONA)** | **Final-year project (B.E. EEE, SSN) — Phase I complete.** Speech noise removal, with A. Rohit Daniel and Vijayaraghavan A. Phase I is the software system and its evaluation; Phase II moves the same model onto an embedded live microphone-to-headphone device. A 722k-parameter GTCRN predicts per-band gains and runs about 10× faster than real time on one laptop CPU core: +9.93 dB SI-SDR on the 824-clip VoiceBank-DEMAND test set, where every classical filter scored below the unprocessed input. Negative results kept: guarded online adaptation gives about zero gain, and enhancement raises Whisper's word error rate by 23–47%. Offline web app with nine methods side by side. |

## Toolbox

`Python` · `PyTorch` · `NumPy / SciPy` · `scikit-learn` · `NetworkX` ·
`Kolmogorov–Arnold networks` · `conformal prediction` · `survival analysis` ·
`gradient boosting` · `NSGA-II / NSGA-III` · `ONNX` ·
`FastAPI` · `TypeScript / React` · `pytest` · `LaTeX`

<!--
Keep this file honest and short. Update it when a paper lands or a repo changes
status; a stale profile README is worse than none.
-->
