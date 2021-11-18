---
title: "Score Geographic Areas by Investment Potential"
---

The client, a multifamily real estate investor, contracted us to create a data-driven analytical system that scores certain geographic areas to show what areas have the highest investment potential for multifamily properties (apartment buildings).

The algorithm we developed for the client uses population density/growth, income growth, job growth, housing values/growth, rental prices/growth, rent-to-income ratio, rent-to-home-value ratio, crime rate, amongst other key metrics. These metrics were obtained and calculated from multiple data providers, including RentRage, CoStar, Zillow, and CubitPlanning. The algorithm assigns a score to each geographic area with the highest scores being the most optimal.

A key component of the algorithm is time series modeling, where trend, seasonal, cycle, and statistical features were carefully created and utilized in a linear regression to perform 1-step or n-step forecasts. For example, the following figures show the performance of a median-rent-forecaster for 1-bedroom apartments.

![](/images/projects/forecast_rent/next-month-forecast.png)
![](/images/projects/forecast_rent/next-12m-forecast.png)