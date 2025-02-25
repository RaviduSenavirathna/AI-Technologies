Unsupervised Learning is a type of machine learning where the model works without labelled data. It learns patterns on its own by grouping similar data points or finding hidden structures without any human intervention.

- It is used for tasks like clustering, dimensionality reduction and Association Rule Learning.
- Helps identify hidden patterns in data
- Useful for grouping, compression and anomaly detection

Unsupervised learning are again divided into **three main categories** based on their purpose: 

- **[[Clustering]]:** group data points into clusters based on their similarities or differences.
- **[[Association Rule]]:** simplify datasets by reducing the number of features while retaining the most important information.
- **[[Dimensionality Reduction]]:** Find patterns between items in large datasets typically in market basket analysis.


## Clustering Algorithms
Clustering is an unsupervised machine learning technique that groups unlabeled data into clusters based on similarity. Its goal is to discover patterns or relationships within the data without any prior knowledge of categories or labels.

- Groups data points that share similar features or characteristics.
- Helps find natural groupings in raw, unclassified data.
- Commonly used for customer segmentation, anomaly detection and data organization.
- Works purely from the input data without any output labels.
- Enables understanding of data structure for further analysis or decision-making.

**Some common clustering algorithms:** 
[[K-Means]] : Groups data into K clusters based on how close the points are to each other.
Hierarchical : Creates clusters by building a tree step-by-step, either merging or splitting groups.
[[DBSCAN]] : Finds clusters in dense areas and treats scattered points as noise.
Mean-Shift : Discovers clusters by moving points toward the most crowded areas.
Spectral Clustering: Groups data by analyzing connections between points using graphs.


## Association Rule Learning
Association rule learning is a rule-based unsupervised learning technique used to discover interesting relationships between variables in large datasets. It identifies patterns in the form of “if-then” rules, showing how the presence of some items in the data implies the presence of others.

- Finds frequent item combinations and the rules connecting them.
- Commonly used in market basket analysis to understand product purchase relationships.
- Helps retailers design promotions and cross-selling strategies.

**Some common Association Rule Learning algorithms:** 
Apriori Algorithm: Finds patterns by exploring frequent item combinations step-by-step.
FP-Growth Algorithm: An Efficient Alternative to Apriori. It quickly identifies frequent patterns without generating candidate sets.
Eclat Algorithm: Uses intersections of itemsets to efficiently find frequent patterns.
Efficient Tree-based Algorithms: Scales to handle large datasets by organizing data in tree structures.

## Dimensionality Reduction
Dimensionality reduction is the process of decreasing the number of features or variables in a dataset while retaining as much of the original information as possible. This technique helps simplify complex data making it easier to analyze and visualize. It also improves the efficiency and performance of machine learning algorithms by reducing noise and computational cost.

- It reduces the dataset’s feature space from many dimensions to fewer, more meaningful ones.
- Helps focus on the most important traits or patterns in the data.
- Commonly used to improve model speed and reduce overfitting.

**Here are some popular Dimensionality Reduction algorithms:**
Principal Component Analysis (PCA): Reduces dimensions by transforming data into uncorrelated principal components.
Non-negative Matrix Factorization (NMF): Breaks data into non-negative parts to simplify representation.
Locally Linear Embedding (LLE): Reduces dimensions while preserving the relationships between nearby points.
Isomap: Captures global data structure by preserving distances along a manifold.



# Applications
- **Customer Segmentation:** Algorithms cluster customers based on purchasing behavior or demographics, enabling targeted marketing strategies.
- **Anomaly Detection:** Identifies unusual patterns in data, aiding fraud detection, cybersecurity and equipment failure prevention.
- **Recommendation Systems:** Suggests products, movies or music by analyzing user behavior and preferences.
- **Image and Text Clustering:** Groups similar images or documents for tasks like organization and content recommendation.
- **Social Network Analysis:** Detects communities or trends in user interactions on social media platforms.
