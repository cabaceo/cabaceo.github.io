---
title: "Generalized Estimating Equation & Power and Sample Size Calculation"
---

A research lab from a well-known American University approached us to analyze data from a pilot study on 77 mice of 2 genotypes and 3 age groups. The data included various cellular measurements collected between 1 and 5 cells per mouse.

We created box-plots of each cellular measure by genotype and age group, and computed the sample averages and the covariance structure.

Using Generalized Estimating Equation (GEE) with an exchangeable correlation structure for each cellular measure, we tested for differences in those measurements between genotypes within an age group, and between any two age groups within a genotype. This work was done in R with the geepack package.

We established a relationship between power and sample size for detecting a certain significant difference in some of the cellular measurements while controlling a 5% type I error. To do this, we modified a method described in the paper "Sample Size Calculations for Studies with Correlated Observations" (Biometrics 53, 937-947, September 1997).

Our GEE approach resulted publication of the study for the client. And the sample size and power relationship we arrived at allowed the client to design a bigger trial with statistical rigor and hence confidence.