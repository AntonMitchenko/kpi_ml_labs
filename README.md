# My completed laboratory for KPI
In this repository, I posted my version of the laboratory work in open access.

Each folder contains several files:
> 1) Date folder (in which the dataset is stored)
> 2) Main file (code of our program)
> 3) The task that was posted by the teacher

Each main file is a file as type `"IPYNB" (.ipynb)` that was pre-launched, and you can see it running.

# There are 5 labs in total

  ## 1. Numpy & Pandas
  
  Numpy
  > NumPy plays a crucial role in machine learning as a foundational library, providing efficient and versatile tools for handling numerical data. Its multi-dimensional arrays enable seamless storage and manipulation of datasets, making it a cornerstone for data preprocessing, feature extraction, and model training. NumPy's mathematical functions and broadcasting capabilities facilitate complex computations essential for algorithm implementation. Integrating seamlessly with other machine learning libraries, NumPy forms an integral part of the data manipulation and numerical computation pipeline that underpins various stages of the machine learning workflow.
> 
  Pandas
 > Pandas is a vital library in the field of machine learning, offering powerful tools for data manipulation and analysis. With its DataFrame and Series data structures, Pandas simplifies data handling, transformation, and exploration, making it indispensable for tasks like data preprocessing, cleaning, and feature engineering. Its functionalities for grouping, aggregation, and merging are pivotal in preparing data for model training. Furthermore, Pandas' seamless integration with other machine learning libraries streamlines the process of loading, manipulating, and transforming datasets, contributing significantly to the efficiency and effectiveness of the machine learning pipeline.
    
  ## 2. Metrics
> Metrics in machine learning are quantitative measures that are used to evaluate the performance of models. They allow you to evaluate how well the model performs its tasks by comparing its predictions with actual values or classes. Metrics play a key role in model selection, hyperparameter tuning, results analysis, and comparison of different machine learning methods.

Depending on the type of problem, such as classification, regression, or clustering, the metrics may vary.

1. Accuracy: Accuracy measures the ratio of correctly predicted instances to the total number of instances. It's a straightforward metric for classification tasks, but it might not be suitable for imbalanced datasets.

2. Precision: Precision quantifies the proportion of true positive predictions among all positive predictions. It's crucial when minimizing false positives is important, such as in medical diagnoses.

3. Recall (Sensitivity or True Positive Rate): Recall calculates the ratio of true positive predictions to the actual positive instances. It's important when minimizing false negatives is critical, like identifying all relevant documents in information retrieval.

<p align="center">
  <img src="http://kflu.github.io/2016/08/26/2016-08-26-visualizing-precision-recall/2016-08-26-visualizing-precision-recall-1.png"/>
</p>

4. F1-Score: The F1-score is the harmonic mean of precision and recall. It provides a balance between precision and recall and is useful when there's an uneven class distribution.

<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:828/0*Dn7_MxfJpHj5jZa4.gif"/>
</p>

5. Mean Squared Error (MSE): MSE is a common metric for regression tasks. It calculates the average of squared differences between predicted and actual values, giving more weight to larger errors.

<p align="center">
  <img src="https://images.squarespace-cdn.com/content/v1/5acbdd3a25bf024c12f4c8b4/1600368657769-5BJU5FK86VZ6UXZGRC1M/Mean+Squared+Error.png?format=1500w"/>
</p>

<p align="center">
  <img src="https://suboptimal.wiki/images/mse_5.jpg" width="350" height="200"/>
</p>

<p align="center">
  <img src="https://suboptimal.wiki/images/mse_4.jpg" width="350" height="200"/>
</p>

6. Root Mean Squared Error (RMSE): RMSE is the square root of the MSE. It's more interpretable as it's in the same unit as the target variable, making it a popular choice for evaluating regression models.

7. Area Under the ROC Curve (AUC-ROC): AUC-ROC quantifies a classifier's ability to distinguish between classes. It plots the true positive rate against the false positive rate and provides a single value representing overall performance.

<p align="center">
  <img src="https://i0.wp.com/sefiks.com/wp-content/uploads/2020/12/roc-curve-original.png?fit=726%2C576&ssl=1" width="600" height="400"/>
</p>

8. Area Under the Precision-Recall Curve (AUC-PR): AUC-PR focuses on the trade-off between precision and recall. It's particularly useful when dealing with imbalanced datasets and provides insights into model performance at different prediction thresholds.

<p align="center">
  <img src="https://cdn-images-1.medium.com/max/437/1*dHeKnaFtqxnMqLfCdJz5bA.png" width="600" height="400"/>
</p>

9. Confusion Matrix: Although not a single metric, the confusion matrix provides a comprehensive view of a model's performance by showing true positives, true negatives, false positives, and false negatives.

<p align="center">
  <img src="https://user-images.githubusercontent.com/15989924/104855460-c6130600-58c1-11eb-8475-f7337a092c77.png" width="600" height="400"/>
</p>

10. MAPE, or Mean Absolute Percentage Error, is a metric commonly used to measure the accuracy of predictions in forecasting and regression tasks. It provides insight into how well a model's predictions match the actual values as a percentage of the actual values. 

<p align="center">
  <img src="https://i.imgur.com/YYMpqUY.jpg" width="300" height="125"/>
</p>

<p align="center">
  <img src="https://i.imgur.com/HPlrPmu.jpg" width="600" height="400"/>
</p>


  ## 3. Decision Tree
> A decision tree is a popular machine learning algorithm used for both classification and regression tasks. It is a tree-like structure that represents a sequence of decisions and their potential consequences. Decision trees recursively partition the data into subsets based on the values of input features, leading to a hierarchical structure where each internal node represents a decision based on a feature, each branch represents an outcome of that decision, and each leaf node represents a prediction or classification label.

<p align="center">
  <img src="https://images.datacamp.com/image/upload/v1677504957/decision_tree_for_heart_attack_prevention_2140bd762d.png"/>
</p>

Decision trees have various parameters that allow you to control their behavior, prevent overfitting, and customize their performance. Here are some important parameters commonly found in decision tree algorithms:

1. Criterion: This parameter determines the function to measure the quality of a split. Common criteria include "gini" for the Gini impurity and "entropy" for information gain. Gini measures the probability of a random sample being misclassified, while entropy measures the disorder or uncertainty in the data.
   
  * Gini
    >The gini impurity measures the frequency at which any element of the dataset will be mislabelled when it is randomly labeled.
    >The minimum value of the Gini Index is 0. This happens when the node is pure, this means that all the contained elements in the node are of one unique class. Therefore, this node will not be split again. Thus, the optimum split is chosen by the features with less Gini Index. Moreover, it gets the maximum value when the probability of the two classes are the same.

  * Entropy
     >Entropy is a measure of information that indicates the disorder of the features with the target. Similar to the Gini Index, the optimum split is chosen by the feature with less entropy. It gets its maximum value when the probability of the two classes is the same and a node is pure when the entropy has its minimum value, which is 0:
     
 <p align="center">
  <img src="https://thatascience.com/wp-content/uploads/2018/10/ginientropy.jpg" width="400" height="200"/>
 </p>

  More info about criterions ***[HERE](https://quantdare.com/decision-trees-gini-vs-entropy/)***

2. Max Depth: Limits the maximum depth of the tree. Setting this parameter can help prevent overfitting by controlling how deep the tree can grow.
   
 <p align="center">
  <img src="https://1329420134-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-LagOeJ2nL90MQERwhxy%2F-LjmGR4-Zkpsp-CXV3zt%2F-Lk-zlkug29fjZ6T44mL%2Fimage.png?alt=media&token=f775f1ce-2256-4172-af1b-e66e916ec127"/>
 </p>
 
3. Min Samples Split: Specifies the minimum number of samples required to split an internal node. This helps prevent splits on small subsets, which might lead to overfitting.

 <p align="center">
  <img src="https://1329420134-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-LagOeJ2nL90MQERwhxy%2F-LjmGR4-Zkpsp-CXV3zt%2F-Lk-zrrQar1T7mfpJ4jY%2Fimage.png?alt=media&token=75b26a95-2227-4832-8860-8e1086a4743b"/>
 </p>
 
4. Min Samples Leaf: Sets the minimum number of samples required to be in a leaf node. Similar to min_samples_split, this parameter helps control overfitting by ensuring that leaves have a minimum amount of data.
 
 <p align="center">
  <img src="https://1329420134-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-LagOeJ2nL90MQERwhxy%2F-LjmGR4-Zkpsp-CXV3zt%2F-Lk-zxxgBiLpOxwn1Fzn%2Fimage.png?alt=media&token=68c7cfa8-2a50-4cfa-a161-9e77e664c4bf"/>
 </p>
 
5. Max Features: Determines the number of features to consider when looking for the best split. It can be an absolute number or a fraction of the total features.

6. Splitter: This parameter defines the strategy for selecting the best feature to split on. It can be "best" to choose the best split or "random" to choose the best random split.

7. Class Weights: Assigns weights to classes, which can be useful when dealing with imbalanced datasets. It adjusts the impact of different classes on the criterion for splitting.

8. Random State: Provides a seed for the random number generator used for random decisions, making the results reproducible.

9. Presort: Determines whether to presort the data for faster fitting. It's helpful for smaller datasets but can slow down training for larger datasets.

  `Good guide about decion tree with examples` ***[HERE](https://julienbeaulieu.gitbook.io/wiki/sciences/machine-learning/decision-trees)***

  ## 4. K-Nearest Neighbors Method
  > The K-Nearest Neighbors (KNN) method is a simple machine learning algorithm used for classification and regression tasks. It works by finding the "k" closest data points (neighbors) to a given input point in a feature space. For classification, the majority class among these neighbors determines the class of the input point. For regression, the average (or weighted average) of the neighbors' target values is used to predict the target value for the input point. KNN relies on the assumption that similar data points tend to have similar outcomes.

 <p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:828/format:webp/0*34SajbTO2C5Lvigs.png"/>
 </p>
 
`Good guide about KNN with examples` ***[HERE](https://medium.com/swlh/k-nearest-neighbor-ca2593d7a3c4)***


  ## 5. Clustering
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

<p align="center">
  <img src="https://github.com/AntonMitchenko/kpi_ml_labs/blob/main/assets/image/1621725540_catworking.gif"/>
</p>


