# credit-risk-classification

# Module 12 Report Template

## Overview of the Analysis



The purpose of this analysis is to tell whether a borrower is credit-worthy and to prevent the lender from losing money.  The banks would like to know whether the loan is safe to give or not. We will use machine learning methods to predict whether there are healthy or unhealthy loans.  The data set we are using shows lending activity from a peer-to-peer lending services company.  We did value counts of the loan status with 0 being healthy and 1 being unhealthy.  The method we used is. LogisticRegression model and OverSharingSampling. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * The Logistic Regression model produced a 99% accuracy score.
![LogisticRegression](https://github.com/alebridegroom/credit-risk-classification/assets/91504694/6b461060-244f-468d-922c-b3391f55a0f3)

The recall score was 100% for healthy loans but not so high forthe non healthy loans which was a 87%.  This tells us that the model will predict healthy loans rather than unhealthy loans and it will predict unhealthy loans 87% of the time which is not too good if you are the CEO of the company.   This could be due to the data being unbalanced which we showed the the majority of the data is in the  healthy loans (75036)  and only 2500 of the data is in the unhealthy category.

<img width="303" alt="logisitcmatrix" src="https://github.com/alebridegroom/credit-risk-classification/assets/91504694/73c800f5-5384-40a1-a541-bc9ee42c5fc1">

For the confusion matrix 18679 were identified as healthy loans coorectly and 558 unhealthy loans were identified correctly, so for recall, it only identifies the true negatives 89% of the time.




* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * For the second one, the random over sampling had a accuracy score of 99%
  * ![randomoversampling](https://github.com/alebridegroom/credit-risk-classification/assets/91504694/54d91819-0623-4b12-9026-097c25210bfd)
 
  * this one has the same precision as the previous one but a higher recall score meaning it can both correctly identify the true positives and true negatives 100% of the time.


  

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* The random over sampling seemed to perform the best since we balanced more of the data.
* it is more important to predict the 1's (unhealthy loans) because we could possibly loose buyers if we suspect them of fraud but aren't actually frauds and also we need to correctly identify fraud so the company doesn't loose money.

If you do not recommend any of the models, please justify your reasoning.
