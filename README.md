# Diabetes Prediction

A machine learning classification project that predicts whether a patient 
has diabetes based on demographic and medical information.

## Overview
- Dataset: Diabetes Prediction Dataset (Kaggle) — 100,000 patient records
- Features: age, gender, BMI, HbA1c level, blood glucose level, hypertension, 
  heart disease, smoking history
- Target: Diabetes (0 = Non-Diabetic, 1 = Diabetic)

## Workflow
- Data cleaning (duplicate removal) and encoding of categorical features
- Exploratory Data Analysis (age distribution, BMI outliers, class balance, correlations)
- Logistic Regression (SGDClassifier) trained over 20 epochs with train/validation/test split
- Applied class weighting to address dataset imbalance (~8.5% diabetic cases)

## Results
| Metric | Value |
|---|---|
| Accuracy | 89.1% |
| Recall | 87.4% |
| Precision | 44.0% |
| F1-Score | 58.5% |

The dataset is highly imbalanced, so recall (correctly identifying diabetic 
patients) was prioritized over raw accuracy — an important consideration in 
healthcare-related predictions.

## Tech Stack
Python, pandas, scikit-learn, matplotlib, seaborn

## How to Run
Open the notebook in Google Colab, upload `diabetes_prediction_dataset.csv` 
when prompted, and run all cells.

## Authors
Haila Alnashri · Ohoud Alzobidi · Alia Alnashri
