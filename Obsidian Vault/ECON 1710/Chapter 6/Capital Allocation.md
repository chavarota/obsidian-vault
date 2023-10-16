The most straightforward way to control the risk of a portfolio is through the fraction of a portfolio invested in [[Treasury Bills|Treasury bills]] versus the fraction invested in [[Risk Premium|risky assets]]. 

Our universe has one risk-free asset and one risky portfolio. We define the *complete portfolio* a the total holdings of the risk-free assets and the risky portfolio. Its [[Scenario Analysis|expected rate of return]] is defined as:
$$E(r_c) = yE(r_p) + (1-y)r_f$$

Where $y$ is the fraction of complete portfolio in the risky asset.

The standard deviation of the complete portfolio is given by:
$$\sigma_c = y\sigma_p$$
The investment opportunity set (Capital Allocation Line) can be described by the straight line that joins the risk free asset's expected return and standard deviation $(r_f, 0)$ and the risky portfolio's expected return and standard deviation $(E(r_p), \sigma_p)$. Thus, its slope is given by $\frac{E(r_p)-r_f}{\sigma_p}$, which is the [[Sharpe Ratio]].
![[Capital Allocation Line.png]]

## Optimal asset allocation
To solve the [[Mean-Variance Utility|utility]]-maximization problem, we write the problem as follows:
$$\max_y(E(r_c)-1/2A\sigma_c^2)=\max_y(yE(r_p) + (1-y)r_f) - 1/2A\sigma_c^2$$
Take the derivative and set to zero:
$$
\begin{align}
0 &=\frac{d}{dy}\left[ yE(r_p) + (1-y)r_f - 1/2A\sigma_c^2 \right] \\
&= \frac{d}{dy} [y(E(r_p)-r_f) + r_f - 1/2A\sigma_c^2] \\
&= \frac{d}{dy} [y(E(r_p)-r_f) + r_f - 1/2Ay^2\sigma_p^2] \text{ (N.B: } \sigma^2_c = y^2\sigma^2_p)\\
&= E(r_p)-r_f - Ay\sigma^2_p
\end{align}
$$

Therefore, we write:
$$
\begin{align}
Ay^*\sigma^2_p &= E(r_p) - r_f
\end{align}
$$
$$y^* = \frac{E(r_p) - r_f}{A\sigma^2_p}$$

## What if I want to invest > 100% in risky assets?
In theory, this line extends beyond $y=100\%$. You can borrow money to invest it into the risky portfolio. Since we borrow money at higher than the risk-free rate, there is a kink in the CAL - the slope to the right of $y=100\%$ is shallower than the slope to the left. (the Sharpe ratio gets smaller - less return for each additional unit of risk.)
![[Capital Allocation 2.png]]

Due to the kink, there are many different values of A that might  have an optimal $y^* = 100\%$. A linear function cannot usually have the same output for many different inputs, so the way we do this is as follows:
- Set $y^* = 1$ and find the risk tolerance A, given the risk-free rate of interest.
- Now perform the same calculation but this time, replace the risk-free rate of interest with the borrowing rate. You will get a different value for A
- These two values for A form the lower and upper bounds for all values of A that would choose $y^* = 1$.