🧠 From Prediction to Causality: Explainable Diabetes Risk Modeling
📌 Overview

This project combines Machine Learning, Explainable AI, and Causal Inference to analyze the relationship between obesity and diabetes risk using the Pima Indians Diabetes dataset.

Unlike traditional predictive models, this project goes beyond correlation and estimates causal effects using advanced econometric techniques such as Inverse Probability Weighting (IPW) and Doubly Robust Estimation (DR).

🎯 Objectives
Build a machine learning model to predict diabetes risk
Interpret model decisions using SHAP explainability
Move beyond prediction to estimate causal effects
Quantify the impact of obesity (BMI > 30) on diabetes
Compare naive vs adjusted causal estimates
📊 Dataset

Pima Indians Diabetes Dataset

Features include:

Pregnancies
Glucose
Blood Pressure
Skin Thickness
Insulin
BMI
Diabetes Pedigree Function
Age

Target:

Outcome (0 = Non-diabetic, 1 = Diabetic)
⚙️ Methodology
1. Data Preprocessing
Handled missing/invalid values (zeros replaced with median)
Cleaned dataset for modeling
2. Exploratory Data Analysis (EDA)
Feature distributions
Correlation analysis
Target imbalance check
3. Machine Learning Model
Model: Random Forest Classifier
Evaluation metrics:
Accuracy
Precision / Recall / F1-score
ROC-AUC
4. Model Explainability (SHAP)
Global feature importance analysis
Local explanations for individual predictions
Key finding:
Glucose is the most influential predictor
BMI and Age also strongly contribute
🧠 Causal Inference Framework
📌 Treatment Definition

Obesity is defined as:

BMI > 30

📌 Propensity Score Modeling

A logistic regression model estimates the probability of being obese given confounders:

Age
Glucose
Blood Pressure
Insulin
Pregnancies
Diabetes Pedigree Function
📌 Inverse Probability Weighting (IPW)

IPW is used to adjust for confounding and estimate the causal effect:

Naive ATE: simple difference in means
IPW ATE: confounder-adjusted estimate
📌 Doubly Robust Estimation (DR)

A hybrid approach combining:

Outcome regression model
Propensity score weighting

This ensures consistency if either model is correctly specified.

📈 Results
Method	Estimated Effect of Obesity on Diabetes
Naive ATE	Biased estimate
IPW ATE	Adjusted causal effect
Doubly Robust ATE	Most robust estimate
Key Insight:

Obesity shows a positive causal effect on diabetes risk across all methods.

🔍 Key Insights
Machine learning models are effective for prediction but do not imply causation
Obesity significantly increases diabetes risk even after adjusting for confounders
Causal inference methods reduce bias from observational data
Doubly Robust estimation provides the most reliable effect estimate
🧪 Causal Assumptions

This analysis assumes:

No unmeasured confounding
Positivity (overlap condition holds)
Correct specification of at least one model (IPW or outcome model)
📊 Technologies Used
Python
Pandas, NumPy
Scikit-learn
SHAP
Matplotlib, Seaborn
🚀 How to Run
Clone repository
Install dependencies:
pip install shap scikit-learn pandas numpy matplotlib seaborn
Run notebook step by step in Jupyter / Colab
📌 Project Highlights
End-to-end ML + Causal Inference pipeline
Explainable AI using SHAP
IPW and Doubly Robust estimation
Transition from prediction → causation
Healthcare-focused real-world dataset
📬 Future Improvements
Add confidence intervals via bootstrap
Use XGBoost / causal forests
Perform sensitivity analysis for unmeasured confounding
Deploy as interactive Streamlit app
🧠 Summary

This project demonstrates that:

Predictive accuracy is not enough — understanding causality is essential for real-world decision making.
