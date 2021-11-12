We have a probability distribution $P$ over some set of observed variables $x_i$, and we want to recover the [[causal structure | latent structure]]. I.e., we want to recover as much as we can of the [[causal structure]] without the assumption of unobserved confounders.

Make a graph with all the nodes. We have three kinds of relationships between nodes.
- A *marked* directed arrow means a direct causal relationship
- An unmarked directed arrow means either a direct causal relationship or an unobserved common cause
- 