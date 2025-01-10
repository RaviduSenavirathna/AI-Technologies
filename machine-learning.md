Machine learning is a branch of Artificial Intelligence that focuses on developing models and algorithms that let computers learn from data without being explicitly programmed for every task. In simple words, ML teaches systems to think and understand like humans by learning from the data.

Machine Learning is mainly divided into three core types:
- **Supervised Learning:** Trains models on labeled data to predict or classify new, unseen data.
- **Unsupervised Learning:** Finds patterns or groups in unlabeled data, like clustering or dimensionality reduction.
- **Reinforcement Learning:** Learns through trial and error to maximize rewards, ideal for decision-making tasks.

## Supervised Learning
Supervised learning algorithms are generally categorized into: 
- **[[Classification]]:** predict using discrete labels or categories. 
- **[[Regression]]:** predict using continuous numerical values.

| Algorithm               | Type           | Method                                                                  | Purpose                                                           |     |
| ----------------------- | -------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------- | --- |
| [[Linear-Regression]]   | Regression     | Linear equation minimizing sum of squares of residuals                  | Predict continuous output values                                  |     |
| [[Logistic-Regression]] | Classification | Logistic function transforming linear relationship                      | Predict binary output variable                                    |     |
| Decision Trees          | Both           | Tree-like structure with decisions and outcomes                         | Model decisions and outcomes                                      |     |
| Random Forests          | Both           | Combining multiple decision trees                                       | Improve classification and regression accuracy                    |     |
| Support Vector Machine  | Both           | Maximizing margin between classes or predicting continuous values       | Create hyperplane for classification or predict continuous values |     |
| K-Nearest Neighbors     | Both           | Finding k closest neighbors and predicting based on majority or average | Predict class or value based on k closest neighbors               |     |
| Gradient Boosting       | Both           | Iteratively correcting errors with new models                           | Combine weak learners to create strong model                      |     |
| Naive Bayes             | Classification | Bayes' theorem with feature independence assumption                     | Predict class based on feature independence assumption            |     |

## Unsupervised learning
Unsupervised learning are again divided into ****three main categories**** based on their purpose: 
- **[[Clustering]]:** group data points into clusters based on their similarities or differences.
- **Association Rule Mining:** simplify datasets by reducing the number of features while retaining the most important information.
- **Dimensionality Reduction:** Find patterns between items in large datasets typically in market basket analysis.

## Reinforcement Learning
Reinforcement learning interacts with environment and learn from them based on rewards.
- **Model-Based Methods:** model of the environment to predict outcomes and help the agent plan actions by simulating potential results.
- **Model-Free Methods:** agent learns directly from experience by interacting with the environment and adjusting its actions based on feedback.