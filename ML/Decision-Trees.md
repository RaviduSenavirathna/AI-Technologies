Decision Tree is a Supervised Machine Learning Algorithm that uses a set of rules to make decisions like human. The intuition behind Decision Trees is that you use the dataset features to create ==yes/no== 	questions and continually split the dataset until you isolate all data points belonging to each class. Every time you ask a question you’re adding a ==node== to the tree. And the ==first node is called the root node==. Each node is connected to other nodes using branches. If you decide to stop the process after a split, the ==last nodes created are called leaf nodes==. Every time you answer a question, you’re also creating branches and segmenting the feature space into disjoint regions.

We can decide the best split by calculating the information gain resulting from each split using the following formula:
$$
Entropy=∑ -pi ~log_{2}~(pi)​​
$$
- The goal of a decision tree is to **reduce entropy** after each split.

$$
IG~ = ~E(parent) - ~∑ ~w_{i} ~~E(~child_{i}~)
$$
- Information Gain measures **how much a split improves purity**.

### Classification
Splits data step-by-step using different features to make a classification decision. During training, the model checks every possible feature and every possible split value to find the best way to divide the data.  A pure leaf node is a final node where all data points belong to the same class. In real-world data, perfectly pure leaf nodes are rare, so many leaf nodes contain a mix of classes. When a leaf node has mixed classes, the model uses majority voting.