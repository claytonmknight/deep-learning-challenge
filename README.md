# deep-learning-challenge
 deep-learning-challenge
# Alphabet Soup Charity Funding Predictor

## Overview of the Analysis

The objective of this analysis is to develop a deep learning model using neural networks to predict the success of funding applications submitted to Alphabet Soup, a fictitious charity organization. The model aims to accurately classify whether an application will be successful or not based on various input features.

## Results

### Data Preprocessing

- **Target Variable(s):**
  - The target variable for the model is "IS_SUCCESSFUL," which indicates whether the funding application was successful (1) or not (0).

- **Feature Variable(s):**
  - The feature variables include all columns except "IS_SUCCESSFUL" since they provide information to predict the target variable.

- **Variable(s) to Remove:**
  - The columns "EIN" and "NAME" were removed as they are neither targets nor features and do not contribute to the model's predictive ability.

### Compiling, Training, and Evaluating the Model

- **Neurons, Layers, and Activation Functions:**
  - The model consists of two hidden layers with 6 neurons each. The first hidden layer uses the ReLU activation function, while the second hidden layer utilizes the hyperbolic tangent (tanh) activation function. The output layer contains 1 neuron with a sigmoid activation function, suitable for binary classification tasks.

- **Target Model Performance:**
  - The target model performance was set to achieve an accuracy of 75%.

- **Steps to Increase Model Performance:**
  - Experimented with different combinations of neurons, layers, and activation functions to optimize model performance.
  - Explored various data preprocessing techniques such as feature scaling and one-hot encoding to improve model training.
  - Adjusted hyperparameters, including optimizers and learning rates, to enhance convergence and reduce loss during training.

### Original Model Performance

The original model was defined with two hidden layers containing 80 and 30 neurons, respectively, with ReLU activation functions. The output layer consisted of 1 neuron with a sigmoid activation function. The model achieved an accuracy of approximately 72.84%.

### Attempt 1

- **Model Configuration:** Two hidden layers with 6 neurons each, both using ReLU activation functions.
- **Result:** Accuracy improved slightly to approximately 72.87%.

### Attempt 2

- **Model Configuration:** Two hidden layers with 6 neurons each, with ReLU activation function for the first hidden layer and hyperbolic tangent (tanh) activation function for the second hidden layer.
- **Result:** The accuracy increased to around 73.29%.

### Attempt 3

- **Model Configuration:** Similar to Attempt 2, with two hidden layers containing 6 neurons each, ReLU activation function for the first hidden layer, and tanh activation function for the second hidden layer. However, the number of epochs was increased to 200.
- **Result:** The accuracy slightly decreased compared to Attempt 2, achieving approximately 73.00%.

## Summary

The deep learning model achieved a moderate accuracy of approximately 73.29% in predicting the success of funding applications for Alphabet Soup. While the model performance fell slightly below the target of 75%, it demonstrated reasonable predictive capability.

While Attempt 3 showed a slight decrease in accuracy compared to Attempt 2, all attempts demonstrated improvements over the original model. Although the target accuracy of 75% was not achieved, the experiments helped identify configurations that led to better performance.

To improve the classification problem and achieve the desired 75% accuracy, further experimentation with the model architecture, hyperparameters, and data preprocessing techniques may be necessary. Additionally, exploring more advanced neural network architectures or ensemble methods, such as bagging or boosting, could help capture complex patterns in the data and enhance predictive performance.