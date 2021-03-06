# Credit Risk Analysis Using Machine Learning
## Overivew of Analysis
* For this analysis I used my knowledge of Machine Learning to predict credit card risk.  
* I was given a dataset from Lending Tree.  With that I used the imbalanced-learn and scikit-learn libraries to build machine learning models and evaluate them using resampling
* I first oversampled the data using the SMOTE and RandomOverSampler algorithms
* Then undersampled the data using the ClusterCentroids algorithm
* Then used the SMOTEENN algorithm which is a combination of over and undersampling
* Finally I compared 2 models that reduce bias the (EasyEnsembleClassifier and BalancedRandomForestClassifier) to predict credit risk
## Results
* These are the results I found from each of the six machine learning models that I employed
  ### RandomOverSampler
   * **Balanced Accuracy Score:** 65%
   * **Precision Score:** 
     * 1% of actual high-risk loans were predicted high risk
     * 99% of actual low-risk loans were predicted low risk
    * **Recall:**
      * high-risk: 69%
      * low-risk: 60%
 ![](images/random_over_sampling.png)
 ### SMOTE Oversampling
 * **Balanced Accuracy Score:** 65%
   * **Precision Score:** 
     * 1% of actual high-risk loans were predicted high risk
     * 99% of actual low-risk loans were predicted low risk
    * **Recall:**
      * high-risk: 62%
      * low-risk: 68%
 ![](images/SMOTE.png)
 ### ClusterCentroids Undersampling
 * **Balanced Accuracy Score:** 54%
   * **Precision Score:** 
     * 1% of actual high-risk loans were predicted high risk
     * 99% of actual low-risk loans were predicted low risk
    * **Recall:**
      * high-risk: 69%
      * low-risk: 40%
 ![](images/Cluster_Centroids.png)
  ### SMOTEENN Combination Over and Under Sampling
 * **Balanced Accuracy Score:** 67%
   * **Precision Score:** 
     * 1% of actual high-risk loans were predicted high risk
     * 100% of actual low-risk loans were predicted low risk
    * **Recall:**
      * high-risk: 78%
      * low-risk: 55%
 ![](images/SMOTEENN.png)
 ### BalancedRandomForest Classifier
 * **Balanced Accuracy Score:** 68%
   * **Precision Score:** 
     * 88% of actual high-risk loans were predicted high risk
     * 100% of actual low-risk loans were predicted low risk
    * **Recall:**
      * high-risk: 37%
      * low-risk: 100%
 ![](images/random_forest.png)
### EasyEnsemble Classifier
 * **Balanced Accuracy Score:** 68%
   * **Precision Score:** 
     * 88% of actual high-risk loans were predicted high risk
     * 100% of actual low-risk loans were predicted low risk
    * **Recall:**
      * high-risk: 37%
      * low-risk: 100%
 ![](images/easy_ensemble.png)
## Summary
* In summary the Easy Ensemble Classifier and Balanced Random Forest Classifiers produced the highest balanced accuracy score of 68%
* They both also produced the highest precision scores.  
* I would recommend that to predict credit risk one should use either of these models, because the produced the highest accuracy scores but also had a good balance of the recall and precision scores as well.
