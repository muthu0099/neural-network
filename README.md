# OVER VIEW
This file defines the neural network architecture used for predicting car prices based on multiple numerical and encoded categorical features.
The model is implemented using PyTorch (torch.nn.Module) and is designed for regression tasks.

The model learns a mapping from input features (such as year, horsepower, and encoded attributes) to a continuous output representing the car price.

# MODEL ARCHITECTURE 

Input Feature 

year
car Model 
car color 
car turbo 
car fueltype 
horsepower 


netork scheme 

Input (6)
 → Linear(6 → 64)
 → ReLU
 → Linear(64 → 128)
 → ReLU
 → Linear(128 → 64)
 → ReLU
 → Linear(64 → 1)ReLU activation is used to introduce non-linearity and avoid vanishing gradients.

Multiple hidden layers allow the model to learn complex feature interactions.

Single output neuron is used because this is a regression problem.

No activation function is applied in the final layer to allow unrestricted numeric output.

# EVALUATION METRICS 
 
the Model evaluated based RMSE and R2 value 

RMSE : 0.4752 %
R2 : 0.7745 
