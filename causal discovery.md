#discovery

We have some data, we want to make a causal graph

Two main approaches
- independence-based: requires the unappealing assumption of [[faithfulness]]
	- you're gonna be doing a lot of conditional independence tests
		- crap ton of data
		- crap ton of time
	- algorithms
		- [[PC algorithm]] assumes no unobserved confounders, acyclicity is slow
		- [[FCI algorithm]] allows unobserved confounders
		- [[CCD algorithm]] allows cyclic graphs
		- [[SAT-base causal discovery]] is the chad
- semi-parametric