# 🏥 Hospital Readmission Prediction with Explainable AI (XAI)

## **Project Overview**
This project focuses on predicting the 30-day readmission risk for diabetic patients using a dataset of **70,000+ clinical records** from US hospitals. The primary goal is to provide a high-performing predictive model while ensuring transparency through **Explainable AI (XAI)** techniques.

## **Technical Workflow**
- **Data Preprocessing:** - Handled missing values using **Median Imputation**.
  - Applied **Ordinal Encoding** for ranked features (e.g., Age groups, Test results).
  - Used **One-Hot Encoding** for nominal categorical features (e.g., Race, Gender).
- **Modeling:** Trained an **XGBoost Classifier** to handle complex non-linear relationships in the medical data.
- **Interpretability:** Integrated **SHAP** (Global Analysis) and **LIME** (Local Analysis) to explain model decisions, making the "Black Box" model understandable for healthcare professionals.

## **Key Results**
- **Model Performance:** Achieved an **AUC Score of 0.68**.
- **Top Feature:** `number_inpatient` (previous hospital visits) was identified as the most significant predictor of readmission.
- **XAI Insights:** SHAP summary plots reveal that age and medication count significantly influence the risk score across the population, while LIME provides patient-specific explanations for high-risk cases.

## **Tech Stack**
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, SHAP, LIME, Matplotlib
