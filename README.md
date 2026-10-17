# Predicting Hypoxia in MCF7 Breast Cancer Cells

Classifies hypoxic vs. normoxic breast cancer cells using single-cell gene expression data (DropSeq and SmartSeq protocols), comparing performance across cell lines and sequencing platforms.

## Overview

Hypoxia (low oxygen) drives aggressive tumour behaviour and treatment resistance. This project builds machine learning classifiers on single-cell RNA-seq data to predict cellular hypoxic state, using feature selection and cross-protocol validation.

Datasets used:
- **DropSeq**: MCF7 and HCC1806 cell lines
- **SmartSeq**: MCF7 and HCC1806 cell lines (higher sensitivity, lower throughput)

## Notebooks

| Notebook | Description |
|---|---|
| `finalissimo.ipynb` | Final model and cross-platform evaluation |
| `MCF7_train.ipynb` | MCF7 DropSeq training and model selection |
| `AI_Lab_Code.ipynb` | Initial exploration and preprocessing pipeline |

## Methods

- Normalisation and filtering of high-dimensional gene expression matrices (3000 genes)
- Feature selection for biologically relevant genes
- Classification: logistic regression, random forest, SVM
- Cross-dataset generalisation evaluation

## Stack

Python · scikit-learn · pandas · NumPy · matplotlib
