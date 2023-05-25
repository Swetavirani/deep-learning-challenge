# deep-learning-challenge

Overview
This analysis will cover the details of the neural network model and the adjustments made to the model in order to increase performance.

Results

Data Preprocessing
The target variable in this model is the "IS_SUCCESSFUL" column.

The feature variables in the final model were:
NAME
APPLICATION_TYPE
AFFILIATION
CLASSIFICATION
USE_CASE
ORGANIZATION
INCOME_AMT
ASK_AMT

The variables that were removed from the final model were:
EIN 
STATUS
SPECIAL_CONSIDERATIONS 

Compiling, Training, and Evaluating the Model
The final model has two layers :
First layer - 100 neurons/nodes with activation function relu
Second layer - 50 neurons/nodes with activation function sigmoid
Third layer - 50 neurons/nodes with activation function sigmoid


The model reached 78.64% accuracy - see the image below.

Model evaluation

Following steps to increase the model's performance:
- Included third layer to increase the model's complexity.
- 2 layers has activation function of relu and 1 layer has activation layer of sigmoid 
- Removed two columns of SPECIAL_CONSIDERATIONS, STATUS which didn't have more than 2 unique values
- Included NAME column  


Summary
The optimized neural network was able to predict outcomes with 78.64% accuracy. The increase in the performance was mainly due to adding NAME COLUMN and removal of SPECIAL_CONSIDERATIONS, STATUS which provided more variables to the data. Also adding one additional hidden layer helped with increase in performance. 

As an alternative to the neural network model, a random forest classifier could be used and was able to get 77.10% accuracy which is better than then threshold of 75% desired level but lower than neural network model with 78.64% accuracy. 