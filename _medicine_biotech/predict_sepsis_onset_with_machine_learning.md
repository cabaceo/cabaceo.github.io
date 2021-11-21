---
title: "Predict Sepsis Onset with Machine Learning"
---

The client, Vivace Health Solutions, hired us to build machine learning models to predict the onset of sepsis and septic shock for adult and pediatric patients.

Using MIMIC-II and MIMIC-III ICU data, we trained and cross-validated the following machine learning models:

- Linear regression for modeling time trends,
- Logistic regression model with LASSO regularization,
- Linear discriminant analysis (LDA),
- Support vector machine (SVM) with radial kernel, and
- Cox proportional hazards model with LASSO regularization and time-varying covariates.

Our models demonstrated success at predicting septic event onset 72 hours in advance. Our models were integrated into the client's clinical decision support technology platform for use in an acute care environment.