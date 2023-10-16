The joint distribution of two discrete [[Random Variables|random variables]] is the probability that they simultaneously take on certain values.

The CDF of the joint distribution is:
$$F(x,y)=P(X \leq x, Y \leq y)$$
For discrete $(X,Y)$ we define the joint PMF as:
$$p(x,y)=P(X=x,Y=y)$$
For continuous $(X,Y)$ we define the joint PDF as:
$$f(x,y)=\frac{\partial{^2}}{\partial x \partial y}(F(x,y))$$
We sometimes refer to the **marginal distribution**: $p(x)=\sum_{y \in Y}p(x,y)$