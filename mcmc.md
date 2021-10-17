markov-chain monte carlo sampling: A technique for sampling from (continuous?) distributions.

In [[rejection sampling]], we face issues when the probability of acceptance gets too low. We have trouble "finding" value of $f(x)$. MCMC says that this is because we are throwing away information. Whenever we get a sample with a high probability of acceptance, it is probably a good idea to look around in the same are because we might be able to get more samples there.

So, we find a markov chain whose stationary distribution is $f(x)$.

