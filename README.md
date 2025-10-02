# 🏠 House Price Prediction - Multiple Linear Regression

This project builds a predictive model to estimate **house sale prices** using numerical and categorical features.  
It demonstrates regression modeling, feature analysis, and diagnostics to ensure reliable predictions for real estate pricing strategies.

## 🔹 Project Overview
- Dataset: 1,460 house records with multiple features (Kaggle’s *House Prices: Advanced Regression Techniques*).
- **Exploratory Data Analysis (EDA):**
  - Correlation checks
  - Handling categorical and numerical variables
  - Multicollinearity check (Variance Inflation Factor - VIF)
- **Modeling:**
  - Built a Multiple Linear Regression model
  - Residual diagnostics to validate model assumptions
- **Results:**
  - R² = **0.83**
  - RMSE = **36,461.63**
  - MAE = **22,339.26**
  - Top predictors: `OverallQual`, `GrLivArea`, `GarageCars`

## 📊 Key Learnings
- Importance of checking multicollinearity in regression models.
- Residual analysis ensures valid model assumptions.
- Certain features strongly influence house prices, improving interpretability.

## 🛠️ Tech Stack
- Python (Pandas, NumPy, Scikit-learn, Statsmodels, Matplotlib, Seaborn)
- Jupyter Notebook

## 📂 Dataset
The dataset comes from [Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).  
Download it from Kaggle and place it in the `data/` folder before running the notebook.

```bash
data/house_prices.csv
