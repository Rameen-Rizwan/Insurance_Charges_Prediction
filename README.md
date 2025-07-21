# Insurance Claim Amount Prediction

## Overview

This project aims to predict the insurance claim (medical charges) amount based on an individual’s personal and lifestyle features. The analysis is performed using the Medical Cost Personal Dataset, which includes variables such as age, sex, BMI, smoking status, number of children, and region.

The core objective is to build a regression model, analyze the relationship between key features and charges, and evaluate model performance using standard metrics.

---

## Objectives

- Estimate insurance charges using personal and lifestyle information
- Apply Linear Regression for modeling
- Visualize how features like age, BMI, and smoking status impact insurance costs
- Evaluate model performance using MAE and RMSE

---

## Dataset

- Dataset: Medical Cost Personal Dataset
- Source: [Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance) 
- Number of records: 1338
- Features include:
  - Age, sex, BMI, children, smoker, region
  - Target variable: `charges`

---

## Tools and Libraries Used

- Python
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

---

## Approach

- Imported and explored the dataset using pandas
- Checked for missing values (none found)
- Performed one-hot encoding on categorical features (`sex`, `smoker`, `region`)
- Defined features (`X`) and target (`charges`)
- Split the data into training and testing sets (80/20)
- Trained a Linear Regression model
- Evaluated performance using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE) and R²
- Visualized relationships between:
  - BMI and charges
  - Age and charges
  - Smoking status and charges

---

## Results

- The model was successfully trained and evaluated
- Evaluation metrics:
  - Mean Absolute Error (MAE): 4181.19
  - Root Mean Squared Error (RMSE): 5796.28
  - R² Score: 0.78
- A strong positive correlation was observed between:
  - Age and insurance charges
  - BMI and insurance charges (especially for smokers)
  - Smoking status had a significant impact on higher charges

---

## Key Insights

- Smoking status is a major factor contributing to higher insurance charges
- Age and BMI show strong linear relationships with charges
- The Linear Regression model explains approximately 78% of the variance in the target variable
- Some variance remains unexplained, suggesting potential for improvement using more advanced models

---

## Visualizations

- Scatter plots were used to show the trend of charges vs. BMI and age
- A box plot illustrated the impact of smoking status on insurance charges
- Residual analysis helped verify the model’s prediction behavior

---

## Possible Improvements

- Use advanced regression models like:
  - Polynomial Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Include interaction terms (e.g., smoker × BMI)
- Apply log transformation to normalize target distribution if skewed
- Perform hyperparameter tuning and cross-validation

---
