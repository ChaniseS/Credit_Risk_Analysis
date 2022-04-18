# Credit_Risk_Analysis
### Overview:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

### Results:
The below results show the Balanced Accuracy Score and the Precision and Recall scores of all six machine learning models.
1. **Naive Random Oversampling**
    - For the Balanced Accuracy test it came out to be 64%, the precision for the high_risk has a very low positivity at 1% and the recall is 60%.
<img width="790" alt="Screen Shot 2022-04-17 at 8 43 17 PM" src="https://user-images.githubusercontent.com/95304025/163738475-e449f02e-9972-498c-9636-0c9f51e21ce4.png">

2. **SMOTE Oversampling**
    - For the Accuracy Score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall.
<img width="803" alt="Screen Shot 2022-04-17 at 8 53 53 PM" src="https://user-images.githubusercontent.com/95304025/163738892-55dff081-faec-4ced-a71f-cd57f80bb719.png">

3. **Undersampling**
     - The balanced accuracy score is 54% overall, the precision is at 1% and the recall is 69%.
%<img width="797" alt="Screen Shot 2022-04-17 at 8 59 56 PM" src="https://user-images.githubusercontent.com/95304025/163739133-268fd61f-e1c7-4fe9-8d7f-20b39dafbeef.png">

4. **Combination (Over and Under) Sampling**
    - The balanced accuracy score is 65% overall, the precision is at 1% and the recall is 72%.
<img width="797" alt="Screen Shot 2022-04-17 at 9 02 53 PM" src="https://user-images.githubusercontent.com/95304025/163739243-b3af8901-4021-498d-ae17-b1fc06dd0ba4.png">

5. **Balanced Random Forest Classifier**
    -  The accuracy score is 79% the precision is 99% and the recall is 87%.
<img width="785" alt="Screen Shot 2022-04-17 at 9 07 29 PM" src="https://user-images.githubusercontent.com/95304025/163739470-971361fd-0b5f-4b3f-8dfe-1c4a978fb4e5.png">

6. **Easy Ensemble AdaBoost Classifier**
    -The accuracy score is 93% the precision is 99% and the recall is 94%.
<img width="785" alt="Screen Shot 2022-04-17 at 9 09 53 PM" src="https://user-images.githubusercontent.com/95304025/163739593-76768619-1f81-4710-ac66-d8c5f86667dd.png">


## Summary:

After we reviewed the above six models:
The **EasyEnsembleClassifer model** has proven to be the best with an accuracy rate of 93%.

  -The sensitivity rate (aka recall) was also the highest at 94% compared to the other models.
  
  -The result for predicting "Low Risk" was also the highest with the sensitivity rate at 94% and an F1 score of 97%. 
  
  -Therefore, if a model needed to be recommended to perform this type of analysis, then this one would be the clear choice.
