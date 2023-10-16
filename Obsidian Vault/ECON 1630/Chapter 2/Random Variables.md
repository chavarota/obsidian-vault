A random variable is a numerical summary of a random process. It has a cumulative distribution function (cdf) that defines the probability that random variable X is some value x or below: $F(x)=P(X \leq x)$.
## Some terminology:
- **Outcomes** are mutually exclusive results of a random process
- The **sample space** is the set of all possible outcomes
- An **event** is a subset of the sample space. Its probability is the sum of probabilities of the included outcomes
- The **support** of a random variable is the set of all values that X can take.

## Density and Mass Functions:

If X is discrete, we define the probability mass function (pmf) as the probability that X takes on each value in the support: $p(x) = P(X = x)$. The cdf is then: 
$$\sum_{i \leq x}p(i)$$
For a continuous random variable, we define the probability density function (pdf) as $f(x) = \frac{d}{dx}F(x)$ where the cdf is:
$$F(x)=\int_{-\infty}^xf(t)dt$$
### Properties of cdfs
- Non-decreasing: $F(x) \geq F(x')$ if $x > x'$
- Satisfies $\lim_{x \rightarrow -\infty}F(x) = 0$ and $\lim_{x \rightarrow \infty}F(x) = 1$
### Properties of pdfs
- Non-negative: $f(x) \geq 0$ for all x
- Satisfies $\int_x f(x)dx = 1$
- For pdfs: $\sum_x p(x)=1$

## Important distributions:
- [[Bernoulli Distribution]]
- [[Normal Distribution]]
- [[Multivariate Normal Distribution]]