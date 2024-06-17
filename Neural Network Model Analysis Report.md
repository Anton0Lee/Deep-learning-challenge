# Neural Network Model Analysis Report

## Overview of the Analysis
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. By utilizing machine learning and neural networks along with features from a given dataset, we aim to construct a binary classifier that predicts the success or failure of applicants post-funding.  

<br/>

## Results

### Data Preprocessing:
The target variable for the model is "IS_SUCCESSFUL".

The features for the model are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT".

The variables removed from the input data are "EIN" and "NAME" because they are neither targets nor features.

<br/>

### Compiling, Training, and Evaluating the Model
1st Attempt:

Initially, the model consists of three layers with 80, 30, and 1 neurons respectively. The activation function for the first two layers is "relu", while the activation function for the output layer is "sigmoid". The number of epochs is 100. This model produced an accuracy of 72.50%, which did not achieve a target predictive accuracy higher than 75%.  

![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%201%20(Codes).png)
![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%201%20(Neurons).png)
![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%201%20(Accuracy).png)

2nd Attempt:

Therefore, 2nd attempt was done by increasing the number of neurons. This model consists of three layers with 300, 300, and 1 neurons respectively. The activation functions and number of epochs remain the same as the original model. This model produced an accuracy of 72.51%, which did not achieve a target predictive accuracy higher than 75%.

![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%202%20(Codes).png)
![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%202%20(Neurons).png)
![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%202%20(Accuracy).png)

3rd-10th Attempt:

After that, more attempts were done by changing the number of neurons, layers, epochs, activation functions. All of the attempts were not able to achieve a target predictive accuracy higher than 75%. The predictive accuracy produced are ranging from 72.36% to 72.71%. 


The Highest Accuracy Attempt (10th Attempt):

The highest accuracy attempt is the 10th attempt. This model consists of four layers with 20, 10, 10 and 1 neurons respectively. The activation function for the first three layers is "relu", while the activation function for the output layer is "sigmoid". The number of epochs is 100. This model produced an accuracy of 72.71%, which did not achieve a target predictive accuracy higher than 75%.    

![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%2010%20(Codes).png)
![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%2010%20(Neurons).png)
![alt text](https://github.com/Roy-Ip/deep-learning-challenge/blob/main/Images/Attempt%2010%20(Accuracy).png)


<br/>

## Summary
After 10 times of attempts, the deep learning model was not able to achieve a target predictive accuracy higher than 75%. The accuracy of each model is included in the name of the file for easier comparison. Although it was not able to achieve 75% accuracy, it produced a very close accuracy percentage (ie. 72.71%) after 10 attempts. It is still a useful and realiable model for Alphabet Soup to predict whether applicants will be successful if funded by Alphabet Soup. 

To further improve the accuracy of the model, an alternative method, such as using "KerasTuner" function, can be used. It may be a better way to achieve a higher percentage as KerasTuner automates the process of finding the best hyperparameters by performing a search over a defined space of possible values. It helps in achieving better model accuracy, faster convergence, and reduced overfitting.

