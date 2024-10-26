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
