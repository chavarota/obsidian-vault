The mean of $Y$ is the weighted average of the conditional expectation of $Y$ given $X$ (the weights are the probability distribution of $X$). Stated mathematically:
$$E(Y)=\sum_{i=1}^n E(Y|X=x_i)P(X=x_i)$$
## Alternate form
The LIE can also be written as:
$$E(Y)=E(E[Y|X])$$
The proof for this is:
$$
\begin{align}
	E(E[Y|X]) &= \sum_{i=1}^n E(Y|X=x_i)P(X=x_i) \\
	&= \sum_{i=1}^n\left( \sum_{j=1}^n y_jP(Y=y_j | X = x_i)\right)P(X=x_i) \\
	&= \sum_{i=1}^n \sum_{j=1}^n y_jP(X = x_i | Y=y_j)P(Y=y_j) \text{ (Thanks to Bayes' Law)}\\
	&= \sum_{i=1}^n \sum_{j=1}^n y_j P(Y=y_j)P(X = x_i | Y=y_j) \\
	&= \sum_{j=1}^n y_j P(Y=y_j) \sum_{i=1}^nP(X = x_i | Y=y_j) \text{ (Note that  } \sum_yP(Y=y|X=x)=1)\\
	&= \sum_{j=1}^n y_jP(Y=y_j) \\
	&= E(Y)
\end{align}
$$

