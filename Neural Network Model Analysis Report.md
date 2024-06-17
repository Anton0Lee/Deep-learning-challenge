# Neural Network Model Analysis Report

## Overview of the Analysis
The nonprofit foundation Alphabet Soup seeks a tool to identify funding applicants with the highest potential for success. Using machine learning and neural networks, along with features from a provided dataset, we plan to develop a binary classifier that predicts the post-funding success or failure of applicants.
<br/>

## Results

### Data Preprocessing:
The target variable for the model is "IS_SUCCESSFUL".

The features for the model are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT".

The variables removed from the input data are "EIN" and "NAME" because they are neither targets nor features.

<br/>

### Compiling, Training, and Evaluating the Model
1st Attempt:

The initial model comprises three layers with 80, 30, and 1 neuron(s), respectively. The first two layers use the "relu" activation function, while the output layer uses "sigmoid." Trained over 100 epochs, this model achieved an accuracy of 72.50%, falling short of the target predictive accuracy of over 75%.

![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%201%20(Codes).png)
![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%201%20(Neurons).png)
![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%201%20(Accuracy).png)

2nd Attempt:

Therefore, a second attempt was made by increasing the number of neurons. This revised model consists of three layers with 300, 300, and 1 neuron(s) respectively, maintaining the same activation functions and number of epochs as the original model. This adjustment resulted in an accuracy of 72.51%, still falling short of the target predictive accuracy of over 75%.

![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%202%20(Codes).png)
![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%202%20(Neurons).png)
![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%202%20(Accuracy).png)

3rd-10th Attempt:

Subsequent attempts involved altering the number of neurons, layers, epochs, and activation functions. Despite these adjustments, none of the models achieved the target predictive accuracy of over 75%. The resulting accuracies ranged from 72.36% to 72.71%.

The Highest Accuracy Attempt (10th Attempt):

The highest accuracy was achieved on the 10th attempt. This model consists of four layers with 20, 10, 10, and 1 neuron(s) respectively. The first three layers use the "relu" activation function, while the output layer uses "sigmoid." Trained over 100 epochs, this model achieved an accuracy of 72.71%, still below the target predictive accuracy of over 75%.

![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%2010%20(Codes).png)
![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%2010%20(Neurons).png)
![alt text](https://github.com/Anton0Lee/Deep-learning-challenge/blob/main/Images/Attempt%2010%20(Accuracy).png)


<br/>

## Summary
After ten attempts, the deep learning model did not reach the target predictive accuracy of over 75%. The accuracy of each model is included in the file names for easier comparison. Despite falling short of the target, the model achieved a close accuracy of 72.71% on the tenth attempt. This makes it a useful and reliable tool for Alphabet Soup to predict the success of applicants if funded.

To further improve the model's accuracy, an alternative method such as using the "KerasTuner" function can be considered. KerasTuner automates the process of finding the best hyperparameters by searching over a defined space of possible values, potentially leading to better model accuracy, faster convergence, and reduced overfitting.

