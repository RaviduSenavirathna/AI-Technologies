Density _ Based Spatial Clustering of Application with Noise.
- Groups points based of **density.**
- Identifies 

Key Parameters
- Epsilon : Neighborhood radius
- MinPts : Minimum points to form a cluster.

Types of Points:
- Core Point : >= MinPts within Epsilon
- Border Point : Near a core point
- Noise Point : Isolated


Steps:
1. Pick a point
2. Find neighbors with E
3. If enpugh -> form cluster
4. Expand cluster
5. Repat

