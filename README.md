# Neural_Networks_Deep_Learning

## Overview: 
* Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

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

### Purpose:
* Preprocessing Data for a Neural Network Model
* Compile, Train, and Evaluate the Model
* Optimize the Model
  * Using TensorFlow, optimize the model in order to achieve a target predictive accuracy higher than 75%. Make at least three attempts to do so.

### Results:
* Data Preprocessing
  * What variable(s) are considered the target(s) for your model?
    * IS_SUCCESSFUL is our target variable
  * What variable(s) are considered to be the features for your model?
    * ["APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS"] is the features for our model
  * What variable(s) are neither targets nor features, and should be removed from the input data?
    * EIN and NAME were neither targets nor features, therefore we removed from the dataset
   
* Compiling, Training, and Evaluating the Model
  * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    * We used two hidden layers for this model, with 80 neurons on the first layer and 30 neurons on the second layers, and the activation for the first layers and second layers are "relu" and activation for output layer is "sigmoid".
  * Were you able to achieve the target model performance?
    * I was not able to reach a taget performance of 75%, based on my three attend the avarage performance is close to 72.9%
  * What steps did you take to try and increase model performance?
    * On the first attend, I added an additional layer to the model and achieved a 73%. On the second attend, I changed the output activiation to "tanh" which also achieve a 72.9%. On the third attend, I added the fourth layer, changed the third and forth activation to "sigmoid", and run it with epochs of 150 times, and it lowered rate to 72.8%.
    
## Summary:
* As of result, the target accruacy rate of 75% was not suucessful, as we only achieved 73% for our best model. Recommandation to achieve 75% accuracy rate, we can try Random Forest Classifier or SVM model. 
