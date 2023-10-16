3 main types:
- Descriptive questions  (i.e. has economic inequality increased since 1960?)
- Causal questions (i.e. How do increases in the minimum wage affect employment?)
- Forecasting questions (i..e. what will the unemployment rate be next quarter?)
## Why is answering these questions hard?
For descriptive questions, we only observe data for a sample of individuals, not the full population.

Causal questions are even harder to answer because they contain both a descriptive component (what are outcomes in reality?) and a counterfactual component (how would things have been under a different treatment?)
## Answering causal questions
When thinking about causal questions, it's often easier to split the problem in two:
1. **Identification**: what could we learn about the parameters we care about if we had observable data for the entire population?
2. **Statistics**: what can we learn about the full population that we care about from the finite sample that we have?

### Framework for thinking about these steps
- **Sample**: the data you actually observe
	- *A survey of students from Brown and URI graduates about their earnings*
- **Estimator**: a function of the data in the sample
	- *Difference in earnings between Brown and URI students in survey*
- **Estimand**: a function of the observable data for the population
	- *Difference in earnings between all brown and URI students.*
- **Target (structural) parameter**: what we actually care about
	- *Causal effect on earnings of going to Brown vs URI.*

*Statistical inference* is the process of learning about the *estimand* from the *estimator* constructed with your *sample*.

*Identification* is the process of learning about the *parameter* from the *estimand*.

When thinking about these steps, we use [[Potential Outcomes Notation|potential outcomes notation]].