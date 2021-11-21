---
title: "Analyze Stock Market Data with Linear Panel Models"
---

The client, a stock trader and researcher, asked us to analyze a collection of stock market data that were observed cross-sectionally and over time using linear panel models in R with the PLM package.

We wrote R code to read and preprocess the data chunk by chunk because some data files were larger than 16 GB.

The data had complex structures. For example, limit order, market quality, feasibility, and participation related fields existed in separate files and had different time frequencies. We carefully joined the files and rolled up the data by day, week and month, while creating different groups such as pre- and post- periods with respect to client specified dates.

We interpretated the main effects and Differences-in-Differences (DID) effects from the linear panel models. This required a deep understanding of the PLM package.

We built an easy-to-use pipeline in R for the client to process large and complex stock market data, run linear panel models, and report results with correct interpretations.