# Credit-Risk-Resampling

## Background
Credit risk poses a classification problem that’s inherently imbalanced. The reason is that healthy loans easily outnumber risky loans. For this Challenge, you’ll use various techniques to train and evaluate models with imbalanced classes. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose was to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* The data was on loan size, interest rate, borrower income, devt to income, number of accounts, derogatory marks, total debt and loan status.
  
* Based on the data of loan status, there were 75,036 healthy loans and only 2,500 high risk loans. There is a big difference between the two.
  
* There was a few steps to go through in order to get the desired outcome
  1. Bring in the data
  2. Split the data into training and testing sets
  3. Clean up the data
  4. Evaluate the results
     
* Method used to predict the data was LogisticRegression. Then I used the Resmapling Method to bring in more data to be able to compare predictions to the original data.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    1. Precision was 100% for healthy loans and 85% for high risk loans. True positive cases.
    2. Recall was 99% for healthy loans and 91% for high risk loans. These numbers correlate to the measure of accuracy at predicting those positive cases.
    3. Support shows the number of data points used for each occurence with healthy loans at 18,765 and high risk loans at 619. Data is not balanced.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    1. Precision was 100% for healthy loans and 84% for high risk loans. True positive cases.
    2. Recall was 99% for healthy loans and 99% for high risk loans. These numbers correlate to the measure of accuracy at predicting those positive cases.
    3. Support shows the number of data points used for each occurence with healthy loans at 18,765 and high risk loans at 619. Data is not balanced. Seems as though with the resample method, the recall accuracy is much higher for high risk loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?

   Although the recall accuracy was much better in the second model, the results were very similar for both. Based on the results, there is not much of a difference on how either model performed.
  
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

  There needs to be an equal amount of occurences for both the healthy loans and high risk loans so that we can get a much better prediction result to compare. The data is imbalanced not giving us the accuracy we need to make an accurate prediction.
  
