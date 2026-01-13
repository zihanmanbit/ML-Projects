# 🧠 Dopamine Overload Prediction

A machine learning–based project that predicts **dopamine overload risk** and **digital dependence levels** using digital lifestyle behavior and mental health indicators.

This project was developed as part of the **Artificial Intelligence Lab (CSE 422)** course and demonstrates a complete end-to-end ML pipeline including preprocessing, feature engineering, model training, evaluation and interpretability.

---

## 📌 Project Overview

In an increasingly digital world, excessive screen exposure, constant notifications and compulsive device usage can dysregulate the brain’s reward system — a phenomenon commonly referred to as **dopamine overload**.  
This project aims to **identify high-risk individuals early** using machine learning models trained on real-world digital behavior and mental wellness data.

---

## 🎯 Objectives

- Predict **dopamine overload risk** (`high_risk_flag`) using classification models
- Predict **digital dependence score** using regression
- Identify **key behavioral and psychological risk factors**
- Handle **class imbalance** effectively
- Provide **model interpretability** using feature importance and SHAP analysis

---

## 📐 Problem Formulation

- **Classification**  
  - Target: `high_risk_flag` (High risk vs. Non-risk)

- **Regression**  
  - Target: `digital_dependence_score`

---

## 🗂 Dataset

- **Name:** Digital Lifestyle Benchmark Dataset  
- **Source:** Kaggle / Hugging Face  
- **Size:** 3,500 samples × 24 features  
- **Data Types:** Numerical + Categorical  

### Includes:
- Device usage metrics
- Social media engagement
- Mental health indicators
- Demographic attributes

🔗 **Dataset links:**
- https://huggingface.co/datasets/tarekmasryo/digital-lifestyle-benchmark  
- https://www.kaggle.com/datasets/tarekmasryo/digital-health-and-mental-wellness  

---

## ⚙️ Methodology

### 1️⃣ Data Preprocessing
- No missing values or duplicates
- Feature scaling using **StandardScaler**
- Categorical encoding via **OneHotEncoder**
- Stratified train-test split (75% / 25%)

### 2️⃣ Feature Engineering
New features created:
- `screen_time_per_unlock`
- `notifications_per_hour`
- `mental_health_load`
- `mood_balance`

### 3️⃣ Handling Class Imbalance
- Applied **SMOTE** on training data
- Balanced high-risk vs non-risk classes

---

## 🤖 Models Used

### 🔹 Classification (High Risk Prediction)
- Logistic Regression
- K-Nearest Neighbors (kNN)
- Random Forest
- XGBoost Classifier ⭐
- Support Vector Machine (SVM)

### 🔹 Regression (Digital Dependence Score)
- Ridge Regression with Cross-Validation (`RidgeCV`)

---

## 📊 Results & Performance

### 🏆 Best Classification Model: **XGBoost**

| Metric | Score |
|------|------|
| Accuracy | **0.872** |
| Precision | **0.767** |
| Recall | **0.523** |
| F1-Score | **0.622** |

✔ Best balance for imbalanced data  
✔ Strong ROC-AUC and confusion matrix results  

---

### 📈 Regression Performance

| Metric | Value |
|------|------|
| MSE | **5.40** |
| R² Score | **0.97** |

✔ Explains 97% of variance  
✔ Strong linear fit with minimal residual error  

---

## 🔍 Feature Importance Insights

Top predictors of dopamine overload:
- `digital_dependence_score`
- `mental_health_load`
- `device_hours_per_day`
- `notifications_per_day`
- `stress_level`
- `anxiety_score`
- `sleep_quality`

📌 Interpretability done using:
- XGBoost feature importance
- SHAP value analysis

---

## 🔎 Technologies Used

- **Python**
- **Pandas, NumPy**
- **Scikit-learn**
- **XGBoost**
- **Imbalanced-learn (SMOTE)**
- **Matplotlib, Seaborn**
- **SHAP**

---

## 📁 Repository Structure

📦 Dopamine-Overload-Prediction  
 ├── Dopamine_Overload_Prediction.ipynb  
 ├── digital-lifestyle-benchmark-dataset.csv  
 ├── Dopamine-Overload-Prediction.pdf   
 ├── Dopamine_Overload_Prediction-Lab_Report.pdf     
 └── README.md  

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/zihanmanbit/ML-Projects.git
cd "ML-Projects/Dopamine Overload Prediction"
```

2. Install dependencies:
```bash
pip install numpy pandas scipy seaborn matplotlib scikit-learn imbalanced-learn xgboost shap
```

3. Run the notebook:
```bash
jupyter notebook Dopamine_Overload_Prediction.ipynb
```

---

## 🧩 Future Improvements

- Hyperparameter tuning and ensemble stacking
- Longitudinal (time-series) behavior analysis
- Real-time monitoring via mobile sensors
- Deployment as a web-based risk assessment tool
- Deeper causal inference and explainability

---

## 👨‍🎓 Author

**Zihan Manbit**  
_GitHub:_ https://github.com/zihanmanbit

---

## 📄 License

This project is for academic and research purposes only.  

---

_**⭐ If you find this project interesting, feel free to star the repository!**_
