---
edited_seconds: 1270
updated_at: 2024-01-25T10:50:10.702+05:30
---
- OLS 
- Finding out minimum of  $\sum \hat{u^2}(\hat{\beta_1},\hat{\beta_2})$
- no variance means all values of X are equal
- No point in running OLS then


#### No Autocorrection or no serial correlation between the Disturbances 
- Given $X_i$ and $X_j$ , the correlation between $u_i$ and $u_j$ is 0, th eobservations are sampled independently
- $$cov(u_i,u_j|X_i,X_j) = 0$$
#### Error Normality
- When samples are small, its advantageous that the random errors, and dependent variable y, given each x value are normally distributed
- Not an issue for regression analysis to work


- Prefer lower variance in sampling distribution for $\hat{\beta}$ so that its closer to the population
- Standard deviation is called Standard error

### Standard errors of Least-Squares Estimates
- least squares estimates are a function of sample data
- Precision of an estimate is measured by its standard error (se)
- Se is nothing but the standard deviation of the sampling distribution
- Distribution of the set of values of the estimator obtained from all possible samples of the same size



Formulae
- $$var(\hat{\beta_2}) = \frac{\sigma^2}{\sum(X_i - \hat{X})^2}$$
- $$se(\hat{\beta_2}) = \frac{\sigma}{\sqrt{\sum(X_i - \hat{X})^2}}$$
	- $$var(\hat{\beta_1}) =  \frac{\sum X_i^2}{n \sum(X_i - \bar X)^2}\sigma^2 $$
	- $$se(\hat{\beta_1}) =  \sqrt{\frac{\sum X_i^2}{n \sum(X_i - \bar X)^2}}\sigma $$
- Residual Sum of Squares:
- $$\hat{\sigma^2} = \frac{\sum \hat{u_i^2}}{n - 2}$$
- $n-2$ degrees of freedom


### Properties of Least Square Estimators: The Gayss Markov Theorem

- $\hat{\beta_2}$ is the **B**est **L**inear **U**nbiased **E**stimator (**BLUE**), IF
	- linear function of a random variable
	- Unbiased, i.e $E(\hat{\beta_2}) = \beta_2$
	- Minimum variance, so it is an efficient estimator
- Gauss-Markov Theorem:
	- Given the assumptions of the classical linear regression model, the least square estimators, in the class of unbiased linear estimators, have min $\sigma^2$. they are BLUE
	- Note: Linear here refers to the parametersD