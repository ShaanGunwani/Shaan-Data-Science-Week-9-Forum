# Shaan-Data-Science-Week-9-Forum

1.	KMeans Clustering: KMeans is an iterative algorithm dividing data into clusters. Initially, K clusters are defined, and data points are assigned to the nearest of K randomly initialized centroids. Centroids are recalculated based on the assigned data points until convergence. This iterative process forms the clusters.

   - Results:
     - Silhouette Score: 0.603
     - Davies-Bouldin Index: 0.492
     - Rand Score: 0.014
     - Calinski and Harabasz Score: 1719.56

2. Mean Shift Clustering:
MeanShift identifies clusters based on data density without requiring a predetermined cluster count. It shifts data points toward the mean within a defined radius, repeating until convergence to locate centroids. Cluster centroids are then assigned data points.

   - Results:
     - Silhouette Score: 0.585
     - Davies-Bouldin Index: 0.505
     - Rand Score: 0.0146
     - Calinski and Harabasz Score: 1607.39

3. Agglomerative Clustering:
Agglomerative Clustering is hierarchical, initially assigning each observation to its own cluster. It merges clusters iteratively by combining the closest ones until there's one cluster with all observations. Proximity between clusters determines their merging.

   - Results:
     - Silhouette Score: 0.544
     - Davies-Bouldin Index: 0.479
     - Rand Score: 0.010
     - Calinski and Harabasz Score: 1173.90

4. Spectral Clustering:
Spectral Clustering utilizes eigenvectors from a similarity matrix to cluster data. It reduces dimensions by computing eigenvectors from the similarity matrix, enabling traditional clustering methods (like KMeans) on the reduced dimensions.

   -Results:
     - Silhouette Score: 0.370
     - Davies-Bouldin Index: 0.380
     - Rand Score: 0.00021
     - Calinski and Harabasz Score: 17.904

Findings:
- Silhouette Score (best to worst): KMeans > Mean Shift > Agglomerative Clustering > Spectral Clustering
- DBI (best to worst): Spectral Clustering > Agglomerative Clustering > KMeans > Mean Shift
- Rand Score (best to worst): Mean Shift > KMeans > Spectral Clustering > Agglomerative Clustering
- Calinski and Harabasz Score (best to worst): KMeans > Mean Shift > Agglomerative Clustering > Spectral Clustering 
