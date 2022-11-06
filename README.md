# Neural Network Charity Analysis

# Overview

Fort this project we used deep-learning neural networks to create a binary classifer that is capable of predicting whether applicants will be successful if funded by a non-profit financing agency. The dataset contained more than 34,000 organizations that have received funding over the years and included a number of useful fields in whcih to build our model on, including:

- Application type 
- Affiliated sector of industry
— Government organization classification
- Use case for funding
— Organization type
- Active status
- Income classification
- Special consideration for application
- Funding amount requested
- If the money used effectively or not

Our model was developed by preprocessing the data, followed by model compiling, training, evaluation and optimization.

# Results

## Data Preprocessing

- Our model's target variable was whether or not the money was used effectively. 
- The remaining variables listed above all served as features for the model. 
- Two fields that held unique identifiers were removed ('Name' and 'EIN').

## Compiling, Training, and Evaluating the Model

- Our deep-learning neural network model is made of two hidden layers with 80 and 30 neurons and input data has a total of 5,981 parameters.
- We used ReLU as the activation function, with Sigmoid on the output layer. Additionally, the optimizer was adam and the loss function is binary_crossentropy.

With the above parameters, our model reached 73% accuracy, well below the target threshold of 75%. In an attempt to improve performance, we made three changes to the model:
- Increased the number of neurons in our layers to 100 and 50, respectively, resulting in a slightly better performance (73.1%). 
- Added a third layer (with 25 neurons), resulting in an outcome of 72.6% accuracy.
- Changed the activation function from ReLU to tanh, resulting in an accuracy score of 72.9%.

# Summary

Because we were unable to meet an acceptable level of performance with out neural network, it may be appropriate to consider a different classification model. A good option in this case may be a balanced random forest classifier for the following reasons:

- They are robust against overfitting and outliers
- They rank importance of input variables, allowing us to see which are the most important
- They can handle thousands of input variables (even though we have less than ten)
- They run efficiently on large datasets, which we have here
- They have high accuracy and interpretability




