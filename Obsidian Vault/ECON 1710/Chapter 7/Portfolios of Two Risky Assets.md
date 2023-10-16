Let us now consider our risky portfolio from our [[Capital Allocation|capital allocation]] question further. Say we have the choice between two risky assets to construct it: stocks and bonds. A proportion $w_D$ is invested in the bond fund, while the remainder, $W_E$, is invested in the stock fund. Note that $w_D + w_E = 1$.

The [[Expected Value|expected rate of return]] in the risky portfolio is given by:
$$E(r_p)=w_DE(r_D)+w_EE(r_E)$$
Its [[Variance|variance]] is:
$$\sigma_p^2=w_D^2\sigma_D^2 + w_E^2\sigma_E^2 + 2w_Dw_ECov(r_D, r_E)$$
It can be remembered as the sum of all the entries in the border-multiplied variance-[[Covariance|covariance]] matrix:

|       | $w_D$ | $w_E$ |
|:-----:|:-----:|:-----:|
| $w_D$ |    $w_Dw_DCov(r_D, r_D)$   |    $w_Dw_ECov(r_D, r_E)$   |
| $w_E$      |   $w_Ew_DCov(r_E, r_D)$    |   $w_Dw_DCov(r_D, r_D)$    |

N.B: $\sigma^2_D = Var(r_D) = Cov(r_D, r_D)$

The units of covariance depend on the units of measurement of the random variable. In order to compare how similarly two different variables move together, use the [[Correlation Coefficient]].

## Extreme case 1: $\rho_{DE} = 1$
If the two assets are perfectly correlated, the portfolio variance is written as:
$$
\begin{align}
\sigma^2_p &=w_D^2\sigma_D^2 + w_E^2\sigma_E^2 + 2w_Dw_E\sigma_D\sigma_E \\
&= (w_D\sigma_D + w_E\sigma_E)^2
\end{align}
$$
In this case, the standard deviation of the portfolio is just the weighted average of the component standard deviations. Therefore, there is no advantage to holding these two assets together.

## Extreme case 2: $\rho_{DE} = -1$
If the two assets are perfectly inversely correlated, then we get that:
$$
\begin{align}
\sigma^2_p &=w_D^2\sigma_D^2 + w_E^2\sigma_E^2 - 2w_Dw_E\sigma_D\sigma_E \\
&= (w_D\sigma_D - w_E\sigma_E)^2
\end{align}
$$
Therefore, a perfectly hedged position can be obtained by choosing the portfolio proportions to solve the equation:
$$w_D\sigma_D - w_E\sigma_E = 0$$
Solving, we find that the portfolio weights that satisfy this are:
$$w_D = \frac{\sigma_E}{\sigma_D+\sigma_E}$$
$$
w_E=\frac{\sigma_D}{\sigma_D+\sigma_E}
$$

We can draw these two cases out in a graph - all possible cases will lie in between these two:
![[Portfolios of 2 Risky Assets.png]]
The **Portfolio opportunity set** is shown for three different possible values of $\rho_{DE}$:
- $\rho_{DE} = -1$: red
-  $\rho_{DE} = 0$: purple
-  $\rho_{DE} = 1$: green

The **portfolio opportunity set** shows all combinations of portfolio expected return and standard deviation that can be constructed from the two available assets.
