# Module 12 Report Template

## Overview of the Analysis
  The purpose of this analysis is to build a logistic regression model to predict creditworthiness in a dataset of healthy and risky loans. Since we are dealing with a large dataset, we must create variables to differentiate between a healthy loan and a risky loan. These values were "0" and "1", which were under the "loan_status" column. These were are target values. Our features were the other columns including: loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt. The machine learning technique that we used was a logistic regression model which is a well-known model used for classification which will allow us to predict categories, in this case, whether a loan is healthy or risky. One of the first steps we used in this build, was to split the data between training and testing sets. The next category is the model, fit, predict, and evaluate method. The first step has already been done as we have picked the logistic regression model. Next is to fit the model into our data, this step allows the selected model to train with the training data provided. Third is the predict method, which classifies our testing features data, so it can allow it to match our target values of "0" and "1". Thus, this will give us the opportunity of how well the model fits using real data. The last stage is simply the result of how well, accurate, and precise our data is, this value will normally(and hopefully) range between zero and one. The closer this value gets to one, the more accurate the model is relative to our data. 
## Results
Key Word Definitions

Accuracy: measures of how often the model was correct

Precision: measures of how confident our model has made its  predictions

Recall: measures how correct our model was in classifying in differentiating the loan status class.

Description of Model 1 Accuracy, Precision, and Recall scores.
- Accuracy: 0.95, The accuracy of this model has a strong rating
- Precision: 0 = 1.00, 1 = 0.86, Precision rating is a solid score for our healthy loans, and a relatively strong score for our risky loans
- Recall:0 = 1.00, 1 = 0.91, Recall ratings are strong

Description of Model 2 Accuracy, Precision, and Recall scores.

- Accuracy score: 0.99, The accuracy of this model has a very strong rating
- Precision score: 0 = 1.00, 1 = 0.86, Precision ratings for both seem to emulate our first machine learning model
- Recall score: 0 = 1.00, 1 = 0.99, The recall value for risky loans is very strong compared to our first model

## Summary
Machine learning model 2 would be the one to choose using the oversampled data. With the oversampled data, the logistic regression model accuracy moves closer to 1.00 with a balanced accuracy score of 0.99, compared to 0.95 from the previous model with original data. This seems to follow across the board with values nearing 1.00. Looking at the classification report as well, under the "Recall" column, both types of loan status had a rating of 1.00 and 0.99, which tells us that the model using the oversampled data had a strong algorithim in differentiating the two. In regards to which values are important to classify, the general answer should be both, we would like to see our model to closely and accurately predict both values, but I guess since the values for "1"(which are the risky loans) seem to have a difference in both models, making sure that value gets closer to one would currently be the priority as both models had similar ratings for the healthy loans. In addition, as background knowledge, there are more healthy loans than they are risky loans, hence classifying the risky loans would be important. 