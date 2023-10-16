We've shown that when the sample size N gets large, the [[The Sample Mean|sample mean]] $\hat{\mu}$ gets close to the population mean $\mu$. How do we quantify how close?

## Overview
1. The **null hypothesis** is that the population mean is a particular value:
$$H_0: \mu = \mu_0$$
2. Calculate the **p-value** that we would observe $\hat{\mu}$ at least this far from $\mu_0$ if $H_0$ is true.
3. Reject if the **p-value** is under a certain threshold $\alpha$ (usually 0.05).
4. Form a **confidence interval** that collects all the possible values of $\mu_0$ that we can't reject in this way.

## Hypothesis testing with a normally distributed $\hat{\mu}$
In most cases, the underlying $Y_i$ are [[Normal Distribution|normally distributed]]. We write $Y \sim N(\mu, \sigma^2)$. This means that the sample mean has the distribution:
$$\hat{\mu} \sim N(\mu, \frac{\sigma^2}{N})$$

Define the $t$ statistic as:
$$\hat{t}=\frac{\hat{\mu}-\mu_0}{\sigma/\sqrt{N}}$$
We define this because under the null hypothesis, $\hat{t} \sim N(0,1)$. Thus, the **p-value** for the null can be defined as:
$$p(\hat{t})=1 - \phi(-t < \hat{t} < t) = 1 - [\phi(|\hat{t}|) - \phi(-|\hat{t}|)]$$
For the 5% level, we reject $H_0$ if $\hat{t} > 1.96$. To get this in terms of $H_0$, solve $\frac{|\hat{\mu}-\mu_0|}{\sigma/\sqrt{N}} < 1.96$. These values will be the upper and lower bounds of the confidence interval.

## Significance and Power
- The **significance** level of a test is the pre-specified probability of incorrectly rejecting the null when it is true (type 1 error). This is equal to the **p-value**.
- The **power** of a test is the probability of correctly rejecting the null when it is false. (type 2 error).



