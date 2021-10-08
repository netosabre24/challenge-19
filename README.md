# Neural Network Charity Analysis

# Overview

The purpose of this analysis is to use Nueral Networks to try to predict if certain investment proposals are likely to be successful. This is accomplished using Tensor Flow's Keras to train and test existing data.

# Data Processing

* First the data is loaded, cleaned up and we determine the "IS_SUCCESSFUL" column is the target of the data. This columm gave the result of whether a proposal was successful. 
* Next the variables, "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS" and "ASK_AMT" are all considered features for this model.
* Two variables "EIN" and "NAME" were neither targets nor features, and were removed from the input data.

# Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

* Next we will scale the acquired data using the Standard scaler method to improve accuracy and consistency of the neural network. The results included the original model had a input layer with 80 nodes and 30 neurons, along with an activation function.

2. Were you able to achieve the target model performance?

* For target model performance, it failed to reach 75% as it stayed barely under 75%.

3.What steps did you take to try and increase model performance?

* To improvise, kerastuner was implemneted which allowed to automate the number of hidden layers and neurons under some conditions. Unfortunately, the accuracy still failed to meet 75% even with the kerastuner.

# Summary

Overall, we were not able to reach an accuracy of 75% which was the goal. More improvement for the model is needed if we want to increase the accuracy output to meet the assigned goal.
