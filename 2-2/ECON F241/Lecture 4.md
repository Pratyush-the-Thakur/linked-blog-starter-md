---
edited_seconds: 100
updated_at: 2024-01-25T10:15:54.638+05:30
---
### OLS
- Unbiased, Efficient
- Probability of being closer to the unknown value is higher


- Need to make certain assumptions (If even a single one of these are untrue, your results will not be desirable)
	- #### Data generation process
		- let ($y_i, x_i$) denote the ith data pair
		- the data pairs are random(value not known till observed), have pdfs 
		- Random variables, dont know value till observed, after which it is fixed
		- Random selection makes the first observation statistically independent of all other data pairs. Same with every other observation pair
		- If true, the behavioural rule $Y = \beta_1 + \beta_2X_i + u_i$
		- holds.....(finish)
	- #### Exogeneity
		- $Y = \beta_1 + \beta_2X_i + u_i$
		- Concerned with the random variable $u_i$, the disturbance/stochastic term
		- Unobservable, cant measure tastes or preference directly
		- Cant use $X_i$  to predict the value of $u_i$ 
		- $$E(u_i|x_i) = 0$$
		- This means that given a household's income, our best attempt is predicting that $u_i$ = 0, that the effects of all other factors on food expenditure average out to 0
		- 2 implications
			- Strictly exogenous
			- $$E(u_i|x_i) = 0 | E(u_i) = 0$$
			- Simply Exogenous
			- $$cov(u_i,x_i) = 0$$
			- Means no association between $u_i$ and $x_i$
		- Endogeneity implies the opposite, you can predict the value of $u_i$ using $x_i$, which obviously violates exogeneity 
		- Can you test for Endogeneity?
		- wage = $\beta_1 + \beta_2edu + \beta_3x+ \beta_4occ + u_i$
		- Endogenous! Why?
			- $\beta_2$ estimate is not unbiased
			- which means $u_i$ is correlated
			- which means $E(ui|x_i) \ne 0$
	- #### Homoscedasticity
		- Conditional variances of $u_i$ is constant
		- $$var(u_i|x_i) = \sigma^2$$
		- Heteroscedasticity implies the opposite, varying variance
		- $var(u_i/x_i) = E(u_i - E(u_i|X_i)^2) = E(U_i^2|X_i)$
		- as $E(u_i|X_i) = 0$
		- $var(u_i) = \sigma^2$
		- Constant
		- Same pdfs for all variables
		- Same mean for all (as $E(u_i) = 0$)
		- 