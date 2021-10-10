---
title: "Predict Default Risk of P2P Loans"
---

The client, Liquid P2P, LLC, was a start-up company that provided P2P loan liquidation services. The project involved analyzing the performance of P2P loan portfolios, pricing individual notes for listing on the secondary market, and building machine learning models to predict the default risk of the loans.

We built XGBoost models in R to predict the default risk of lending club loans at issuance on the primary market. Model training and cross validation were done using parallel computing on AWS. In addition, we built API services using the R plumber package to pass data between the database, the models, and the dashboard. We also analyzed loan life cycles and calculated the fair price of seasoned loans to be listed on the secondary market. Finally, we wrote technical white papers and content for marketing.

Our models consistently identified 2 ~ 5% more high quality notes across loan grades. Given a seasoned note, our pricing formula output prices that allowed quick and profitable sales on the secondary market.