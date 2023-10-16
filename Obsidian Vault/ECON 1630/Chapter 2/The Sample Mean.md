Suppose we are interested in learning about the population mean $\mu = E[Y_i]$ from an *iid* representative sample $\mathbf{Y}$ of size N. A natural estimator for this is the sample mean:
$$\hat{\mu}=\frac{1}{N}\sum_i Y_i$$
Even though the population average, $\mu$, remains constant, $\hat{\mu}$ will depend on the sampled individuals, so it is a random variable. We can derive the expected value and variance of $\hat{\mu}$:
$$
E[\hat{\mu}]=E\left[ \frac{1}{N}\sum_i Y_i\right] =\frac{1}{N} \sum_iE[Y_i] = \frac{N\mu}{N}=\mu\\
$$
The above equation states that the sample mean is an **unbiased** estimator for the population mean because its expected value is the population mean.
$$
Var(\hat{\mu})=Var\left(\frac{1}{N}\sum_i Y_i\right)=\frac{1}{N^2} \sum_i Var(Y_i) = \frac{\sigma^2}{N}$$
The above equation states that the standard deviation of the sample mean from its mean (which is equal to the population mean) shrinks as sample size increases. Therefore, $\hat{\mu}$ is a consistent estimator for the population mean.