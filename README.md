# Healthcare-Analytics-Predicting-Patient-Length-of-Stay

This repository contains a healthcare analytics capstone project focused on **predicting patient Length of Stay (LOS)** using hospital admission data. Accurate LOS prediction helps healthcare providers allocate resources effectively, reduce patient risk, and optimize hospital operations.

---

## 🎯 Project Goal

To build predictive models that can estimate a patient’s Length of Stay (LOS) upon hospital admission, using both patient-level and hospital-level features. This can assist hospitals in optimizing bed usage, reducing infection risk, and enhancing care planning.

---

## 🔍 Problem Statement

Hospitals track various performance metrics, but **Length of Stay** is a critical one tied to costs, patient outcomes, and operational efficiency. Our project analyzes patient and hospital admission data to uncover key predictors and apply machine learning for classification of LOS into 11 categories.

---

## 🧪 Modeling Approach

We implemented three predictive models using Python:

### 1. **Naïve Bayes Classifier**
- Type: Probabilistic model
- Accuracy: **34.55%**
- Purpose: Baseline classifier for multi-class classification

### 2. **XGBoost Classifier**
- Type: Gradient Boosted Trees (ensemble method)
- Accuracy: **43.05%**
- Tuned with learning rate, regularization, and tree depth
- Delivered the highest performance among models

### 3. **Neural Network (Keras)**
- Architecture: 6 dense layers with ReLU activations and Softmax output
- Accuracy: **42.05%**
- Regularized using early stopping (limited to 4 epochs)
- Tracked training via TensorBoard

---

## 🔬 Data Overview

The dataset contains **318,000+ records** with 17 features related to:
- Admission type, severity, age, deposit amount
- Ward/facility codes, hospital region/type
- Visitor count, department, and more

Target variable: **`Stay`** (length of stay in 11 categorical levels from 0–10 days up to 100+ days)

---

## 🔧 Feature Engineering

- Filled missing values using mode imputation
- Encoded ordinal features using Label Encoding
- Engineered patient re-admission counts and ward/hospital visit patterns
- Split data into train/test using 80/20 ratio

---

## 📊 Results & Insights

| Model          | Accuracy |
|----------------|----------|
| Naïve Bayes    | 34.55%   |
| XGBoost        | 43.05%   |
| Neural Network | 42.05%   |

- **XGBoost outperformed** the other models in terms of prediction accuracy.
- LOS was most frequently predicted in the **21–30 days** range.
- Enhanced feature engineering improved all model performances.

---

## 🔮 Future Enhancements

- Integrate real-time data feeds for proactive resource planning
- Expand model with lab results and clinical notes (NLP)
- Incorporate wearable data and real-time vitals for risk modeling
- Use SHAP or LIME for explainability in model predictions

---

## 📌 Key Skills & Tools Used

- Python (Pandas, NumPy, Scikit-learn, XGBoost, Keras)
- SQL for preprocessing
- TensorBoard for monitoring neural network performance
- Label Encoding, Data Imputation
- Multiclass classification and model evaluation
- Jupyter Notebook for workflow development


---
