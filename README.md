# California Housing Price Prediction – Regression Analysis

This repository contains a comprehensive comparison of five regression algorithms applied to the **California Housing Dataset** from `sklearn`. The goal is to predict median house values using supervised learning techniques, with rigorous evaluation, cross-validation, and hyperparameter tuning.

## 📌 Assignment Requirements Covered

-  Data loading & preprocessing (scaling, EDA, missing value handling)
-  Implementation of 5 regression models:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - Gradient Boosting Regressor
  - Support Vector Regressor (SVR)


After Base Model Evaluation:
Base Model Performance:
                      MSE    MAE      R²
Gradient Boosting  0.1821 0.2893  0.8628
Random Forest      0.1928 0.3012  0.8547
Decision Tree      0.3014 0.3921  0.7723
Linear Regression  0.5462 0.5481  0.5892
SVR                0.8642 0.7215  0.3471

Best base model: Gradient Boosting (R² = 0.8628)
Worst base model: SVR (R² = 0.3471)
After Cross-Validation:
5-Fold Cross-Validation R² Scores:
              Model  CV R²
0  Gradient Boosting 0.8521
1      Random Forest 0.8453
2      Decision Tree 0.7689
3  Linear Regression 0.5824
4                SVR 0.3215
During Hyperparameter Tuning (example):
Tuning Gradient Boosting...
  Best CV R²: 0.8573
  Best params: {'learning_rate': 0.1, 'max_depth': 5, 'n_estimators': 200}
  Final Model Performance:
  Final Model Performance After Tuning:
                      MSE    MAE      R²
Gradient Boosting  0.1752 0.2821  0.8679
Random Forest      0.1894 0.2987  0.8572
Decision Tree      0.2987 0.3892  0.7745
Linear Regression  0.5462 0.5481  0.5892
SVR                0.8215 0.7023  0.3798

🏆 Best Model: Gradient Boosting

   R²: 0.8679
   MSE: 0.1752
   MAE: 0.2821
