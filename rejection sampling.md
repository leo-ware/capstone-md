#sampling

We have a complicated pmf $f(x)$ which we want to sample from. We pick another distribution $g(x)$ which is easy to sample from. Then, we pick an $M$ such that $Mg(x) > f(x)$. To get a sample from $f$, we first sample $x_i$ from $g$. Then, we "accept" $x_i$ with probability $f(x_i)/MG(x_i)$ and reject it otherwise.

This works well when $Mg$ traces $f$ closely. It falls apart when they are not close because you end up rejecting lots of samples. This tends to happen for complicated/high dimensional $f$.