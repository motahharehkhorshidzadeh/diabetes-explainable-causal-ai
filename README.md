# 🧠 Explainable & Causal AI for Diabetes Prediction

## 📌 Overview

This project builds an end-to-end machine learning system for predicting diabetes and understanding the underlying factors behind predictions.

Unlike traditional models, this system not only predicts disease risk but also explains decisions and estimates causal effects of treatments.

---

## 🔬 Problem Statement

Early detection of diabetes is critical in healthcare.
This project aims to:

* Predict diabetes risk using patient data
* Explain model decisions (Why this prediction?)
* Estimate causal effects (Does treatment actually work?)

---

## 🧠 Methods Used

### 🤖 Machine Learning

* Random Forest Classifier
* Train/Test Split
* Model Evaluation (Accuracy, Confusion Matrix)

---

### 📊 Explainable AI (SHAP)

* Global feature importance (Which features matter most?)
* Local explanations (Why this patient is high risk?)

---

### ⚖️ Causal Inference

* Naive ATE (baseline)
* Propensity Score Modeling
* Inverse Probability Weighting (IPW)

---

## 📁 Project Structure

```
diabetes-explainable-causal-ai/
│
├── data/
├── notebooks/
│   ├── 01_preprocessing.ipynb
│   ├── 02_model.ipynb
│   ├── 03_shap.ipynb
│   └── 04_causal.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── model.py
│   ├── shap_utils.py
│   └── causal.py
│
├── results/
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   ├── shap_summary.png
│   └── shap_patient_0.png
│
├── requirements.txt
└── README.md
```

---

## 📊 Results

### ✔ Model Performance

* Accurate classification of diabetes risk
* Evaluated using confusion matrix and accuracy score

### ✔ Explainability

* SHAP identifies key features such as glucose, BMI, and age
* Provides patient-level explanations

### ✔ Causal Insights

* Naive ATE is biased
* IPW provides adjusted treatment effect
* Treatment reduces diabetes risk

---

## 📸 Visualizations

### Confusion Matrix

![Confusion Matrix](results/confusion_matrix.png)

### Feature Importance

![Feature Importance](results/feature_importance.png)

### SHAP Summary

![SHAP Summary](results/shap_summary.png)

### Patient Explanation

![SHAP Patient](results/shap_patient_0.png)

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Run notebooks in order:

   * Data preprocessing
   * Model training
   * SHAP explainability
   * Causal inference

2. Outputs will be saved in the `results/` folder

---

## 🎯 Key Contributions

* End-to-end ML pipeline
* Explainable AI integration (SHAP)
* Causal inference for treatment effect
* Patient-level interpretability

---

## 🧠 Conclusion

This project demonstrates how machine learning can go beyond prediction by providing explanations and causal insights.

It highlights the importance of combining:

* Predictive modeling
* Explainability
* Causal reasoning

---

## 👨‍💻 Author

Motahhareh Khorshidzadeh
Machine Learning / Data Science

---
