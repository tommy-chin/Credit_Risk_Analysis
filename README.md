# Credit_Risk_Analysis
## Purpose
A P2P lending services company named Fast Lending was interested in using machine learning to predict the credit risk of its potential loaners. To perform this credit risk data analysis, credit card data from a company named LendingClub was used. This analysis uses both imbalanced-learn and skikit-learn libraries for its machine learning. These libraries are used to create various different models to better understand which models have the most ideal accuracy, precision, and recall scores for high credit risk loaners. 
## Results
For this data analysis, six different machine learning models were used which are listed below.
* Naive Random Sampling
  * The accuracy score was 62.85%, the precision score for high risk was 1%, and the recall score for high risk was 54%.
![Naive Random Samplijng.PNG](https://github.com/tommy-chin/Credit_Risk_Analysis/blob/main/Images/Naive%20Random%20Samplijng.PNG)
* Smote Oversampling
  * The accuracy score was 61.57%, the precision score for high risk was 1%, and the recall score for high risk was 57%.
![Smote Oversampling.PNG](https://github.com/tommy-chin/Credit_Risk_Analysis/blob/main/Images/Smote%20Oversampling.PNG)
* Undersampling
  * The accuracy score was 59.03%, the precision score for high risk was 1%, and the recall score for high risk was 61%.
![Undersampling.PNG](https://github.com/tommy-chin/Credit_Risk_Analysis/blob/main/Images/Undersampling.PNG)
* Combination Sampling
  * The accuracy score was 52.31%, the precision score for high risk was 1%, and the recall score for high risk was 61%.
![Combination Sampling.PNG](https://github.com/tommy-chin/Credit_Risk_Analysis/blob/main/Images/Combination%20Sampling.PNG)
* Balanced Random Forest
  * The accuracy score was 78.78%, the precision score for high risk was 4%, and the recall score for high risk was 67%.
![Balanced Random Forest.PNG](https://github.com/tommy-chin/Credit_Risk_Analysis/blob/main/Images/Balanced%20Random%20Forest.PNG)
* Easy Ensemble AdaBoost
  * The accuracy score was 92.54%, the precision score for high risk was 7%, and the recall score for high risk was 91%.
![Easy Ensemble AdaBoost.PNG](https://github.com/tommy-chin/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20AdaBoost.PNG)

## Summary
As seen in the results, the naive random sampling, smote oversampling, undersampling, and combination sampling had very similar results as they all had mediocre accuracy scores ranging from 52.31% to 62.85%, precision scores for high risk at 1%, and mediocre recall scores ranging from 54% to 61%. However, when looking at the Balanced Random Forest and Easy Ensemble AdaBoost classifiers, both of them have much higher accuracy scores at 78.78% and 92.54% respectively. The precision scores for high risk were slightly higher at 4% for Balanced Random Forest and 7% for Easy Ensemble AdaBoost. Although the recall score for Balanced Random Forest was not much higher at 67%, Easy Ensemble AdaBoost had a recall score of 91% which was much higher than all of the other models created. Although the Easy Ensemble AdaBoost model has the highest scores across the board, it is not recommended to use any of these models for credit risk analysis due to the precision scores for all of the models being low. A low precision score means that the model is detecting a high number of false positives which in the case of high risk credit loaners means that many potential loaners will be flagged as high risk. 
