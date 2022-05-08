# Neural_Network_Charity_Analysis

## Overview

Help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. To do this I will:

* Preprocess data for a neural network model
* Compile, train, and evaluate the model 
* Optimize the model
* Write a written report on the neural network model

## Results

#### Data preprocessing

* The variable considered the target for my model is the column: IS_SUCCESSFUL
* The variables considered to be the features are all the columns execpt for IS_SUCCESSFUL and the ones that will be dropped
* The variables that are considered neither targets nor features and should be removed are: EIN and NAME

#### Compiling, training, and evaluating the model

* For my neural network model i had 2 hidden layers, the first layer having 80 neurons and the second having 30. The activation function used was "relu" for the hidden layers. Sigmoid was used for the output layer.
* The target model was not able to achieve the target performance. The target performance was 75% and the target model was less then that.
* To try and increase the model performance I applied bucketing to the feature "ASK_AMT" and organized the different values by intervals. I increased the number of neurons on one of the hidden layers, then used a model with three hidden layers. Also I tried a different activation function, being "tanh" but none of those steps helped improve the model's performance.

## Summary

The deep learning neural network model did not reach the target of 75% accuracy. Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.

