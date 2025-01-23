Mean Absolute Error measures the average difference between predicted values and actual values in a dataset. It shows how far predictions are from the true values without considering direction.

- Calculated using absolute differences
- Simple to compute and interpret
- Treats all errors equally
- Less sensitive to large errors than MSE
- Commonly used to evaluate regression models

$$
\mathrm{MAE} = \frac{1}{n} ~~ \sum_{i=1}^{n}\left   | y_i - \hat{y}_i \right|
$$
- ​$y_{i}$ :Actual value for the $i^{th}$ observation
- $\hat{y}$ ​: Calculated value for the $i^{th}$ observation
- $n$: Total number of observations


### Implementation 

**Example**:
```
actual = [2, 3, 5, 5, 9]
calculated = [3, 3, 8, 7, 6]

n = 5
sum = 0
for i in range(n):
    sum += abs(actual[i] - calculated[i])

error = sum/n
print("Mean absolute error : " + str(error))

```

**Output:**
` Mean absolute error: 1.8`


### Why to Choose Mean Absolute Error?

- **Interpretability** : Since MAE is in the same unit as the target variable, it's easy to understand. For instance, an MAE of 5 in a house price prediction model indicates an average error of $5,000.

- **Robustness to Outliers** : Unlike metrics that square the errors (like MSE), MAE doesn't disproportionately penalize larger errors, making it less sensitive to outliers.

- **Simplicity** : MAE provides a straightforward measure of average error, facilitating quick assessments of model performance.