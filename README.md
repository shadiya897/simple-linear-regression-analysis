# simple-linear-regression-analysis
Simple Linear Regression on multiple datasets using R

## Overview of Work

In this project, simple linear regression was applied to multiple real-world datasets using R. The workflow included:

- Data loading and inspection  
- Checking for missing values and structure  
- Correlation analysis using matrices and heatmaps  
- Splitting data into training and testing sets  
- Building regression models using `lm()`  
- Evaluating models using MAE, RMSE, and R²  
- Visualizing results using scatter plots with regression lines  

The analysis was performed on five datasets:
Boston Housing, Diabetes, Auto MPG, Advertising, and Housing datasets.

---

## Results and Interpretation

### 1. Boston Housing Dataset (medv ~ rm)

**Output:**
- Intercept = -35.2069  
- Slope (rm) = 9.1916  
- R² ≈ 0.48  
- RMSE ≈ 6.04  

**Interpretation:**
There is a moderate positive relationship between number of rooms and house price. For every additional room, the price increases by approximately 9.19 units. However, the R² value indicates that other variables also influence house prices.

---

### 2. Diabetes Dataset (BMI ~ Insulin)

**Output:**
- Intercept ≈ 30.96  
- Slope (Insulin) ≈ 0.012  
- R² ≈ 0.03  
- RMSE ≈ 7–8  

**Interpretation:**
The model shows a very weak relationship between insulin and BMI. The low R² indicates poor explanatory power, and the model is not suitable for prediction.

---

### 3. Auto MPG Dataset (mpg ~ weight)

**Output:**
- Intercept ≈ 46.73  
- Slope (weight) ≈ -0.0077  
- R² ≈ 0.69  
- RMSE ≈ 4.35  

**Interpretation:**
A strong negative relationship exists between weight and fuel efficiency. As weight increases, mpg decreases. This model performs well and provides reliable predictions.

---

### 4. Advertising Dataset (Sales ~ TV)

**Output:**
- Intercept ≈ 7.03  
- Slope (TV) ≈ 0.0475  
- R² ≈ 0.81  
- RMSE ≈ 2.28  

**Interpretation:**
There is a strong positive relationship between TV advertising and sales. This model has the highest R² and lowest error, making it the best-performing model in this analysis.

---

### 5. Housing Dataset (median_house_value ~ median_income)

**Output:**
- Intercept ≈ 44918  
- Slope (median_income) ≈ 41830  
- R² ≈ 0.47  
- RMSE ≈ 83000+  

**Interpretation:**
The model shows a moderate relationship between income and house value. While income is an important predictor, the high RMSE indicates large prediction errors.

---

## Conclusion

This analysis demonstrates that the performance of simple linear regression depends on the strength of the relationship between variables.

- Strong relationships (Advertising, Auto) produce accurate models  
- Weak relationships (Diabetes) lead to poor predictions  
- Moderate models (Boston, Housing) indicate the need for additional predictors  

Overall, this highlights the importance of:
- Interpreting regression coefficients  
- Evaluating models using R² and RMSE  
- Selecting appropriate variables  

It also shows that simple linear regression is useful for initial analysis but may not be sufficient for complex real-world data.
