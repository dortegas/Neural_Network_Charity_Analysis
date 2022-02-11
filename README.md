# Neural Network Charity Analysis

## Overview
Alphabet Soup’s business team has a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Into this dataset are several columns that capture metadata about each organization. With our knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to create a binary classifier capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
**Data Preprocessing**

1. The variable IS_SUCCESSFUL is a data type bool that entails whether or not the charity donation is effective. Therefore this variable is considered as the target for our neural network model
2. The variables considered to be features on the model are:
   - **APPLICATION_TYPE**. Alphabet Soup application type
   - **AFFILIATION**. Affiliated sector of industry
   - **CLASSIFICATION**. Government organization classification
   - **USE_CASE**. Use case for funding
   - **ORGANIZATION**. Organization type
   - **STATUS**. Active status
   - **INCOME_AMT**. Income classification
   - **SPECIAL_CONSIDERATIONS**. Special consideration for application
   - **ASK_AMT**. Funding amount requested
4. The EIN and NAME variables were removed because these are identifications of foundations and don't represent any value to the model

**Compiling, Training, and Evaluating the Model**

According to the best practices and experts recommendations to avoid building a neural network model overfitted, we started considering the following settings:
- 1 Input layer with 44 variables
- 2 Hidden layers:
   - First layer with 80 neurons and Relu as activation function
   - Second layer with 30 neurons and Relu as activation function
- The Output layer with the Sigmoid activation function

The 80 neurons in the first hidden layer are in a 1:2 ratio of our input variables (44). Because we are creating a binary classifier capable of predicting whether applicants will be successful if funded by "Alphabet Soup," we chose the ReLU function in the hidden layers as the ideal for looking at positive nonlinear input data for classification and its less complexity.

The accuracy of this model was 0.7251. For this reason, we tried to optimize the model to achieve a target predictive accuracy higher than 75% by making the following modifications in three attempts.

**Attempt 1**
Dropping the column SPECIAL_CONSIDERATIONS and creating an additional APPLICATION_TYPE bin. The neural network model was built as follows:
- 1 Input layer with 43 variables
- 2 Hidden layers:
   - First layer with 80 neurons and Relu as activation function
   - Second layer with 30 neurons and Relu as activation function
- The Output layer with the Sigmoid activation function

Accuracy outcome: 0.7262, not a considerable optimization.



