# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * The model fitted with imbalanced data has a higher possibility of making these mistakes:

   a healthy loan (low-risk) is classified as a non-healthy loan (high-risk).
   a non-healthy loan (high-risk) is classified as a healthy loan (low-risk).

  <img width="242" alt="image" src="https://github.com/Elevate04/credit-risk-classification/assets/108631132/9533da59-04cf-47f1-9ee1-98cf70c02512">

  balanced_accuracy_score(y_test, LR_predictions) = 0.9520479254722232




* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * The model fitted with balanced (oversampled) data has a much lower possibility of making these mistakes:

    a healthy loan (low-risk) is classified as a non-healthy loan (high-risk).
    a non-healthy loan (high-risk) is classified as a healthy loan (low-risk).

    <img width="269" alt="image" src="https://github.com/Elevate04/credit-risk-classification/assets/108631132/66bb61c6-3b30-4822-aac6-f782a5852757">

    balanced_accuracy_score(y_test, LR_predictions) = 0.9520479254722232 = 0.9936781215845847



## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

  Logistic Regression model fitted with OverSampled data
  
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

The Logistic Regression model fitted with OverSampled data performed much better than the model fitted with Imbalanced data due to the data being balanced and generating a higher accuracy score and a higher recall, indicating that the model will make extremely fewer mistakes when classifying non-healthy loans.

If you do not recommend any of the models, please justify your reasoning.
