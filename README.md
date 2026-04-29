# From Prediction to Causality: Explainable Diabetes Risk Modeling with IPW

## 📌 Project Overview

This project focuses on predicting diabetes risk using machine learning and interpreting model decisions using explainability techniques. Additionally, it introduces causal inference concepts to move beyond correlation and toward understanding potential cause-effect relationships.

---

## 📊 Dataset

The dataset used is the **Pima Indians Diabetes Dataset**, which includes medical predictor variables such as:

* Glucose level
* BMI (Body Mass Index)
* Age
* Blood pressure
* Insulin level

Target variable:

* `Outcome` (0 = Non-diabetic, 1 = Diabetic)

---

## ⚙️ Project Pipeline

### 1. Data Preprocessing

* Handling missing values (replacing invalid zeros with median values)
* Basic data cleaning

### 2. Exploratory Data Analysis (EDA)

* Feature distribution analysis
* Correlation heatmap
* Target class balance

### 3. Model Training

* Model used: Random Forest Classifier
* Train-test split (80/20)

### 4. Model Evaluation

* Accuracy
* Precision, Recall, F1-score
* Confusion Matrix
* ROC-AUC Curve

### 5. Model Explainability

* SHAP (SHapley Additive exPlanations)
* Global feature importance (beeswarm plot)
* Local explanation (waterfall plot)

### 6. Causal Inference (Next Step)

* Defining treatment variables
* Estimating treatment effects (ATE)
* Propensity score methods

---

## 📈 Results

The model demonstrates solid performance in predicting diabetes risk. SHAP analysis shows that:

* Glucose is the most influential feature
* BMI and Age also contribute significantly

---

## 🧠 Key Insights

* Machine learning models can effectively predict diabetes risk
* Explainability tools help interpret predictions at both global and local levels
* Causal inference is required to move from correlation to actionable insights

---

## 🚀 Future Improvements

* Use additional models (XGBoost, Logistic Regression)
* Perform hyperparameter tuning
* Apply causal inference methods (matching, IPW)
* Deploy as a web app (Streamlit)

---

## 🛠️ Tech Stack

* Python
* Scikit-learn
* SHAP
* Pandas, NumPy
* Matplotlib, Seaborn

---

## 📎 How to Run

1. Open the notebook in Google Colab
2. Install dependencies:

   ```bash
   pip install shap
   ```
3. Run all cells

---

## 📬 Contact

For questions or collaboration, feel free to reach out.
