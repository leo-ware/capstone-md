#sampling

https://www.youtube.com/watch?v=OXDqjdVVePY

We have a complicated pmf $f(x)$ which we want to sample from. We pick another distribution $g(x)$ which is easy to sample from. Then, we pick an $M$ such that $Mg(x) > f(x)$. To get a sample from $f$, we first sample $x_i$ from $g$. Then, we "accept" $x_i$ with probability $f(x_i)/MG(x_i)$ and reject it otherwise.

This works well when $Mg$ traces $f$ closely. It falls apart when they are not close because you end up rejecting lots of samples. This tends to happen for complicated/high dimensional $f$.

Proof:

Let $D$ represent the density of the samples. Let $S$ represent the sample itself and $A$ represent the chance that we accept it.

Then by Bayes theorem, the density of samples that we accept is equal to the probability that we we accept a sample given its value times the density of the sampling distribution at that value, divided by the unconditioned probability of acceptance.

$$
D(S | A) = {P(A | S)D(S) \over P(A)}
$$