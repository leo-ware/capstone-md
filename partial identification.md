Make weaker assumptions, get stronger results. Partial identification is about bounding the [[ATE]] using extremely weak assumptions.

General technique with the proofs here is to break up the causal estimand into the observational-counterfactual decomposition. Then, you do bounds on different terms.

![[Pasted image 20211016234504.png]]

## No Assumptions Bound

If $a < Y < b$, e.g. is the outcome is lower and upper bounded by a and b, then:
![[Pasted image 20211016234133.png]]
The length of this interval is $b - a$. Unfortunately, this interval will always contain 0. It will not tell you whether the effect is positive or negative.

## 