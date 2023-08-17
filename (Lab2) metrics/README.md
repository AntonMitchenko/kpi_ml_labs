 # 2. Metrics
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



