# Neural Network Charity Analysis

## Overview

This analysis uses neural networks to attempt to predict whether organizations that applied for funding from Alphabet Soup will get the grants. 

## Results

### Data Processing

  - What variable(s) are considered the target(s) for your model?
    - The target variable of this analysis is "IS_SUCCESSFUL", as we are predicting whether the organizations are successful in applying for funding. 
  
  - What variable(s) are considered to be the features for your model?
    - The feature variable of this analysis are the rest of the data excluding "IS_SUCCESSFUL". 
  
  - What variable(s) are neither targets nor features, and should be removed from the input data?
    - Other variables that are neither targets or features are "EIN" and "NAME".

### Compiling, Training, and Evaluating the Model

  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - There were 80 neurons in the first hidden layer and 30 neurons in the second hidden layer. The activation function chosen was "relu" as it is the most common activation function and the dataset did not have any negative values in it. 
  
  - Were you able to achieve the target model performance?
    - The original accuracy score is 72.68%, just shy of the targeted score of 75%.
  
  - What steps did you take to try and increase model performance?
    - In attempt to optimize the model, I tried to add in third / fourth hidden layer and also replaced any counts in "INCOME_AMT" that is less than 955 and classified them as "other". 
![inc](https://github.com/donovancai/Neural_Network_Charity_Analysis/blob/main/income_amt.jpg)

## Summary

In an attempt to optimize the results, despite adjusting the number of hidden layers and classifying "INCOME_AMT", the accuracy score remained 72.68%. 

Other ways to improve the accuracy socre could be to try other activation methods such as tanh, linear and leak Relu. 
