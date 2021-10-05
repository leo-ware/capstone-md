#libraries 

A library for causal inference
- authors: [[Amit Sharma]]
- paper: [[sharma 2020 - dowhy.pdf]]
- github: [github/dowhy](https://github.com/microsoft/dowhy)

Idea is that other libraries (which?) spend too much time on [[estimation]] and not enough time on [[identification]] and [[robustness]]. Breaks modeling process into four steps
- model = incorporate prior information
- identify = identify causal graph
- estimate = estimate causal treatment effect
	- uses [[backdoor adjustment]]  and graph based methods to work out an expression
	- plug and play with [[EconML]] and [[causalml]]
- robustness checking