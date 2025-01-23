Mean Squared Error (MSE) is one of the most common metrics used for evaluating the performance of regression models. It measures the average of the squares of the errors—that is, the average squared difference between the predicted and actual values. MSE provides a way to quantify how much error exists in a model’s predictions, and is particularly useful in fields like machine learning, data science, and statistics.



$$
\mathrm{MSE} = \frac{1}{n}\sum_{i=1}^{n}\left(y_i - \hat{y}_i\right)^2
$$
- $y_{i}$​ is the actual value (true value).
- $\hat{y_{i}}$​ is the predicted value (from the model).
- $n$ is the total number of data points.



### Implementation

**Example:**
```
import numpy as np

# Given values
Y_true = [1,1,2,2,4]  # Y_true = Y (original values)

# Calculated values
Y_pred = [0.6,1.29,1.99,2.69,3.4]  # Y_pred = Y'

# Mean Squared Error
MSE = np.square(np.subtract(Y_true,Y_pred)).mean()
```

**Output:
`Output: 0.21606`

