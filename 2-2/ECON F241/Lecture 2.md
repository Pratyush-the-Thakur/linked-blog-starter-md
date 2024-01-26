### Simple Linear Regression Model
- Answer questions like
	- If weekly income goes up by 10, how much will food expenditure rise or fall
- Several Corresponding y values for each x value

#### Conditional pdf of Y
- Probability associated with Y given the value of X
- The amount spent on food depends on many factors
	- kids, old people, veg/non veg, eating out
	- Random factors like impulse buying
- Make a graph of E(Y|X)

### Population Regression Function

- You cant just get data for the whole world, impractical
- Even if people are completely irrational, the slope shall remain constant
- $E(Y|X_i)$ is the conditional expectation function or PRF or Population regression or Linear Population Regression function
- what form does $f(X_i)$ assume?
- Empirical question, although we can use theory in specific cases
- For example, an economist might argue that consumption expenditure is linearly related to income
$$E(Y|X_i) = \beta_a + \beta_bX_i$$
- $\beta_1$ and $\beta_2$ are unknown but fixed, know as regression coefficients
- Known as intercept and slope coefficients respectively
- estimate their values based on sample observations


### Stochastic Specification of  PRF
$$u_i = Y_i - E(YX_i)$$
OR
$$Y_i = E(Y|X_i) + u_i$$
- Two components to PRF, fixed and random. U is the random one
- Stochastic means Random I think?
- $u_i$ is known as the stochastic disturbance, or stochastic error term or disturbance term
- $E(Y|X_i)$ is the deterministic component and $u_i$ is the random or nonsystematic component
$$Y_i = \beta_1+ \beta_2 + u_i$$
$$E(Y|X_i) = E(E(Y|X_i)) + E(u_i|X_i)$$

$$E(Y|X_i) =E(Y|X_i) $$
- We assume that $E(u_i|X_i)$ = 0 by logic
- $u_i$ is a proxy for all omitted variables that we didnt include, but still affect $Y$. 
	- Say a group of families are part of a religion that does  intermittent fasting on certain months, that would affect their expenditure on food, and is accounted for in $u_i$

#### What is the need?
- Vagueness of theory
- Sometimes we dont have enough data
	- Other factors might affect food expenditure. Tastes, age,habits, location, religion
- Intrinsic Randomness of Human behaviour
	- We are very impulsive, a family could just go to mcdonalds on a tuesday night for no reason whatsoever
- Wrong Functional form
	- might not actually be linear maybe a quadratic or cubic function

### Sample and Population
- 