
### Linear Regression Model
- We wont use $E(Y|X_i)$ for actually drawing the line
- Sample regression function 
- $$ \hat{Y} = \hat{\beta_1} + \hat{\beta}_2X$$
- $$\hat{\beta_2} = \frac{Y_h - Y_1}{X_h - X_1}$$
- Statistical method to estimate population is called estimator (shocking)
- The estimator is always random
- You can draw a very large number of samples from a population, the regression coefficients will be different for each and every one
- This means that the value of the slope($\hat{\beta_2}$) is essentially random
- This is trivial, as this ignores quite literally every single point except the two we've selected, therefore it is not used
- We use the Ordinary Least Square Method (OLS)
- Why?
	- unbiased
	- least variance ($\sigma$)
- 2 Formulae
	- Slope method $$\hat{\beta_2} = \frac{Y_h - Y_1}{X_h - X_1}$$
	- OLS $$\hat{\beta_2} = \frac{\sum(X_i - X)(Y_i - Y)}{\sum(X_i-X)^2}$$
	- Every Random variable has a pdf, the Expected value of it will be the mean
	- $$E(\hat{\beta}) = \beta_2$$
	- $\beta_2$ being the  population parameter
	- This is the same for the OLS $\hat{\beta_2}$, however the variance is less due to the narrower distribution
	- This means the value is closer to the population parameter
![[Pasted image 20240119102857.png]]
- Fitting the line needs us to know the values of $\hat{\beta_1}$ and $\hat{\beta_2}$ 
$$Y_i = \hat{\beta_1} + \hat{\beta_2}X + \hat{u_i}$$
$$\hat{u_i} = Y_i - \hat{Y_i}$$
$\sum \hat{u_i}^2 = RSS$ = Residual Sum of Squares
- Partially Differentiate wrt $\hat{\beta_1}$ and $\hat{\beta_2}$
- we get the values
- OLS Estimator line formula
$$\bar{Y} = \hat{\beta_1} + \hat{\beta_2}X$$
$$\hat{\beta_2} = \frac{\sum(X_i - X)(Y_i - Y)}{\sum(X_i-X)^2}$$
- the pdfs of these variables are used in further analysis
