## Simhaa T. T.

Research student, Department of Electrical & Electronics Engineering,
**SSN College of Engineering, Chennai**. I work on machine learning for physical
and remote-sensing data, with a bias toward methods that are *reproducible by a
stranger*: frozen configs, deposited artifacts, and a one-command check that the
numbers in the paper are the numbers the code produces.

- **Interests:** hyperspectral image analysis · graph-based / training-free methods ·
  time-series forecasting for battery degradation · multi-objective optimisation
- **Currently:** preparing manuscripts on spectral-spatial region discovery and
  matched-budget multi-objective forecasting
- **Reach me:** [ORCID 0009-0006-9041-1103](https://orcid.org/0009-0006-9041-1103)

---

### Research code

| Project | What it is | Artifact |
| --- | --- | --- |
| **[Graph-RMS](https://github.com/Simhaatt/Graph-RMS)** | Training-free, class-count-free spectral–spatial region discovery in hyperspectral images. Sparse reciprocal graph → damped diffusion → robust mean-shift modes → reference-free consolidation. Nine scenes, Trento held out. | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21876447.svg)](https://doi.org/10.5281/zenodo.21876447) |
| **[battery-moo-recursive-forecasting](https://github.com/Simhaatt/battery-moo-recursive-forecasting)** | Recursive LSTM forecasting of capacity and resistance under a matched-budget NSGA-II / NSGA-III / random-search comparison. Headline: **92.5% fewer parameters at statistically indistinguishable accuracy** (12,600-trial log included). | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22067837.svg)](https://doi.org/10.5281/zenodo.22067837) |

Both repositories are built to be re-run by a stranger: the reported tables and
figures regenerate from deposited artifacts in minutes, on CPU, with no dataset
download and no model retraining (`python analysis/reproduce_all.py` in the
battery repository; `scripts/export_tables.py` and `scripts/generate_figures.py`
in Graph-RMS).

### Applied / systems work

| Project | What it is |
| --- | --- |
| **[money_muling_detection](https://github.com/Simhaatt/money_muling_detection)** | Graph-based fraud detection over transaction networks — PageRank, betweenness, cycle detection, Louvain communities and temporal smurfing windows behind a FastAPI + React app. [Live demo](https://money-muling-detection-backend.onrender.com/). |
| **[ocr](https://github.com/Simhaatt/ocr)** | Document OCR, field mapping and fuzzy verification (PaddleOCR + FastAPI) wired to a MOSIP pre-registration flow. |

### Toolbox

`Python` · `PyTorch` · `NumPy / SciPy` · `scikit-learn` · `NetworkX` · `FastAPI` ·
`NSGA-II / NSGA-III` · `TypeScript / React` · `pytest` · `LaTeX`
