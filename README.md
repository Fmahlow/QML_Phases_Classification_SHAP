# QML Phases Classification with SHAP
[![arXiv](https://img.shields.io/badge/arXiv-2408.00544-b31b1b.svg)]([https://arxiv.org/abs/2408.00544](https://arxiv.org/abs/2504.10673)) 

This repository contains the data and notebooks used in the study of phase classification in the ANNNI model with quantum machine learning techniques and SHAP for feature selection. The results are discussed in our [paper on arXiv](https://arxiv.org/abs/2504.10673).

## Repository structure

### Code notebooks
- `data_generation.ipynb` – Generates the datasets by computing observables of the ANNNI model.
- `QSVM_code.ipynb` – Quantum Support Vector Machine implementation for the phase classification task.
- ` VQC_code.ipynb` – Variational Quantum Classifier implementation for the phase classification task.
- `calculate_precision.ipynb` – Calculates accuracy of the models, based on the theoretical phase transitions.
- `plots.ipynb` – Contains scripts used to build the figures presented in the paper.

### Data files
- `8_sites_data.csv` – Dataset with observables for an eight‑site lattice.
- `12_sites_data.xlsx` – Dataset with observables for a twelve‑site lattice.
- `results_8_sites_VQC.csv` – Predictions of the VQC model for the eight‑site data.
- `results_8_sites_QSVM.csv` – Predictions of the QSVM model for the eight‑site data.
- `results_12_sites_VQC.csv` – Predictions of the VQC model for the twelve‑site data.
- `results_12_sities_QSVM.csv` – Predictions of the QSVM model for the twelve‑site data.
- `accuracy_vs_features_8_sites_new.csv` – Accuracy as a function of the number of features (eight‑site case).
- `accuracy_vs_features_12_sites.csv` – Accuracy as a function of the number of features (twelve‑site case).

The CSV result files store the grid values (\`g\` and \`k\`) alongside the predicted phase label for each model.

## Usage

Run the notebooks in the order listed above to reproduce the datasets, train the models and generate the plots. The notebooks were developed using Python and Qiskit.

