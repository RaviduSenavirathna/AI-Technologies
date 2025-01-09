Classification is a supervised machine learning technique used to predict labels or categories based on input data. The goal is to assign each data point to a predefined class.

![[{C6805EBB-016E-4BE5-8030-5BECCE679C5A}.png]]
## Types of Classification

The process of sorting data into categories based on specific features or characteristics. There are different types of classification problems depending on how many categories (or classes) we are working with and how they are organized.

#### 1. Binary Classification
This is the simplest kind of classification. The goal is to sort the data into two distinct categories. Imagine a system that sorts emails into either spam or not spam. It works by looking at different features of the email like certain keywords or sender details and decides whether it’s spam or not.

#### 2. Multiclass Classification
The data needs to be sorted into more than two categories. The model picks the one that best matches the input. Think of an image recognition system that sorts pictures of animals into categories like cat, dog and bird.


![[{60F4D921-037E-4624-8CEC-96E1F1A97206}.png]]

#### 3. Multi-Label Classification
Single piece of data can belong to multiple categories at once. Unlike multiclass classification where each data point belongs to only one class, multi-label classification allows datapoints to belong to multiple classes. A movie recommendation system could tag a movie as both action and comedy. The system checks various features (like movie plot, actors or genre tags) and assigns multiple labels to a single piece of data, rather than just one.


## Classification Algorithms Types
Now, for implementation of any classification model it is essential to understand Logistic Regression, which is one of the most fundamental and widely used algorithms in machine learning for classification tasks. There are various types of classifiers algorithms. Some of them are : 

1. **Linear Classifiers:** Linear classifier models create a linear decision boundary between classes. They are simple and computationally efficient. Some of the linear classification models are as follows: 
- [[Logistic-Regression]]
- [Support Vector Machines having kernel = 'linear'](https://www.geeksforgeeks.org/machine-learning/support-vector-machine-algorithm/)
- [Single-layer Perceptron](https://www.geeksforgeeks.org/python/single-layer-perceptron-in-tensorflow/)
- [Stochastic Gradient Descent (SGD) Classifier](https://www.geeksforgeeks.org/python/stochastic-gradient-descent-classifier/)

1. **Non-linear Classifiers:** Non-linear models create a non-linear decision boundary between classes. They can capture more complex relationships between input features and target variable. Some of the non-linear classification models are as follows:
- [K-Nearest Neighbours](https://www.geeksforgeeks.org/machine-learning/k-nearest-neighbours/)
- [Kernel SVM](https://www.geeksforgeeks.org/machine-learning/major-kernel-functions-in-support-vector-machine-svm/)
- [Naive Bayes](https://www.geeksforgeeks.org/machine-learning/naive-bayes-classifiers/)
- [Decision Tree Classification](https://www.geeksforgeeks.org/machine-learning/decision-tree/)
- [Ensemble learning classifiers:](https://www.geeksforgeeks.org/machine-learning/ensemble-classifier-data-mining/) 
- [Random Forests,](https://www.geeksforgeeks.org/dsa/random-forest-classifier-using-scikit-learn/) 
- [AdaBoost,](https://www.geeksforgeeks.org/machine-learning/implementing-the-adaboost-algorithm-from-scratch/) 
- [Bagging Classifier,](https://www.geeksforgeeks.org/machine-learning/What-is-Bagging-classifier/) 
- [Voting Classifier,](https://www.geeksforgeeks.org/machine-learning/ml-voting-classifier-using-sklearn/) 
- [Extra Trees Classifier](https://www.geeksforgeeks.org/machine-learning/ml-extra-tree-classifier-for-feature-selection/)
- [Multi-layer Artificial Neural Networks](https://www.geeksforgeeks.org/deep-learning/multi-layer-perceptron-learning-in-tensorflow/)