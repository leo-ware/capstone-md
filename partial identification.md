Make weaker assumptions, get stronger results. Partial identification is about bounding the [[ATE]] using extremely weak assumptions.

The **no assumptions bound** says that If $a < Y < b$, e.g. is the outcome is lower and upper bounded by a and b, then:
![[Pasted image 20211016234133.png]]

The length of this interval is $b - a$. Unfortunately, this interval will always contain 0. It will not tell you whether the effect is positive or negative.

General bounding technique here is to break up the causal estimand into the observational-counterfactual decomposition. Then, you do bounds on different terms.

![[Pasted image 20211016234504.png]]

You can do this for different sets of assumptions. You can assume that the effect of treatment is always positive or always negative.

Neal mentions bounding on the assumption that expected outcomes under both treatment and control conditions are better for the treatment group than the control group. E.g., positive self-selection. I don't 