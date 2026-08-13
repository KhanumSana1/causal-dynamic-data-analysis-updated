# Causal Dynamic Data Analysis

Notebooks and datasets for analyzing causal relationships in non-stationary / dynamic time series data, using both real-world and synthetically generated data.

## Repository Structure

```
causal-dynamic-data-analysis/
├── Real World Dataset/
│   ├── AA_RSTE_ATP_mean_all_60_final_3_6_ea_new.ipynb
│   │   Causal analysis notebook applied to real-world time series data
│   │   (ATP mean measurements).
│   ├── Copy_of_AA_RSTE_ATP_mean_all_60_final_3_6_ea_new.ipynb
│   │   Working copy of the above analysis notebook.
│   ├── Results_Metabolites_Enzymes_Sana.xls
│   │   Real-world metabolite and enzyme measurement results.
│   └── Results_cytokines_1.xls
│       Real-world cytokine measurement results.
│
├── Synthetic Data/
│   ├── Bidirectional/
│   │   ├── Plot_synthetic_data_bidirectional_share.ipynb
│   │   │   Visualization of bidirectional synthetic causal datasets.
│   │   ├── Synthetic_data_bidirectional_run_results.ipynb
│   │   │   Generation and analysis of bidirectionally causal synthetic
│   │   │   time series.
│   │   ├── correlation_12.xlsx, correlation_12_1.xlsx
│   │   │   Correlation results/tables from bidirectional trials.
│   │   └── Efficient_Paper_Synthetic_Data_1.xlsx, _1_1.xlsx,
│   │       Efficient_Paper_Synthetic_Data_2.xlsx, _2_1.xlsx
│   │       Synthetic datasets used in the bidirectional experiments.
│   │
│   └── Unidirectional/
│       ├── Plot_synthetic_data_uni_share.ipynb
│       │   Visualization of unidirectional synthetic causal datasets.
│       ├── Synthetic_data_unidirectional_run_results.ipynb
│       │   Generation and analysis of unidirectionally causal synthetic
│       │   time series.
│       ├── correlation_12.xlsx, correlation_12_1.xlsx, correlation_12_3.xlsx
│       │   Correlation results/tables from unidirectional trials.
│       └── Efficient_Paper_Synthetic_Data_1.xlsx, _1_1.xlsx, _1_3.xlsx,
│           Efficient_Paper_Synthetic_Data_2.xlsx, _2_1.xlsx, _2_3.xlsx
│           Synthetic datasets used in the unidirectional experiments.
│
└── README.md
```

## Overview

This repository accompanies work on causal discovery / causal inference in dynamic (time-varying, non-stationary) systems. It includes:

- **Real-world dataset analysis**: causal-relationship notebooks applied to measured ATP time series data.
- **Synthetic data generation & analysis**: controlled experiments with known ground-truth causal structure (including AR processes, non-stationary and nonlinear bidirectional causality), used to validate the causal analysis methodology before applying it to real data.
- **Visualization notebooks**: plotting utilities for inspecting both univariate and bivariate synthetic causal series.

## Requirements

The notebooks primarily rely on:

```
numpy
pandas
matplotlib
statsmodels
openpyxl
```

Install with:

```bash
pip install numpy pandas matplotlib statsmodels openpyxl
```


## Notes

- Some notebook files are large as they contain embedded plot outputs.
- `.xlsx` files under `Synthetic Dataset/` and `Real world Dataset/` contain the relevant python notebooks
.

## License

Add a license of your choice (e.g., MIT) if you intend this repository to be reused by others.
