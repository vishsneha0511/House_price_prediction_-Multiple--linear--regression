# 🏠 House Price Prediction using Regression Models

## 📌 Project Overview

This project focuses on predicting house prices using **Multiple Linear Regression**, **Ridge Regression**, and **Lasso Regression**. The objective is to build a robust regression model, evaluate key statistical assumptions, handle multicollinearity and heteroscedasticity, and compare regularized models against the classical linear regression approach.

The project emphasizes **statistical understanding + machine learning best practices**, making it suitable for academic evaluation as well as interview discussion.

---

## 🎯 Objectives

* Perform end-to-end regression modeling for house price prediction
* Validate key regression assumptions
* Address multicollinearity using Ridge and Lasso regression
* Compare models using **R², Adjusted R², RMSE, and MAE**
* Select the most appropriate model based on performance and interpretability

---

## 🗂 Dataset Description

* **Target Variable:** House Price
* **Features:** Mix of numerical and categorical variables related to property characteristics
* **Preprocessing:**

  * Missing value handling
  * Outlier detection
  * Log transformation of target variable
  * Categorical encoding using pipelines

---

## 🔧 Tools & Libraries Used

* Python
* NumPy, Pandas
* Matplotlib, Seaborn
* Scikit-learn
* Statsmodels
* SciPy

---

## ⚙️ Methodology

### 1️⃣ Exploratory Data Analysis (EDA)

* Distribution analysis
* Correlation analysis
* Outlier identification

### 2️⃣ Feature Engineering & Preprocessing

* Log transformation of the target variable
* Encoding categorical variables using pipelines
* Train-test split

### 3️⃣ Assumption Checking (Linear Regression)

The following assumptions were evaluated:

| Assumption          | Method Used                 | Observation                               |
| ------------------- | --------------------------- | ----------------------------------------- |
| Linearity           | Residual vs Fitted plot     | Mild non-linearity observed               |
| Normality of Errors | Q-Q Plot, Shapiro-Wilk Test | Test significant due to large sample size |
| Homoscedasticity    | Breusch-Pagan Test          | Heteroscedasticity detected               |
| Multicollinearity   | VIF Analysis                | High multicollinearity present            |

> Note: With large datasets, normality tests tend to be overly sensitive. Visual inspection showed approximate normality of residuals.

---

## 📊 Models Implemented

* Multiple Linear Regression
* Ridge Regression (L2 Regularization)
* Lasso Regression (L1 Regularization)

---

## 📈 Model Evaluation Metrics

* **R² Score**
* **Adjusted R²**
* **RMSE (Root Mean Squared Error)**
* **MAE (Mean Absolute Error)**

### 🔍 Final Model Comparison

| Model             | Train R² | Train Adj R² | Test R²    | Test Adj R² | Test RMSE | Test MAE  |
| ----------------- | -------- | ------------ | ---------- | ----------- | --------- | --------- |
| Linear Regression | 0.8854   | 0.8345       | **0.8147** | **0.7510**  | **39276** | **21341** |
| Ridge Regression  | 0.8566   | 0.8494       | 0.7985     | 0.7505      | 39309     | 21353     |
| Lasso Regression  | 0.8568   | 0.8495       | 0.7979     | 0.7497      | 39373     | 21431     |

---

## ✅ Key Insights

* Linear Regression achieved the **best predictive performance** on test data.
* Ridge Regression reduced model complexity and multicollinearity but slightly reduced accuracy.
* Lasso Regression performed feature shrinkage but resulted in information loss for this dataset.
* Regularization improved model stability rather than performance, indicating **no severe overfitting** in the baseline model.

---

## 🏆 Final Conclusion

Although classical regression assumptions were partially violated, Multiple Linear Regression demonstrated strong generalization ability and the highest test performance. Ridge and Lasso served as robustness checks, confirming that regularization was not strictly necessary for prediction, but valuable for model stability and interpretability.

The final selected model is **Multiple Linear Regression**, with Ridge Regression as a strong alternative when coefficient stability is prioritized.

---

## 🚀 Future Improvements

* Try Box-Cox transformation
* Apply robust regression techniques
* Explore tree-based and ensemble models (Random Forest, XGBoost)
* Perform cross-validation for hyperparameter tuning

---

## 👩‍💻 Author

**Sneha Vishwakarma**
M.Sc. Statistics (IIT Bombay)

---

⭐ If you find this project useful, feel free to star the repository!


## 📂 Dataset
The dataset comes from [Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).  
Download it from Kaggle and place it in the `data/` folder before running the notebook.

```bash
data/house_prices.csv
