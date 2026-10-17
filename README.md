# Predicting Hypoxia in MCF7 Breast Cancer Cells

Classifies hypoxic vs. normoxic breast cancer cells from single-cell RNA-seq data (DropSeq and SmartSeq), comparing model performance across cell lines and sequencing protocols.

## Overview

Hypoxia drives aggressive tumour behaviour and treatment resistance. This project builds supervised classifiers on high-dimensional single-cell gene expression data (3000 selected genes), using dimensionality reduction and statistical feature selection.

Datasets:
- **DropSeq**: MCF7 and HCC1806 cell lines
- **SmartSeq**: MCF7 and HCC1806 cell lines

## Notebooks

| Notebook | Description |
|---|---|
| `finalissimo.ipynb` | Full pipeline: EDA, QC, PCA, t-SNE, k-means, t-test feature selection, classification |
| `MCF7_train.ipynb` | MCF7 DropSeq training experiments |
| `AI_Lab_Code.ipynb` | Initial exploration and preprocessing pipeline |

## Methods

**Preprocessing & EDA**
- Quality control: filtering low-count cells, removing duplicates, sparsity analysis
- Normalisation of read counts

**Dimensionality Reduction & Clustering**
- PCA and t-SNE for visualisation
- k-means clustering to explore cell groupings

**Feature Selection**
- t-test to identify statistically significant differentially expressed genes between hypoxic and normoxic cells

**Classification**
- Logistic Regression
- SVM / Linear SVC
- KNN
- Feature scaling with `StandardScaler` applied to distance-based models

## Stack

Python · scikit-learn · pandas · NumPy · matplotlib · seaborn · UMAP
