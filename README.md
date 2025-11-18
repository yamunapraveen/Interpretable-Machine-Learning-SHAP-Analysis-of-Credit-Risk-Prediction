**Credit Risk Prediction with SHAP Explainability**

**Project Summary**
This project focuses on building an **interpretable Credit Risk Prediction System** using advanced machine learning algorithms and **SHAP explainability**.  
The goal is to accurately classify loan applicants as *high-risk (default)* or *low-risk (non-default)* while maintaining **transparency and interpretability** in model decisions.

Three models  **RandomForest**, **XGBoost**, and **LightGBM** — were trained and evaluated on the `credit_risk.csv` dataset.  
Among them, **XGBoost** delivered the best overall performance with:

**AUC:** 0.9499  
**Accuracy:** 0.9351  
**F1-score:** 0.8313  

The project integrates **SHAP (SHapley Additive Explanations)** to interpret both **global feature importance** and **local-level predictions**, enabling stakeholders to understand *why* the model makes certain decisions.

From a business perspective, the analysis highlights that **Debt-to-Income Ratio**, **Credit Utilization**, and **Late Payment History** are the strongest predictors of default.  
These insights can guide **credit policy improvements**, **loan risk segmentation**, and **responsible lending practices**.



**Models:** RandomForest + XGBoost + LightGBM  
**Explainability:** Global & Local SHAP Analysis  
**Dataset:** `credit_risk.csv`


**Project Overview**

This project implements an **end-to-end Credit Risk Prediction system** using advanced Machine Learning techniques and interpretable AI.  
The model predicts whether a loan applicant is likely to **default (1)** or **not default (0)**, while **SHAP (SHapley Additive exPlanations)** provides transparency on the model’s decision-making process.


**Expected Deliverables**

 **Code Implementation**
 Complete ML workflow in Python (see notebook/script)
 Includes:
    Data cleaning and preprocessing
    Model training and evaluation (AUC, F1-score, Precision, Recall)
    SHAP computation and visualization

 **Analytical Results**
 Model performance metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC
 Comparison of multiple models (RandomForest, XGBoost, LightGBM)

**SHAP Visualizations**

**Global Interpretability:**
   SHAP Summary Plot (feature importance)
   Dependence Plots for top drivers
**Local Interpretability:**
  Force/Waterfall plots for selected high-risk and low-risk applicants

**Textual Interpretations**
 Narrative on global SHAP results (feature-level insights)
 Local-level explanations for specific customer predictions

**Business Report**
 Executive summary of findings
 Key drivers affecting default risk
 Actionable recommendations for credit policy optimization


**Repository Structure**
 credit-risk-shap/
 README.md
 requirements.txt
 Final_Credit_Risk_SHAP_WithModels.ipynb
 credit_risk.csv
 project_output/
 models/
 figures/
 shap_feature_importance.csv
 report.md
 local_shap_high_risk.png
 local_shap_low_risk.png
 project_output.zip

 


**How to Run the Project**
1️⃣ Install Dependencies
pip install -r requirements.txt
pip install pandas numpy scikit-learn shap matplotlib joblib xgboost lightgbm

2️⃣ Run the Notebook
Open and execute the Jupyter Notebook:
jupyter notebook Final_Credit_Risk_SHAP_WithModels.ipynb

All generated results (models, metrics, figures, and reports) will appear in the project_output/ directory.

**Final Model Performance**
| Model            | AUC    | Accuracy | F1-Score |
| **RandomForest** | 0.9313 | 0.9313   | 0.8179   |
| **XGBoost**      | 0.9499 | 0.9351   | 0.8313   |
| **LightGBM**     | 0.9479 | 0.9357   | 0.8307   |



**Explainability Highlights**
**Global SHAP**
Top Predictive Features:
Debt-to-Income Ratio
Credit Utilization
Number of Late Payments
Monthly Income
Loan Amount

**Local SHAP**
High-Risk Applicant: High debt ratio and multiple past dues were main risk drivers.
Low-Risk Applicant: Low utilization and steady income contributed to low default probability.

**Business Insights**
Debt Ratio and Credit Utilization are the strongest indicators of borrower default.
Applicants with frequent late payments exhibit significantly higher risk.
SHAP explanations enhance model transparency for auditors and business stakeholders.
Feature-driven insights support policy updates and credit scoring thresholds.

**Tech Stack**
Language: Python 3.10+
Libraries: scikit-learn, XGBoost, LightGBM, SHAP, Pandas, NumPy, Matplotlib, Joblib
Environment: Jupyter Notebook / Python Script
Outputs: Figures, CSV, Markdown Reports, Saved Models



**Final Notes**

This project demonstrates a **complete, interpretable machine learning pipeline** for **credit risk prediction**, integrating **model performance** with **explainability** using SHAP.  
Among all tested models, **XGBoost** achieved the best performance with:
**AUC:** 0.9499  
**Accuracy:** 0.9351  
**F1-score:** 0.8313  
SHAP analysis revealed that **Debt-to-Income Ratio**, **Credit Utilization**, and **Late Payment History** are the most influential factors driving default predictions.  
The combination of **predictive power** and **explainability** ensures that the model’s insights are transparent, actionable, and aligned with responsible AI practices in credit decision-making.  
This work can serve as a **foundation for production-grade credit scoring systems**, academic research, or explainable AI demonstrations.








