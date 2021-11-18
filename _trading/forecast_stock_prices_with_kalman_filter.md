---
title: "Kalman Filter & the Mean-Reverting Strategy"
---

If a stock price series is mean-reverting, we could trade on it and make a profit
if we could accurately estimate its means and standard deviations for the near
future. Kalman filter is an excellent algorithm for doing that. In this project,
we implemented a 1D Kalman Filter in Python to forecast the near-future mean 
prices of AAPL, AMZN, FB, GOOG, and TSLA stocks based on their daily close price 
and volume data between January 1 and August 6, 2021. We discovered that only 
TSLA showed a mean reverting pattern for this period. Our Kalman filter is smart 
enough to wait and see if a real trend develops before reflecting it in its 
forecasts. Read our [paper](/assets/stock-price-forecasting-with-kalman-filter.pdf)
to understand how Kalman filter works its magic.

![](/images/projects/forecast_stock_prices_with_kalman_filter/AAPL.png)

![](/images/projects/forecast_stock_prices_with_kalman_filter/AMZN.png)

![](/images/projects/forecast_stock_prices_with_kalman_filter/FB.png)

![](/images/projects/forecast_stock_prices_with_kalman_filter/GOOG.png)

![](/images/projects/forecast_stock_prices_with_kalman_filter/TSLA.png)