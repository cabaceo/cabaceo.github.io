---
title: "Predict Sepsis Onset with Machine Learning"
---

The client, Vivace Health Solutions, Inc, contracted us to build machine learning models to predict the onset of sepsis and septic shock for adult and pediatric patients using the MIMIC-II and MIMIC-III ICU data.

The client was creating clinical decision support technology for use in an acute care environment. One of the goals they want to achieve was to successfully predict septic event onset or mortality x hours in advance, with x the bigger, the better. Using the MIMIC-II and MIMIC-III ICU data, we trained and cross-validated the following machine learning models:

- Multivariate regression for modeling time trends,
- Cox proportional hazards model with LASSO regularization and time-varying covariates,
- Logistic regression model with LASSO regularization,
- Linear discriminant analysis (LDA), and
- Support vector machine (SVM) with radial kernel.

Our models were integrated into the client's technology platform and are powering their products to this day.