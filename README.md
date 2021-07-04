# Neural_Network_Charity_Analysis

## Overview
This analysis was intended to create a neural network model that can predict whether applicants might be successful if they're funded by Alphabet Soup. To mae these predictions, we are using a dataset with over 34,000 organizations that have received funding from Alphabet Soup in the past. 

## Results
- Data Preprocessing
  - The target variable for this analysis is the "IS_SUCCESSFUL" columns which produces a dichotomous result of whether or not an application was successful
  - The features for this model include Application Type, Affiliation, Classification, USe Case, Organization, Status, Income Amount, Special Considerations, and Ask Amount.
  - The "EIN" and "NAME" columns are not features of this model and can be dropped from the dataframe.

- Compiling, Training, and Evaluating the Model
  - For the application, I ended up using three hidden layers to attempt to achieve 75% accuracy. For each hidden layer, I used 30, 15, and 10 neurons respectively with ReLu, Tanh, and Sigmoid activation functions. I was unable to achieve 75%, so I kept experimenting with different activation functions and additional hidden layers/neurons to try to achieve better results. 
  - This model was unfortunately unable to achieve target model performance.
  - As mentioned, I tried to increase the number of hidden layers and neurons to optimize performance, which did improve slightly. I also removed the "STATUS" column of our dataframe to reduce the number of variables involved in predicting application success.

## Summary
This model was able to achieve an accuracy of about 72.9%, with a loss metric of about 0.55. Another machine learning model that can be used to analyze this data is logistic regression. This model would work because it is a supervised learning algorithm that is used to predict the probability of a dichotomous outcome. In this case, it would classify predictions into whether or not an Alphabet Soup application might be successful based on the features mentioned in the Results section. 
