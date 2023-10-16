$$D_i=
	\begin{cases}
		0&\text{if person i does not go to Brown}\\ 
		1&\text{if person i does go to Brown}
	\end{cases}
$$
$$Y_i(1)=\text{outcome under treatment} = \text{earnings at Brown}$$$$Y_i(0)=\text{outcome under control} = \text{earnings at URI}$$
We can write the observed outcome as $Y_i = D_iY_i(1) + (1-D_i)Y_i(0)$

We can write the expected outcome conditional on a treatment (note that some of these groups might not exist in the real world), such as $E[Y_i(0)|D_i=1]$, which signifies the "hypothetical average earnings at URI (treatment 1) for actual, current Brown students."

To get around this, we could assume, for example, that  $E[Y_i(0)|D_i=1] =E[Y_i(0)|D_i=0]$. However, this is not true if there are confounding variables that affect the income of Brown and URI students.

**Confounding variables** are variables that affect the outcome of an experiment other than the treatment.
