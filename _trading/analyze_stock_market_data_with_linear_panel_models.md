---
title: "Analyze Stock Market Data with Linear Panel Models"
---

The client, a stock trader and researcher, contracted us to analyze a collection of large files of stock market data using linear panel models with the R PLM package.

The provided stock market data were observed on cross-sections of units and over time. This double dimensionality required linear panel models for proper analysis and presented the following major challenges, which we solved beautifully.

1. Some data files were larger than the 16 GB RAM of our computers so we wrote code to read in the data chunk by chunk.
2. The data had complex structures. For example, limit order related fields were in one file, market quality related fields were in another, so were feasibility and participation related fields. Some fields had one observation per day, while others had multiple observations. We carefully joined the files and roll up the data by day, week and month, while creating different groups such as pre- and post- periods with respect to client specified dates.
3. The interpretation of the main effects and Differences-in-Differences (DID) effects from the linear panel models required careful study and deep understanding of the R PLM package, as well as an intimate knowledge of the created groups.

We built an easy-to-use pipeline in R for the client to prepare large and complex stock market data, run linear panel data modeling, and report analysis results with correct interpretations.