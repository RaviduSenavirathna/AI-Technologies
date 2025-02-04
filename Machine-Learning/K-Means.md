K-Means Clustering groups similar data points into clusters without needing labeled data. It is used to uncover hidden patterns when the goal is to organize data based on similarity. "*k*" represents the number of groups or clusters we want to classify our items into.

- Helps identify natural groupings in unlabeled datasets
- Works by grouping points based on distance to cluster centers
- Commonly used in customer segmentation, image compression, and pattern discovery
- Useful when you need structure from raw, unorganized data


Step 1:
* Clusters the data into `k` groups where `k` is predefined.
Step 2:
- Select `k` points at random as cluster centers.
Step 3:
- Assign objects to their closest cluster center according to the Euclidean distance function.
Step 4:
- Calculate the centroid or mean of all objects in each cluster.
Step 5:
- Repeat steps 2,3 and 4 until the same points are assigned to each cluster in consecutive rounds (iterations), or the difference between the values of the objective function in two consecutive iterations drops below a threshold. 