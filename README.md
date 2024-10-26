# Unsupervised Machine Learnings 


# 1. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
DBSCAN is a density-based clustering algorithm, ideal for datasets with noise and clusters of varying shapes and sizes.

**How It Works:**
Core Points: Points with at least min_samples points within a specified distance eps are core points.
Reachable Points: Points within the eps radius of a core point but not dense enough to be core points.
Noise: Points that do not belong to any cluster.

**Advantages:**

Can find arbitrarily shaped clusters.
Effectively handles outliers (noise).
No need to pre-define the number of clusters.
Disadvantages:
Performance can degrade on datasets with varying density.
Sensitive to eps and min_samples parameters.

![image](https://github.com/user-attachments/assets/cc54c2d0-6d5b-4b1e-9b85-569f418d08a9)

![image](https://github.com/user-attachments/assets/6a0256c3-c285-436f-924e-56c7b902f7db)

![image](https://github.com/user-attachments/assets/ff1e8c47-90d2-4845-83ca-c9476604dfe3)


# 2. Hierarchical Clustering
Hierarchical Clustering builds a hierarchy of clusters through a tree-like structure (dendrogram) and comes in two types:

Agglomerative: Bottom-up approach, where each point starts as its own cluster and merges with others iteratively.
Divisive: Top-down approach, where all points start in a single cluster, which splits until only individual points remain.

**How It Works (Agglomerative):**

Calculates the distance between clusters (e.g., single-linkage, complete-linkage, average-linkage).
Merges the closest clusters iteratively until a stopping criterion (e.g., a pre-defined number of clusters) is met.

**Advantages:**
No need to specify the number of clusters (though it can be set as a stopping criterion).
Effective for small to medium-sized datasets and hierarchical relationships.

**Disadvantages:**
Computationally expensive, especially for large datasets.
Choosing the distance measure (linkage criterion) impacts results.

![image](https://github.com/user-attachments/assets/6f3ebec6-c79b-4bfe-b1a1-43f3b9a3cda7)


![image](https://github.com/user-attachments/assets/dc3e4a94-6a70-43fc-b28d-95f0b4b2ea77)


# 3. K-Means Clustering
K-Means is a popular and straightforward algorithm that divides the data into a pre-defined number of clusters (k).

**How It Works:**
Initialize k cluster centroids randomly.
Assign each point to the nearest centroid.
Update centroids by calculating the mean of points in each cluster.
Repeat the assignment and update steps until convergence (when cluster assignments no longer change).

**Advantages:**
Simple to implement and computationally efficient.
Works well with large datasets and spherical-shaped clusters.

**Disadvantages:**
Requires specifying k (the number of clusters) in advance.
Sensitive to the initial placement of centroids (can lead to suboptimal results).
Assumes clusters are spherical and equally sized, which may not always be true.

![image](https://github.com/user-attachments/assets/5bad04f2-cb7b-40e5-ab7f-4ece85c34758)

![image](https://github.com/user-attachments/assets/6ba48279-01c1-49ff-b0ba-07c6c04ebc0b)

![image](https://github.com/user-attachments/assets/2a10353e-5413-4559-ae26-6cf21576aff0)




