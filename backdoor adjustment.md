#identification

The *Modularity Assumption* if we set the value of one of the nodes in the graph to a constant, then the *conditional distributions* of all the other variables do not change. Aka, we can intervene without disrupting the mechanisms.

This gives us the *truncated factorization*. This is the most basic way of turning do statements into statistical expressions. It says that if we condition on doing x, then the distribution will be zero everywhere x isn't done.

![[Pasted image 20211006005956.png]]

We can use this to get the back-door adjustment. This says that if we block all the noncausal paths from T to Y by conditioning on w, then we can get an expression for P(Y | do(T)).

More specifically, w is a *sufficient adjustment set* iff,
- w blocks all backdoor paths from T to Y
- w contains no descendants of T

![[Pasted image 20211006005832.png]]

This should be familiar. It's just saying that you need to control for confounders when you do your regression. This is the formal model that allows us to prove that intuition.