# Regression

- Using least squares to minize the squared-error between each point and the predict line
- evaluate this bying checking the r-square value

**Measuring error with r-squared**

- How do we measure how well our line fits our data?
- R-squared measures the fraction of the total variation in Y that is captured by the model
- Ranges from 0 to 1: 0 is bad, 1 is good

# Linear Regression

~ Regression using straight line

- Fit a line to a data set of observations
- Then use the line to predict unobserved values

**Steps**

1. Plot the scatter pots graph: scatter(x, y)
2. Get necessary information:

```python
from scipy import stats

slope, intercept, r_value, p_value, std_err = stats.linregress(pageSpeeds, purchaseAmount)
```

> We use slope and intercept to construct a fit line (line go through most of the dots)

> Then use r_value to evalutate to see how well the data is captured

# Polynomial Regression

~ Regression using higher order polynomial graph to define the patterns

**Notice** Just use the right amount of order to create the polynomial to fit the data. Be aware of overfitting

# Multiple Regression

Regression affected by several features (variables)

- Multivariate regression: predict more than one things of the time using multiple features
- Still uses least squares
- Still measure fit with r-squared
