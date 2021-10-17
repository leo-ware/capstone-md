#discovery

We have some data, we want to make a causal graph

Two main approaches
- independence-based: requires the unappealing assumption of [[faithfulness]]
	- you can't do better than a [[markov equivalence]] class
	- you're gonna be doing a lot of conditional independence tests = crap ton of data
	- algorithms
		- [[PC algorithm]] assumes no unobserved confounders, acyclicity is slow
		- [[FCI algorithm]] allows unobserved confounders
		- [[CCD algorithm]] allows cyclic graphs
		- [[SAT-base causal discovery]] is the chad
- semi-parametric
	- if you have a linear functional form with nongaussian noise, you can get the direction