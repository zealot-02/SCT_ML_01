# Kaggle - House Prices: Advanced Regression Techniques

Welcome to my solution for the [Kaggle House Prices](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) competition — a supervised regression task aimed at predicting home sale prices using advanced feature analysis and modeling techniques.

---

## Problem Statement

The goal is to accurately predict the final sale price of homes in Ames, Iowa, based on 79 explanatory variables describing various aspects of residential houses (e.g., area, quality, year built, neighborhood). This problem emphasizes real-world challenges like:
- Handling missing data
- Dealing with mixed data types (numerical + categorical)
- Preventing overfitting
- Building robust ML pipelines

---

## Approach Overview

### Data Preprocessing
- Filled missing numerical values with column means
- Replaced missing categorical values with `"None"`
- Applied **Label Encoding** to transform categorical features into numerical form

### Modeling
- Used **XGBoost Regressor** for its efficiency and handling of non-linear relationships
- Parameters used:
  - `n_estimators=1000`
  - `learning_rate=0.05`
- No log transformation or advanced hyperparameter tuning applied (baseline model)

### Evaluation
- Used Kaggle's leaderboard (log RMSE) to measure model performance
- Generated `submission.csv` formatted according to Kaggle requirements

---

## Repository Structure

house-prices-kaggle/
├── house_prices_model.ipynb # Main notebook with preprocessing, modeling, submission generation
├── submission.csv # Output file ready for Kaggle submission
├── README.md # Project documentation
└── (train.csv/test.csv) # Not included — must be downloaded from Kaggle

---

## Tools and Libraries

- **Python 3.8+**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Scikit-learn** – Preprocessing & evaluation
- **XGBoost** – Gradient boosting regressor
- **Jupyter Notebook** – Interactive development

---

## Competition Link

📎 [Kaggle Competition: House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

## Connect with Me

If you have feedback or want to collaborate on similar ML projects, feel free to connect on [LinkedIn](https://www.linkedin.com/in/sujithkamal-katta-ba6a63338/) or fork this repo.

Thankyou for visiting!

---