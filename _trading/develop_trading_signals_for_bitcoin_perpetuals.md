---
title: "Develop Trading Signals for Bitcoin Perpetual Future Contracts"
---

>It was an absolute pleasure to work with Guangming. Communication was seamless and he went above and beyond original expectations to provide excellence. You will be hard pressed to find a data scientist with this level of creative problem solving and efficiency. There is no problem too large. From fairly undeveloped ideas, he created a trading strategy yielding greater than 1% daily returns. I look forward to working together again.

The client, a technical trader, contracted us to develop trading signals for BTC perpetuals using statistics and machine learning. The client was already using two indicators to make trade decisions, and was looking for new signals to add in the mix.

Using tick data (open interest, funding rate, last price, mark price, and index price) from tardis.dev, we trained logistic regression models to forecast whether price would increase or decrease over the next candle period for 12-hour, 6-hour, 4-hour, 2-hour, 1-hour, 30-min, and 15-min periods respectively. The biggest challenge was feature engineering and selection, and we event built sub-models to capture local trends as features. After backtesting the models, we deployed them to a digital ocean cloud server, and had them output realtime trading signals to the client's google drive. In addition to those models, we also created ten indicators using order book L2 data from tardis.dev. These indicators measure the average and extreme buying and selling pressures for each candle period. They are very telling when correlated with price.

We used Python for historical data downloading and realtime data streaming via tardis API. We wrote shell scripts for data cleaning and size reducing. We used R for data preparation and visualization, feature engineering and selection, statistical analysis, and model training and backtesting.