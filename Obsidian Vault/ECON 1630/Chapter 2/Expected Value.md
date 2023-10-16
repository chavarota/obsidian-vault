Intuitively, the expected value of a [[Random Variables|random variable]] is the long-run average value of the random variable under many repeated trials.

The expected value of X can also be defined as its probability-weighted typical value.
- For discrete random variables: $E[X] = \sum_{x \in X} p(x)x$
- For continuous random variables: $E[X] = \int_{x \in X}xf(x)dx$
	- May not exist if $p(x)$ puts high probability on extreme x.

**The expectation operator is linear:** $E[a+bX] = a + bE[X]$