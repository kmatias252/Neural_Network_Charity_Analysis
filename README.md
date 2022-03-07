# Neural_Network_Charity_Analysis

## Overview of Neural Network Charity Analysis: 

The purpose of this analysis is to create a neural networks model which will use the features in the provided dataset to help our client create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The dataset includes more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Deliverables: 

* Deliverable 1: Preprocessing Data for a Neural Network Model
* Deliverable 2: Compile, Train, and Evaluate the Model
* Deliverable 3: Optimize the Model

## Results: 

### Data Preprocessing

* What variable(s) are considered the target(s) for your model?

    * IS_SUCCESSFUL — Was the target variable for our model ( if the money used effectively)

![Screen Shot 2022-03-06 at 8 59 31 PM](https://user-images.githubusercontent.com/91925639/156955136-b6796932-ed31-4197-acfb-6bac3c7c6aac.png)


* What variable(s) are considered to be the features for your model?

    * APPLICATION_TYPE
    * AFFILIATION
    * CLASSIFICATION
    * USE_CASE
    * ORGANIZATION
    * STATUS
    * INCOME_AMT
    * SPECIAL_CONSIDERATIONS
    * ASK_AMT

![Screen Shot 2022-03-06 at 8 58 51 PM](https://user-images.githubusercontent.com/91925639/156955048-8b488b58-dd76-42af-9f67-ebdde2fc615f.png)

    
* What variable(s) are neither targets nor features, and should be removed from the input data?

    * EIN
    * NAME

![Screen Shot 2022-03-06 at 8 57 49 PM](https://user-images.githubusercontent.com/91925639/156954953-587845b2-709b-4caa-9018-3e15753a5e24.png)


### Data Preprocessing

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

In our model we had an input layer, hidden layer 1 had 80 neurons, hidden layer 2 had 30 meurons and we had an output layer. In terms of activation function our model used relu and sigmoid functions given that we were trying to develop a binary classification model to calculate the model’s loss and accuracy.

![Screen Shot 2022-03-06 at 9 10 43 PM](https://user-images.githubusercontent.com/91925639/156956003-78515b89-32bb-4026-b0f8-87c4b2414420.png)

* Were you able to achieve the target model performance?

Our model was only able to achieve 73% accuracy vs our target of 75%. 

![Screen Shot 2022-03-06 at 9 11 21 PM](https://user-images.githubusercontent.com/91925639/156956047-e64d3485-c658-405b-8758-af52c6bda52f.png)

* What steps did you take to try and increase model performance?

  * Optimization attempt 1: Increased the number of hidden nodes for each layer
  * 
    ![Screen Shot 2022-03-06 at 9 18 17 PM](https://user-images.githubusercontent.com/91925639/156956630-f011e94b-7073-4b16-a927-d8e9b2e14f8d.png)
    
  * Optimization attempt 2: Increase the number of layers
  
   ![Screen Shot 2022-03-06 at 9 14 06 PM](https://user-images.githubusercontent.com/91925639/156956278-d2aa8431-19f4-40a9-a0c0-0bf9cb9a1fe9.png)

  * Optimization attempt 3: Increase the number of epochs
  
   ![Screen Shot 2022-03-06 at 9 15 15 PM](https://user-images.githubusercontent.com/91925639/156956370-14996e14-9947-4858-9a79-c3ffd9d51919.png)

## Summary: 

Based on our analysis we can conclude that our neural networks model was not able to achieve our accuracy target of 75% (our results yielded in a 73% accuracy score), therefore I would not recommend this model to predict whether applicants will be successful if funded by Alphabet Soup. 
I would recommend using a different model possibly a supervised machine learning model such as Random Forest Classifier which could help solve the classification problem we experienced.
