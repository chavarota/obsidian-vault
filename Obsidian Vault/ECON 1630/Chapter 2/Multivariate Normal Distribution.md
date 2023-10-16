This distribution is the same as the [[Normal Distribution|normal distribution]] except it is defined for a vector of multiple variables.

## Parameters
- $\mu \in R^K$ = a vector representing the mean (expected) values of all K [[Random Variables|random variables]].
- $\Sigma \in R^K$ = a variance-covariance matrix representing the relations between all K variables.

## Useful facts
- If $(X,Y)'$ is joint-normally distributed, then:
	- The marginal distributions of $X$ and $Y$ are normal
	- The [[Conditional Distribution|conditional distributions]] of $X | Y$ and $Y|X$ are normal
	- Any fixed linear combination $aX+bY+c$ is normally distributed.