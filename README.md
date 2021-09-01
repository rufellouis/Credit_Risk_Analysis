# Credit_Risk_Analysis

# Overview
To predict Credit Risk, using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the dataset was oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the ClusterCentroids algorithm followed by a Logistic regression algorithm to make predictions. Then, a combinatorial approach of over and undersampling using the SMOTEENN algorithm was employed on the data, followed by a Logistic regression algorith to make predictions. Next, a comparison was made between two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, and predictions were made using each.   All machine learning algorithm predictions were evaluated using a confusion matrix, accuracy score, precision & recall scores, as well as f1 scores.  This repo emcompases the jupyter notesbooks that contain the python code to run the above analyses and this repo also contains the summary of the same, here in the README file.

# Results
                          For RandomOverSampling and LogisticRegression:
![image](https://user-images.githubusercontent.com/31424076/131608235-6be5aa08-9b65-462d-8968-17fd837a0c39.png)
Balanced Accuracy Score: 0.54

                          For RandomOverSampling using SMOTE and LogisticRegression:
                          
![image](https://user-images.githubusercontent.com/31424076/131608361-1701884a-8853-41cd-abaa-4541067c0ee0.png)
Balanced Accuracy Score: 0.78

                          For UnderSampling using CLUSTERCENTROIDS and LogisticRegression:
                          
![image](https://user-images.githubusercontent.com/31424076/131608465-0d9828ff-0e18-4241-96e3-50409bdf4fa7.png)
Balanced Accuracy Score: 0.74

                          For CombinationOverUnderSampling using SMOTEENN and LogisticRegression:
                          
![image](https://user-images.githubusercontent.com/31424076/131608649-b2e47f99-d7fe-4d7d-a15d-7103a58856ac.png)
Balanced Accuracy Score: 0.78

                          For BalancedRandomForestClassifier:
![image](https://user-images.githubusercontent.com/31424076/131609138-89584e8c-aec2-4e83-8dea-bc4faa2a3f5e.png)
Balanced Accuracy Score: 0.75

                          For EasyEmsembleAdaBoostClassifier:
![image](https://user-images.githubusercontent.com/31424076/131609297-4cc7d874-d700-45b4-a47b-1851ba8ec372.png)
Balanced Accuracy Score: 0.67
# Summary
Even though the EasyEmsembleAdaBoostClassifier had the best F1 scores for both Credit Risk conditions in the y-variable, compared to all other classifiers, its overall Accuracy is 10% below the leaders like SMOTE and SMOTEENN, however, none of the algoriths and sampling methods did a great job at identifying the under-respresented target class of 'high_risk' as oppossed to 'low_risk' the more voluminous target class.  But when comparing F1 scores, a more equalized approach across both prediction classes, it is clear that EasyEmsembleAdaBoostClassifier performed the best with scores of 0.46 and 1.00 respectively for the classes of 'high_risk' and 'low_risk.'  
