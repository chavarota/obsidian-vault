We will now bring together our study of the [[Portfolios of Two Risky Assets|optimal portfolio of two risky assets]] and of the [[Capital Allocation|optimal allocation to risky and risk-free assets]]. In this case, [[Treasury Bills|treasury bills]] are the risk-free asset, and our risky portfolio is made up of a [[Equity Securities|stock fund]] and a [[The Bond Market|bond fund]].

## Step 1: Find optimal risky portfolio
In our case, the risky portfolio opportunity set is given to us (a function of $\rho_{DE}$, the [[Correlation Coefficient|correlation coefficient]], the [[Expected Value|expected returns]] and [[Variance|standard deviations]] of the funds). Thus, first we have to find the portfolio opportunity set (see [[Portfolios of Two Risky Assets|here]]).

## Step 2: find the steepest possible CAL that intersects the portfolio opportunity set
We essentially want a risky portfolio that maximizes the [[Sharpe Ratio]]. This translates to wanting to find the steepest capital allocation line, given the constraint of our portfolio opportunity set. Graphically, this translates to finding the steepest CAL that still crosses the portfolio opportunity set - so it must be tangent.

We can define our *objective function* as the Sharpe Ratio (what we are trying to maximise):
$$\max_{w_i} S_p=\frac{E(r_p)-r_f}{\sigma_p}$$
As a constraint, we know that: 
$$E(r_p)=w_DE(r_D)+w_EE(r_E)$$
$$\sigma_p=\sqrt{w_D^2\sigma_D^2 + w_E^2\sigma_E^2+2w_Dw_ECov(r_D, r_E)}$$
$$w_D+w_E=1$$
After some boring algebra, this comes out to:
$$w_D^*= \frac{E(r_D)\sigma_E^2-E(r_E)Cov(r_D, r_E)}{E(r_D)\sigma_E^2 + E(r_E)\sigma_D^2- [E(r_D) + E(r_E)]Cov(r_D, r_E)}$$
This equation gives the combination of $w_D, w_E$ that results in the optimal risky portfolio, P:
![[Opportunity Set.png]]
