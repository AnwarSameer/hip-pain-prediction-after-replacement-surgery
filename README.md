# Hip Replacement Pain Prediction using PROMs (NHS Data)

This project applies machine learning to predict post-operative pain scores following hip replacement surgery using NHS England's 2021 PROMs (Patient Reported Outcome Measures) dataset.

The goal is to assist clinicians in identifying patients at risk of poor recovery outcomes and support shared decision-making using pre-operative patient-reported data and demographic features.

## 🔍 Problem Statement
Can we accurately predict a patient's pain score after surgery using only their pre-operative PROM responses and basic demographic data?

## 📊 Dataset
- Source: NHS Digital – PROMs CCG-Level Dataset (Hip Replacement, 2021)
- Outcome Variable: `Hip.Replacement.Post.Op.Q.Pain` (0 = severe pain, 4 = no pain)
- Features: Pre-operative PROM scores (OHS, EQ-5D), demographics (age, gender), comorbidities

## 🧠 Models Used
- Linear Regression
- Random Forest
- XGBoost (Best Performing)

## 📈 Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² (Variance Explained)

## 🧰 Tools & Libraries
- R (caret, xgboost, DALEX, ingredients, tidyverse)
- R Markdown (for analysis + report)
- Shiny (optional deployment for prediction UI)

## ✅ Key Findings
- XGBoost achieved the best performance.
- Most important features: Pre-op pain score, EQ-5D index, comorbidity score
- SHAP-style explanations were used to interpret model predictions both globally and locally.

## 📦 Deliverables
- Full R Markdown report (PDF & HTML)
- Feature engineering pipeline
- Model training, evaluation, and explainability
- Optional: Shiny app for clinicians to predict pain outcomes interactively

## 📚 References
- NHS Digital PROMs Data: https://digital.nhs.uk/data-and-information/publications/clinical-indicators/proms
- DALEX Package: https://modeloriented.github.io/DALEX/
