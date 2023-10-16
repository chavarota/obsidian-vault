The conditional distribution $Y|X=x$ is the distribution of Y among the sub-population with $X=x$.

The PMF of the conditional distribution is:
$$p(y|x)=P(Y=y|X=x)=\frac{P(Y=y, X=x)}{P(X=x)}=\frac{p(y,x)}{p(x)}$$
This leads to [[Bayes' Rule]].

## Conditional Expectation
The conditional expectation of $Y$ given $X$ is the mean of the conditional distribution of $Y$ given $X$
$$E(Y|X=x)=\sum_{i=1}^n P(Y=y_i|X=x)$$
If $E(X|Y)=E(Y)$, we say that $X$ is **mean independent** of $Y$. If $X$ and $Y$ are [[Independence (Statistics)|independent]], when we say that they are also mean independent, but this is not necessarily true the other way around.