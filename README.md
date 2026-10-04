# CodeML 2026
## Jadco challenge - Collection Équinoxe
Our task was to:
- estimate Collection Équinoxe’s 2026 rent increase using the history of six buildings in Québec and Ontario
- define the increase measured and justify method

To use the notebook, you must be added as one of the owners of GCP project. Feel free to reach out and we
will be happy to add you.

The libraries used are mostly the ones provided through Google Colab Entreprise. However, you do need to
install the tabpfn-client for our regression model. This also requires a (free!) api key, which we are also
happy to provide.

Other than the 4 datasets that Jadco provided us with, we also sourced floor plans from Jadco's website to
group individual units together, and we used data from StatCan and CMHC for macroeconomic indices. Our full
list of datasets can be found through https://console.cloud.google.com/storage/browser/codeml26 (must also
be authenticated).

## Backtest

| Year | Actual change | Predicted | Error (pts) | Model RMSE | Naive* RMSE |
|---|---|---|---|---|---|
| 2020 | 2.72% | 1.91% | −0.80 | 0.0319 | 0.0390 |
| 2021 | 3.75% | 2.83% | −0.92 | 0.0367 | 0.0427 |
| 2022 | 4.70% | 3.89% | −0.81 | 0.0404 | 0.0471 |
| 2023 | 2.17% | 4.54% | +2.37 | 0.0487 | 0.0557 |
| 2024 | 1.84% | 3.05% | +1.21 | 0.0488 | 0.0564 |
| 2025 | 3.82% | 3.71% | −0.12 | 0.0500 | 0.0630 |
| **Average 2023–2025** | **2.61%** | **3.77%** | **1.23** | **0.0492** | **0.0584** |
| **Average 2020–2025** | **3.17%** | **3.32%** | **1.04** | **0.0428** | **0.0507** |

*naive = last year's mean change.

Special thanks to Claude Code for generating the charts found in our notebook.
