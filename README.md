# RNA-Seq Cancer Type Classification

## Overview

This project implements an end-to-end machine learning pipeline for multi-class classification of high-dimensional gene expression data (~20,000 features per sample).

The objective is to build a scalable and reproducible workflow for classifying tumor samples into predefined cancer types using supervised learning techniques.

---

## Key Features

- Designed modular ML workflow across structured notebooks
- Built preprocessing pipeline for high-dimensional data
- Applied dimensionality reduction via cross-validated feature selection
- Trained and compared Logistic Regression and Random Forest models
- Evaluated models using stratified splitting and Macro F1-score

---

## Model Performance (Test Set)

**Logistic Regression**
- Accuracy: 99.38%
- Macro F1-score: 0.9947

**Random Forest**
- Accuracy: 98.76%
- Macro F1-score: 0.9893

---

## Technical Approach

### Data Preprocessing
- Data validation and duplicate removal
- Label encoding
- Log transformation for variance stabilization
- Low-variance feature filtering
- Feature standardization
- Stratified train-test split

### Feature Selection
- Cross-validation-based selection
- Reduced dimensionality from ~20,000 to ~5,000 features
- Leakage-safe workflow (training-only fitting)

### Modeling
- Logistic Regression (linear baseline model)
- Random Forest (ensemble model)
- Class-wise performance evaluation

---

## Repository Structure

rna-seq-cancer-classification/
│
└── notebooks/
├── 01_preprocessing.ipynb
├── 02_featureselection.ipynb
├── 03_modelselection.ipynb
├── 04_interpretation.ipynb
└── 05_results.ipynb

---

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Future Improvements

- Hyperparameter optimization
- Deployment-ready pipeline packaging
- Integration of additional datasets for robustness testing
- Exploration of advanced ensemble or deep learning approaches

---

## Author
Hemanti Mukherjea
M.Sc. Data Science
Technische Universität Braunschweig
