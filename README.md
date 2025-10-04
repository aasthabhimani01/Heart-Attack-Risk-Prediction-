# Heart Disease Risk Prediction – Logistic Regression Model

This repository contains the code and analysis accompanying the research paper:  
**_“Heart Attack Risk Prediction Using Logistic Regression and Risk Factor Modeling”_**  
Department of Statistics and Data Science, CHRIST (Deemed to be University), Bengaluru, India.

---

## Overview

This project develops a **clinically interpretable logistic regression model** for predicting heart disease risk using the publicly available [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease).

The study introduces a **1–5 scaling normalization scheme** and a **five-level risk stratification** framework that make the model’s outputs directly interpretable for clinical decision-making.
- **Proposed Model:** Applies 1–5 feature scaling, sigmoid-based risk computation, and five-tier risk classification.

---

## Features

- Data cleaning and preprocessing (encoding, imputation)
- Scaled and stratified logistic regression (1–5 range)
- Risk-factor computation using the sigmoid function
- Evaluation metrics: Accuracy, Precision, Recall, F1-Score, and AUC
- Visualization of correlations, confusion matrix, and ROC curve

## 📊 Model Performance

| Metric | Baseline Model | Proposed Scaled Model |
|:--|:--:|:--:|
| Accuracy | 76.5 % | **80.1 %** |
| Precision | 74.2 % | **78.3 %** |
| Recall | 82.0 % | **88.6 %** |
| F1-Score | 77.9 % | **83.1 %** |
| AUC | 77.5 % | **79.1 %** |

---

## 🧠 Methodology

1. **Data Preprocessing:**  
   Missing values imputed using median/mode strategies.  
   Categorical features encoded numerically or via one-hot encoding.

2. **Feature Scaling (Proposed Model):**  
   Continuous features normalized to a [1, 5] range for interpretability.

3. **Modeling:**  
   Binary logistic regression with L2 regularization (`C = 1.0`) implemented using scikit-learn.

4. **Evaluation:**  
   Performance assessed using confusion matrix, ROC curve, and standard classification metrics.

---

## 📂 Repository Structure

