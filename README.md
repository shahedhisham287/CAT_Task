# CAT_Task

## Overview

This notebook focuses on analyzing and cleaning a dataset as part of a recruitment task. The main objectives are to ensure data integrity, extract meaningful insights, and prepare the dataset for further analysis or modeling. 

1. **Data Loading**: Importing the dataset and examining its structure.
2. **Data Cleaning**: Identifying and handling missing or incorrect values, removing duplicates, and ensuring consistency.
3. **Exploratory Data Analysis (EDA)**: Understanding data distributions, relationships, and patterns.
4. **Feature Engineering**: Creating and refining features to enhance analysis and predictive capabilities.
5. **Insights and Visualizations**: Highlighting key findings using visualizations and statistical summaries.

---
## Key Steps and Highlights

### 1. Data Exploration and Cleaning
- **Challenges Identified**: The dataset had several columns with unreliable values caused by incorrect or inconsistent data entry. These errors included:
  - Misspellings and inconsistent formats in categorical fields.
  - Out-of-range or missing values in numerical columns.
- **Resolution**:
  - Applied data cleaning techniques such as fuzzy matching, outlier detection, and imputation for missing values.
  - Ensured consistency in data formats and removed duplicates to maintain data integrity.

### 2. Feature Engineering
- Created new features to enhance the dataset's predictive capability.
- Engineered features based on domain knowledge to improve model performance.

### 3. Modeling and Evaluation
- **Models Tried**:
  - Random Forest
  - Decision Tree
  - Linear Regression
  - XGBoost
  - CatBoost
  - LightGBM
- **Final Model**: LightGBM was selected as the best-performing model due to:
  - Its ability to handle large datasets efficiently.
  - Faster training times compared to other boosting algorithms.
  - Achieving the lowest Mean Absolute Error (MAE) during evaluation.

### 4. Evaluation Metric: Mean Absolute Error (MAE)
- **Why MAE?**:
  - MAE measures the average magnitude of errors in predictions, providing a straightforward interpretation of the model's performance.
  - It is less sensitive to outliers than other metrics like Mean Squared Error (MSE), making it ideal for this dataset where data entry errors could introduce extreme values.

---

## Results and Insights

- Successfully cleaned and preprocessed the dataset, addressing all major issues.
- Derived actionable insights through exploratory data analysis and feature engineering.
- Identified LightGBM as the optimal model with the lowest MAE and fastest runtime.

---

## Requirements

To run this notebook, you need the following:
- Python 3.x
- Libraries: `numpy`, `pandas`, `seaborn`, `matplotlib`, `fuzzywuzzy`
- The dataset (`train.csv`) in the specified directory.

---

