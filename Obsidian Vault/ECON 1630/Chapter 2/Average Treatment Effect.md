Recall the [[Potential Outcomes Notation|potential outcomes framework]].

Suppose that for each person we assign $D_i$ by flipping a coin. We can then say that $D_i \perp\!\!\!\perp (Y_i(1), Y_i(0))$. In words, the treatment is [[Independence (Statistics)|independent]] from the outcome.

What is the population mean for treated units?
$$E[Y_i|D_i=1] = E[Y_i(1)|D_i=1]$$
The above equation tells us that the average outcome for all people who actually received the treatment (real-world observation) is the same as the expected outcome of all potential people who might receive the treatment given that they have received the treatment. Then, because of the independence condition, we can say that $D_i$ and $Y_i$ are mean-independent. Thus:
$$E[Y_i(1)|D_i=1] = E[Y_i(1)]$$
We can similarly write that $E[Y_i|D_i=0]=E[Y_i(0)|D_i=0]=E[Y_i(0)]$.

The point of doing this is that we can now use the difference in two population means to estimate the treatment effect on the entire population. Define the Average Treatment Effect (ATE):
$$
\begin{split}
\text{Average treatment effect} &= \text{Treated population average} - \text{Control population average} \\
\text{ATE} &= E[Y_i|D_i=1] - E[Y_i|D_i=0] =E[Y_i(1)-Y_i(0)]
\end{split}
$$
## Identification under conditional unconfoundedness
Now suppose that $D_i \perp\!\!\!\perp (Y_i(1), Y_i(0))|\bf{X_i}$, where $\bf{X_i}$ is a vector of observable characteristic.

Conditional unconfoundedness says we effectively have an experiment among people with the same value of $\bf{X_i}$.

We can define the **conditional average treatment effect**:
$$E[Y_i|D_i=1, \mathbf{X_i=x} ] - E[Y_i|D_i=0,\mathbf{X_i=x}] = E[Y_i(1)-Y_i(0)|\mathbf{X_i=x}]$$
Given a CATE, we can identify the ATE using the [[Law of Iterated Expectations]]:
$$E[E[Y_i(1)-Y_i(0)|X_i]] = E[Y_i(1)-Y_i(0)]$$
However, this requires us to have some treated and some control units for each value of $\mathbf{X_i}$ in order to learn about the overall ATE.