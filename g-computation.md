also called COM

The most literal interpretation of the potential outcomes framework. You train a model to predict outcome given treatment and covariates. Then, you predict everyone's outcome but if they were treated. Then, you predict everyone's outcome but if they were untreated. Then, you compare the means.

The tricky bit is correclty specifi

#question: won't the baseline characteristic of the population bias the model? e.g., if 90% of the study population is treated, and then the model will probably be better at predicting outcomes for treated guys than untreated guys. Seems like we should weigh the inputs such that they reflect the distribution we want to make inferences about.