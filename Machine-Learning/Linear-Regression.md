Linear regression is a type of supervised machine-learning algorithm that learns from mapping the data points with most optimized linear functions which can be used for prediction on new datasets. It assumes that there is a linear relationship between the input and output, meaning the output changes at a constant rate as the input changes. This relationship is represented by a straight line.

### Best Fit Line in Linear Regression
In linear regression, the best-fit line is the straight line that most accurately represents the relationship between the independent variable (input) and the dependent variable (output). It is the line that minimizes the difference between the actual data points and the predicted values from the model.

Equation for best fitted line.
$$
y=mx+b
$$
- **y** is the predicted value (dependent variable)
- **x** is the input (independent variable)
- **m** is the slope of the line (how much y changes when x changes)
- **b** is the intercept (the value of y when x = 0)



$$
SSE = \sum_{i=1}^{n} (y_i - \hat{y}_i)^2
$$
$$
MSE = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2
$$

| **Advantages**                                                                     | **Disadvantages**                                  |
| ---------------------------------------------------------------------------------- | -------------------------------------------------- |
| Simple and easy to implement with interpretable coefficients.                      | Assumes a linear relationship between variables.   |
| Computationally efficient, suitable for large datasets and real-time applications. | Sensitive to multicollinearity among features.<br> |
| Relatively robust to outliers.                                                     | Requires proper feature engineering.               |
| Serves as a good baseline model.                                                   | Can overfit or underfit depending on data.         |
| Widely available in ML libraries and software.                                     | Limited for modeling complex relationships.        |
