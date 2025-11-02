# feature-engineering
Feature Engineering on Bank Marketing Dataset
# 🧩 Feature Engineering on Bank Marketing Dataset

## 📘 Overview
This project demonstrates how to apply **Feature Engineering** techniques to transform raw data into informative features using the **Bank Marketing Dataset** (UCI Repository).

The dataset predicts whether a bank client will subscribe to a term deposit (`y` = yes/no).

---

## 🧠 Feature Engineering Steps

### 1. Data Cleaning
- Checked for missing values and replaced `'unknown'` entries with the mode.
- Removed duplicates and standardized data types.

### 2. Encoding
- Applied **Label Encoding** for target variable `y`.
- Used **One-Hot Encoding** for categorical variables like `job`, `marital`, and `education`.

### 3. Feature Scaling
- Standardized all numeric columns using `StandardScaler` to ensure equal feature importance.

### 4. Feature Extraction
- Implemented **Principal Component Analysis (PCA)** to visualize data variance and reduce dimensionality.

### 5. Feature Selection
- Used **Variance Threshold** to remove low-variance features.
- Applied **SelectKBest (f_classif)** to select top 5 most important features for the target variable.

---

## 📊 Tools and Libraries
- Python  
- pandas, numpy  
- scikit-learn  
- matplotlib, seaborn  

---

## ⚖️ Ethical Considerations
Since the dataset includes sensitive attributes (e.g., age, marital status, job type), care was taken to avoid bias:
- Exclude sensitive variables if they cause discrimination.
- Apply fairness-aware modeling techniques.
- Maintain transparency in feature selection and data use.

---

## 📁 Files
- `bank.csv` – Original dataset  
- `feature_engineering_bank.ipynb` – Jupyter Notebook with full implementation  
- `README.md` – This file  

---

## 🏁 Outcome
The final dataset is fully preprocessed, encoded, scaled, and feature-selected, ready for model training or exploratory analysis.
