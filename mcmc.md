#sampling 

markov-chain monte carlo sampling

How do we sample from a distribution when we only have a likelihood function?

In [[rejection sampling]], we face issues when the probability of acceptance gets too low. We have trouble "finding" value of $p(x)$. MCMC says that this is because we are throwing away information. Whenever we get a sample with a high probability of acceptance, it is probably a good idea to look around in the same are because we might be able to get more samples there.

So, we want find a markov chain whose stationary distribution is $p(x)$. It turns out we can use something called the detailed balance condition. Let $T(a | b)$ represent the probability that a markov chain $M$ transitions to state $a$, given that it is in state $b$. Then the detailed balance condition states that, for any pair $-\infty \lt (x, y) \lt \infty$.

$$p(x)T(y | x) = p(y)T(x | y)$$

If this holds, then the stationary distribution of $M$ is $p(x)$. Proof:

$$\sum_x p(x)T(y | x) = \sum_x p(y)T(x | y)$$
$$\sum_x p(x)T(y | x) = p(y)$$
$$pT = p$$

There are a couple techniques for finding a markov chain like this.
- Metropolis-Hastings samples from a distribution centered at zero. It adds this sample to the current value $a$ to get a candidate next value $b$. It accepts the next value with probability ${p(b)T(b | a) \over p(a)T(a | b)}$ where $p$ is our likelihood and $T$ is our transition function.
- Gibbs sampling is for when sampling from a multivariable distribution is expensive, but samplein