# Diabetes Risk Analysis Based on Nutrition and Health Indicators

This project analyzes the relationship between nutritional and general health indicators and diabetes prevalence across multiple countries. It combines data from several sources, processes and merges them into a unified dataset, and trains a machine learning model to predict diabetes rates based on selected features.

---

## 📊 Objective

To identify key nutritional and health-related factors that influence the prevalence of diabetes (ages 20–79) across different countries, and to build an interpretable machine learning model capable of predicting diabetes rates using those indicators.

---

## 📁 Dataset Overview

Multiple datasets were collected from publicly available sources (e.g., WHO, FAO). These datasets include:

- Dietary indicators (e.g., energy, sugar, fat, vitamins, minerals)
- Health metrics (e.g., obesity rate, overweight rate, anemia)
- Demographic and population data
- Diabetes prevalence per country (target variable)

Before modeling, country names were standardized across all datasets to ensure proper merging. A pivot table was created to organize the data by country and indicator.

---

## ⚙️ Technologies Used

- **Python**
- **Google Colab**
- **Pandas** & **NumPy** – for data manipulation and analysis  
- **Scikit-learn** – for preprocessing, modeling (Random Forest, Isolation Forest), and evaluation  
- **SHAP** – for explaining feature contributions  

---

## 🧠 Modeling Approach

- Outliers were removed using **Isolation Forest** to improve model robustness.
- Features were selected based on their correlation with the target variable.
- A **Random Forest Regressor** was trained using **Leave-One-Out Cross-Validation** for reliable evaluation.
- Log transformation was applied to the target variable to normalize distribution.
- SHAP values were computed to interpret the model and rank feature importance.

---

## ✅ Results

- The model showed good predictive performance while remaining interpretable.
- Nutritional elements such as calories, sugar, and fat were found to have a strong positive association with diabetes prevalence.
- Other indicators, such as vitamin B6 intake and vegetable consumption, had a potential protective (negative) effect.
- Obesity and overweight prevalence were also strong predictors, confirming their medical relevance.



