# Neural_Network_Charity_Analysis

## Overview of the Analysis:
 The purpose of the analysis is to help the Alphabet Soup Charity predict where to make investments. We will use the dataset 'charity_data.csv' to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The dataset contains more than 34,000 organizations that have received funding from Alphabet Soup. The dataset contains a number of columns that capture metadata about each organization such as:
- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

In this analysis we will accomplish the following:
- Deliverable 1: Preprocessing Data for a Neural Network Model
- Deliverable 2: Compile, Train, and Evaluate the Model
- Deliverable 3: Optimize the Model
- Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Results
#### Data Preprocessing:
1) What variable(s) are considered the target(s) for your model?
  - The variable that is considered the target for my model is the 'Is-Successful' column, this tells us if the organization did well and is the money donated was used and thus made the organization successful.
  
2) What variable(s) are considered to be the features for your model?
  - The features of my model are: NAME, APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, STATUS, AND ASK_AMT.
  
3) What variable(s) are neither targets nor features, and should be removed from the input data?
  - The EIN (Employer Id) and Name were dropped because it is not significant and does not add any value or information that we need to decide on if an organization should be funded or not. I didn't remove these columns but they don't add any important information or value for what we are trying to accomplish; Special_considerations and Status. 
  
#### Compiling, Training, and Evaluating the Model
1) How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - Intially, I decided to use two hidden layers, the first layer with 80 neurons and relu activation, the second layer with 30 neurons and relu activation, and the output layer with sigmoids activation. This had an accuracy of 72.7%. When trying to optimize the model I made the following changes to get the accuracy over 75%: three hidden layers and and output layer. First layer was 100 neurons and relu activation, the second layer was 30 and sigmoid activation, the third 10 and sigmoid activation, and the output layer with sigmoid activation. Adding the third hidden layer and changing the second and third activation functions to sigmoid seemed to get the accuracy level above 75% to 78.9%.

2)Were you able to achieve the target model performance? 
  - Yes, see above. 

3) What steps did you take to try and increase model performance? 
  - Changing the Name column to a value had a big impact on helping to improve the accuracy of the dataset and adding a third hidden layer along with changing the second and third layers to sigmoid activation. 

## Summary: 
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
Below you will see images I included that shows what I explained above to get an accuracy of 78.9%  along with changing the Name column. 

<img width="600" alt="image3" src="https://user-images.githubusercontent.com/100392991/179435214-c921cf40-3b34-40e7-b8e8-cf37bab006b0.PNG">


<img width="500" alt="image4" src="https://user-images.githubusercontent.com/100392991/179435223-3cb37c60-4fa2-4198-9e5b-cff2ed41dc7a.PNG">



