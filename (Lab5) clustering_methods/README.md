# 5. Clustering
  > Clustering is a machine learning technique used for grouping similar data points together in an unsupervised manner. The goal is to find patterns or structures in the data without having predefined labels. One common clustering algorithm is K-Means. It works by iteratively assigning data points to the nearest cluster center and updating the centers based on the assigned points. The algorithm aims to minimize the distance between data points and their respective cluster centers. The result is a set of clusters where data points within the same cluster are more similar to each other than to those in other clusters. Clustering helps in exploring data, identifying natural groupings, and gaining insights into the underlying structure of the data.

  *There are many clustering methods, each suitable for different types of data and tasks. Some of the more popular clustering methods are listed below:*
  
  * `K-Means`: Splits data into a predetermined number of clusters by determining cluster centers and assigning points to the nearest center.
  ***[More about KNN](https://ealizadeh.com/blog/knn-and-kmeans/)***
    
<p align="center">
  <img src="https://ealizadeh.com/blog/knn-and-kmeans/img/202203092227_K-Means.png" width="300" height="300"/>
</p>  
    
  * `DBSCAN (Density-Based Spatial Clustering of Applications with Noise)`: Based on point density. It identifies high dot density areas as clusters and can detect outliers.

<p align="center">
  <img src="https://lh5.googleusercontent.com/VLwovohNM_KYh_NNJmG7ZzJF19HYnpr88hsCI5eHtafNjb63HQ6yYpxkwFuVagnDfrPrFqzWyzq9yp2bn25YtC-MHBaKU0M5ph5laf4gVL1JgwPhsKO9hsWyo5joIXY4F1Q11JIL"/>
</p>

 * `Hierarchical Clustering`: Creates a hierarchy of clusters, starting at each point as a single cluster and progressively merging the closest clusters.

   1) `Agglomerative Clustering`: This is a hierarchical clustering method, starting from each point as a separate cluster and sequentially merging the nearest clusters.
    
<p align="center">
  <img src="https://images.datacamp.com/image/upload/v1674149819/Dendrogram_of_Agglomerative_Clustering_Approach_4eba3586ec.png" width="600" height="600"/>
</p>

   2) `Divisive clustering`: On the other hand, divisive clustering is top-down because it starts by considering all the data points as a unique cluster. Then it separates them until all the data points are unique.

<p align="center">
  <img src="https://images.datacamp.com/image/upload/v1674149823/Dendrogram_of_Divisive_Clustering_Approach_8623354c7b.png" width="600" height="600"/>
</p>    

***[More about Hierarchical Clustering](https://www.datacamp.com/tutorial/introduction-hierarchical-clustering-python)***


*There are a couple of methods for finding the optimal number of clusters*
  
   1) Elbow Method:
   The essence of the method lies in graphical analysis, where the graph displays the number of clusters along the X axis and the sum of squared distances from points to the centers of their clusters along the Y axis. The "elbow" point on the graph usually indicates the optimal number of clusters, after which an increase in the number of clusters begins to give diminishing benefits in reducing intra-cluster variance.

<p align="center">
  <img src="https://www.oreilly.com/api/v2/epubs/9781788295758/files/assets/995b8b58-06f1-4884-a2a1-f3648428e947.png"/>
</p>  
 
   2) Average Silhouette Method:
This method evaluates the quality of clustering by measuring how much more similar points within one cluster are to each other than to points from other clusters. For each point, a silhouette coefficient is calculated, which can range from -1 to 1. A value closer to 1 indicates good clustering, and closer to -1 indicates that the point is in the wrong cluster. By calculating the average silhouette coefficient for all points, you can determine the optimal number of clusters, at which it will be maximum.
   
<p align="center">
  <img src="https://www.datanovia.com/en/wp-content/uploads/dn-tutorials/004-cluster-validation/figures/015-determining-the-optimal-number-of-clusters-k-means-optimal-clusters-wss-silhouette-2.png"/>
</p>  
   
   3) Prediction Strength Method:
This method measures the stability of clustering by dividing the data into subsets, performing clustering on each subset, and evaluating how strongly the clustering results are consistent across subsets. The higher the stability, the more reliable the selected number of clusters will be. The predictive strength method is especially useful when choosing the number of clusters for complex and noisy data.


