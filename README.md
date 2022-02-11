# Neural Network Charity Analysis

## Overview
Alphabet Soup’s business team has a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Into this dataset are several columns that capture metadata about each organization. With our knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to create a binary classifier capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
**Data Preprocessing**
1. The variable IS_SUCCESSFUL is a data type bool that entails whether or not the charity donation is effective. Therefore this variable is considered as the target for our analysis
2. The variables considered to be features on the model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT
3. The EIN and NAME variables were removed because these are identifications of foundations and don't represent any value to the model

**Compiling, Training, and Evaluating the Model**
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - Were you able to achieve the target model performance?
  - What steps did you take to try and increase model performance?
