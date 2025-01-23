Root Mean Squared Error (RMSE) is the square root of the mean of the squared errors. It is a useful error metric for numerical predictions, primarily to compare prediction errors of different models or configurations for the same variable, as it is scale-dependent. RMSE measures how well a regression line fits the data.

$$
\mathrm{RMSE} = \sqrt{\frac{1}{n}\sum_{i=1}^{n}\left(y_i - \hat{y}_i\right)^2  } 
$$
- $y​_{i}$ = actual value
- $\hat{y_{i}}$​ = predicted value
- $n$ = number of observations

### Significance of RMSE

- **Scale-Dependent**: RMSE has the same units as the target variable. A lower RMSE indicates better model performance, but the value must be compared with the scale of the target variable to make sense.

- **Sensitive to Outliers**: Since RMSE squares the error terms, larger errors have a disproportionately large effect, making RMSE sensitive to outliers.

- **Comparing Models**: RMSE can be used to compare models. A model with a lower RMSE value is generally considered better at predicting the target variable.