---
title: "Estimate TV Attribution with Wavelets"
---

The client, Metrics Media Group, LLC, runs TV ad campaigns for its customers. They contracted us to develop a methodology of attribution to help them understand which TV station-ad-spots provide the most web traffics so that they can better allocate their ads spendings.

They provided us with a dataset of minute-level web sessions tracked by Google Analytics (GA), and a log file of TV spots data (airtime, TV station, and spot rate). The first challenge was to estimate how web traffics would have evolved after a spot if the spot had never occurred, known as the baseline estimation problem or the counterfactual prediction problem. To solve this, we tried three methods on the minute-level GA sessions data: 95% trimmed mean, simple moving average, and Discrete Wavelet Transform (DWT). DWT, combined with simple moving average, worked magic. Once the baseline was estimated, the above-baseline sessions was attributed to specific TV spots. And this was where the second challenge happened, namely, how to divide the sessions among the overlapped TV spots. To solve this, we used a probabilistic model to apportion sessions based on the ratio of each spot’s rate. Lastly, we crystalized our solutions in a pipeline of generalized R scripts that the client integrated to their Azure production environment.

The client used to use a service called Quality Analytics for attribution modeling, which cost them $2500 per month. Our solution allowed the client to eliminate this cost entirely.

![](/images/projects/estimate_tv_attribution_with_wavelets/baseline-vs-actual-fwd-5mins.png)