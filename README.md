# Neural Network Charity Analysis

## Overview of the Analysis
    
    The purpose of this analysis is to build a deep neural network model using TensorFlow's Keras API to predict whether applicants to a charity organization will be successful if funded. The dataset contains information on various features such as EIN, organization name, application type, affiliation, classification, use case, organization type, status, income amount, special considerations, ask amount, and success status (1 for successful, 0 for unsuccessful).

 * Data Exploration
    * Application Type (APPLICATION_TYPE): The dataset has 17 unique application types. The most common application types are T3, T4, T6, T5, and T19.

    * Classification (CLASSIFICATION): There are 71 unique classification types. The top classifications are C1000, C2000, C1200, C3000, and C2100.

 * Model Architecture
    The deep neural network model is constructed with the following architecture:

    * Input Layer: The input layer has a number of nodes equal to the number of features in the dataset.

    * Hidden Layers: The model has two hidden layers with 80 and 30 nodes, respectively. The activation function used is 'relu' for both hidden layers.

    * Output Layer: The output layer has 1 node with a 'sigmoid' activation function, suitable for binary classification problems.

 * Model Training
    The model is trained for 100 epochs using the Adam optimizer and sparse categorical cross-entropy loss function. The training process shows a gradual improvement in both loss and accuracy across epochs.

## Results
 * Model Accuracy: The final accuracy on the training dataset is approximately 74.15%, and on the testing dataset, it is around 72.66%.

 * Loss: The loss on the testing dataset is 0.5539.

 * Unique Values Count After Processing:

    * Application Type: 17
    * Affiliation: 6
    * Classification: 71
    * Use Case: 5
    * Organization Type: 4
    * Status: 2
    * Income Amount: 9
    * Special Considerations: 2
    * Ask Amount: 8747
    * Is Successful: 2

## Summary
    The neural network model shows moderate accuracy on the given dataset. Further optimization and tuning may be required to enhance model performance. Consideration should be given to feature engineering, hyperparameter tuning, and alternative model architectures.