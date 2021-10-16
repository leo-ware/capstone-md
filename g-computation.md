also called *conditional outcomes model (COM)*

The most literal interpretation of the potential outcomes framework. You train a model to predict outcome given treatment and covariates. This is called the *Q-model* Then, you predict everyone's outcome but if they were treated. Then, you predict everyone's outcome but if they were untreated. Then, you compare the means.

Alternative formulation: you get a model for $P(Y | X, T)$. Then, you marginalize on $X$. This gives you $P(Y | do(T))$. I think?

The tricky bit is correctly specifying a model for outcome given treatment and covariates. But also you could just use like a random forest or something right?

Pitfalls: this method can underestimate the effect of T in high-dimensional data.

#question: [[chatton 2020 - g-computation sim.pdf]] claims that you can do this for the ATT by just marginalizing using the treatment group, but I am skeptical. Won't the baseline characteristic of the population bias the model? e.g., if 90% of the study population is treated, and then the model will probably be better at predicting outcomes for treated guys than untreated guys. This means we will only be able to get ATE, not ATT and ATC? right?