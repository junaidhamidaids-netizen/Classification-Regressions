# Classification-Regressions
# Classification Assignment - Framingham Heart Disease Prediction

This project focuses on building an end-to-end Machine Learning classification pipeline to predict 10-year Coronary Heart Disease (CHD) risk using the Framingham Heart Disease dataset.

## 📌 Project Overview
- **Dataset:** Framingham Heart Disease (`framingham.csv`)
- **Target Variable:** `TenYearCHD` (Binary Classification)
- **Problem Type:** Imbalanced Medical Classification

## 🛠️ Key Pipeline Steps
1. **Data Preprocessing & Cleaning:**
   - Imputed missing values (`education`, `cigsPerDay`, `BPMeds`, `totChol`, `BMI`, `heartRate`, `glucose`) using Median strategy.
2. **Class Imbalance Handling:**
   - Applied **SMOTE** (Synthetic Minority Over-sampling Technique) on training data to balance class distribution.
3. **Feature Scaling:**
   - Standardized features using `StandardScaler`.
4. **Model Comparison:**
   - Evaluated Logistic Regression, Decision Tree Classifier, and Random Forest Classifier.
5. **Hyperparameter Tuning:**
   - Optimized Random Forest Regressor/Classifier using `GridSearchCV`.

## 📊 Results Summary
- **Tuned Model:** Random Forest Classifier
- **Accuracy:** ~81.77%
- **Best Hyperparameters:** `{'class_weight': 'balanced', 'max_depth': 15, 'min_samples_split': 2, 'n_estimators': 200}`

## 📁 Repository Structure
- `Classification_Assignment.ipynb` - Complete analysis & code
- `framingham.csv` - Dataset
- `README.md` - Documentation
