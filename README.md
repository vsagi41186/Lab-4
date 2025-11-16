#Lab 4
# Diabetes Disease Progression Prediction - Regression Models

## Purpose of the Lab Work

This lab explores the performance of various regression models to predict disease progression using the Diabetes dataset from sklearn. The goal is to evaluate Linear Regression, Multiple Regression, Polynomial Regression, Ridge Regression, and Lasso Regression models, applying them to understand their accuracy, behavior, and overfitting tendencies. The dataset contains several features related to patient health, and the target variable is disease progression.

## Models Implemented

- **Linear Regression**: A simple linear model that uses one or more features to predict the target variable.
- **Multiple Regression**: A linear model that utilizes multiple features to predict the target.
- **Polynomial Regression**: An extension of linear regression that uses polynomial features to model non-linear relationships.
- **Ridge Regression**: A linear model that uses L2 regularization to prevent overfitting.
- **Lasso Regression**: A linear model that uses L1 regularization, performing both regularization and feature selection.

## Model Evaluation and Results

### **Linear Regression**:
- **R²**: 0.233
- **MAE**: 52.26
- **RMSE**: 63.73
- Linear Regression performed poorly with a low R² value, indicating that the model explained only 23.3% of the variance in the target variable.

### **Multiple Regression**:
- **R²**: 0.453
- **MAE**: 42.79
- **RMSE**: 53.85
- Multiple Regression improved the model's performance, explaining 45% of the variance and reducing the error metrics compared to Linear Regression.

### **Polynomial Regression**:
- **R²**: 0.233
- **MAE**: 52.18
- **RMSE**: 63.75
- Polynomial Regression showed similar performance to Linear Regression, with similar error metrics, suggesting overfitting at higher polynomial degrees.

### **Ridge Regression**:
- **R²**: 0.419
- **MAE**: 46.14
- **RMSE**: 55.47
- Ridge Regression improved performance with regularization, though it was outperformed by Lasso.

### **Lasso Regression**:
- **R²**: 0.472
- **MAE**: 42.85
- **RMSE**: 52.90
- Lasso Regression showed the best performance, reducing overfitting and having the lowest error metrics. Its ability to perform feature selection also contributed to improved results.

## Key Insights

- **Lasso Regression** was the best-performing model overall, showing the highest R² and the lowest error metrics, while also handling overfitting effectively.
- **Multiple Regression** and **Ridge Regression** outperformed Linear and Polynomial Regression by incorporating more features and applying regularization techniques.
- **Polynomial Regression** showed a risk of overfitting, especially with higher-degree polynomials, and did not provide any significant improvement over Linear Regression.
- The results highlight the importance of **regularization** (Ridge and Lasso) in preventing overfitting and improving model performance.

## Conclusion

In this lab, we applied multiple regression techniques to predict disease progression in the Diabetes dataset. Lasso Regression demonstrated the best results due to its ability to handle overfitting and select relevant features. Ridge Regression and Multiple Regression also showed improvements over simpler models, while Polynomial Regression was prone to overfitting. Regularization techniques such as Lasso and Ridge are critical in improving model generalization and preventing overfitting.
