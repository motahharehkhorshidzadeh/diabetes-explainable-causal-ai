# Explainable and Causal Machine Learning for Diabetes Prediction

---

## Abstract

Early and accurate prediction of diabetes is a critical challenge in healthcare systems. Traditional machine learning models provide high predictive performance but often lack interpretability and causal understanding.

In this project, we propose an end-to-end framework for diabetes prediction using a Random Forest classifier combined with Explainable AI (SHAP) and causal inference techniques. The system not only predicts disease risk but also explains individual predictions and estimates treatment effects using propensity score methods.

---

## Keywords

Machine Learning, Explainable AI, SHAP, Causal Inference, Propensity Score, Healthcare, Diabetes Prediction

---

## 1. Introduction

Diabetes Mellitus is one of the most common chronic diseases worldwide. Early detection can significantly improve patient outcomes. However, clinical decision-making requires both predictive accuracy and interpretability.

This project addresses three key questions:

* Can we predict diabetes risk accurately?
* Why does the model make a specific prediction?
* Does treatment causally reduce disease risk?

---

## 2. Methodology

### 2.1 Data Processing

Patient data includes:

* Age
* BMI
* Glucose level
* Additional clinical features

Missing values are handled using statistical imputation techniques.

---

### 2.2 Machine Learning Model

A Random Forest classifier is used for diabetes prediction due to its:

* Robustness
* Non-linearity handling
* Feature importance extraction capability

---

### 2.3 Explainable AI (SHAP)

SHAP (SHapley Additive Explanations) is used to:

* Identify global feature importance
* Provide local explanations for individual predictions
* Improve clinical interpretability

---

### 2.4 Causal Inference

To estimate treatment effects beyond correlation, we use:

* Naive Average Treatment Effect (ATE)
* Propensity Score Modeling
* Inverse Probability Weighting (IPW)

These methods help correct selection bias and estimate causal impact.

---

## 3. Experimental Results

### 3.1 Model Performance

The model achieves strong predictive performance in classifying diabetes risk.

### 3.2 Explainability Results

SHAP analysis shows that:

* Glucose level is the most influential feature
* BMI and age also significantly contribute to predictions

### 3.3 Causal Analysis

* Naive ATE is biased due to confounding
* IPW provides a more reliable estimate
* Treatment is associated with reduced diabetes risk

---

## 4. Discussion

The integration of SHAP and causal inference enhances both transparency and reliability of machine learning models in healthcare settings.

This framework demonstrates that predictive models alone are insufficient for clinical decision-making without interpretability and causal reasoning.

---

## 5. Conclusion

This project presents a comprehensive AI system that combines:

* Predictive modeling
* Explainable AI
* Causal inference

for improved understanding and decision-making in diabetes prediction systems.

---

## 6. Future Work

* Integration with deep learning models
* Real-world clinical dataset validation
* Deployment as a clinical decision support system

---

## Author

Motahhareh Khorshidzadeh 
Machine Learning & Data Science

---
