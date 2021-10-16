The propensity score is the probability of receiving treatment given relevant covariates.

We only care about confounders in the first place because of how they influence P(T). The propensity score basically encodes all the relevant information here. If we condition on the true propensity score, then we can guarantee that 

model that predicts treatment given covariates, used in a number of ways
- matching
- stratification
- conditional adjustment
- inverse probability of treatment weighting

generally super biased and not great, also pretty popular