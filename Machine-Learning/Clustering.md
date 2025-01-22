Clustering is an unsupervised machine learning technique used to group similar data points together without using labelled data. It helps discover hidden patterns or natural groupings in datasets by placing similar data points into the same cluster.

- Discover the natural grouping or structure in unlabeled data without predefined categories.
- Data points are assigned to clusters based on similarity or distance measures.
- Uses Euclidean distance, cosine similarity or other metrics depending on data type and clustering method.

![[{7F3A18ED-790C-48ED-8AC3-0C81C15456F3}.png]]

### Types of Clustering
- **1. Hard Clustering**
	Hard clustering assigns each data point to exactly one cluster. A data point cannot belong to multiple clusters, making the grouping clear and easy to interpret.

- **2. Soft Clustering**
	Soft clustering allows a data point to belong to multiple clusters with different probabilities. Instead of assigning a strict cluster, it gives a degree of membership to each cluster.


## Clustering Methods
Clustering methods can be classified on the basis of how they form clusters.

##### 1. Centroid based Clustering
Centroid based clustering groups data points around central points called centroids. Each cluster is represented by the average of its points and data points are assigned to the nearest centroid.

**Algorithms:
- **[[K-Means]]:** Iteratively assigns points to nearest centroid and recalculates centroids to minimize intra cluster variance.
- K-medoids: Similar to K-means but uses actual data points (medoids) as centers, robust to outliers.

| Advantages                            | Limitations                                     |
| ------------------------------------- | ----------------------------------------------- |
| Fast and scalable for large datasets. | Requires choosing number of clusters in advance |
| Simple to implement and interpret.    | Sensitive to initialization and outliers.       |
|                                       | Not suitable for non spherical clusters.        |

##### 2. Density based Clustering
Density based clustering identifies clusters as regions where data points are densely packed together. Points in low density areas are treated as noise.

**Algorithms:
- DBSCAN: Groups points with sufficient neighbors; labels sparse points as noise.
- OPTICS: Extends DBSCAN to handle varying densities.

| Advantages                                    | Limitations                                                  |
| --------------------------------------------- | ------------------------------------------------------------ |
| Handles clusters of varying shapes and sizes. | Difficult to choose parameters like epsilon and min points.  |
| Does not require cluster count upfront.       | Less effective for varying density clusters (except OPTICS). |
| Effective in noisy datasets.                  |                                                              |

##### 3. Connectivity based Clustering
Connectivity based or Hierarchical clustering builds clusters by gradually merging or splitting groups of data points. It creates a tree like structure called a dendrogram that shows relationships between clusters.

**Approaches:
- Agglomerative: Starts with each point as a cluster and merges them step by step.
- Divisive: Starts with one cluster and splits it into smaller clusters.

| Advantages                                    | Limitations                                  |
| --------------------------------------------- | -------------------------------------------- |
| Provides a full hierarchy, easy to visualize  | Computationally intensive for large datasets |
| No need to specify number of clusters upfront | Merging/splitting decisions are irreversible |
|                                               | Choosing parameters can be difficult         |

##### 4. Distribution-based Clustering

Distribution based clustering assumes that data points come from a mixture of probability distributions. Each cluster is modelled as a statistical distribution.

**Algorithm:
- Gaussian Mixture Model (GMM): Fits data as a weighted mixture of Gaussian distributions, assigns data points based on likelihood

| Advantages                         | Limitations                              |
| ---------------------------------- | ---------------------------------------- |
| Flexible cluster shapes            | Requires specifying number of components |
| Provides probabilistic memberships | Computationally more expensive           |
| Suitable for overlapping clusters  | Sensitive to initialization              |

##### 5. Fuzzy Clustering
Fuzzy clustering allows data points to belong to multiple clusters with different degrees of membership. It is useful when cluster boundaries are not clear.

**Algorithm:
- Fuzzy C-Means: Similar to K-means but with fuzzy memberships updated iteratively

| Advantages                           | Limitations                                |
| ------------------------------------ | ------------------------------------------ |
| Models data ambiguity explicitly     | Choosing fuzziness parameter can be tricky |
| Useful for complex or imprecise data | Slightly higher computational cost         |
