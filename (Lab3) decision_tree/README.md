# 3. Decision Tree
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

