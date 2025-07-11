# Linear Regression Implementation

A gradient descent-based linear regression model.

## How It Works
- Learns weights to predict targets using a linear combination of features
- Optimizes weights using gradient descent to minimize prediction error
- Supports customizable learning rate and training iterations
## Setup
- First clone the repo by using the command below </br>
```!git clone https://github.com/ThomasKarabo/linear-regression-from-scratch.git```
- Append the directory of the algorithm by running the code</br>
```python
import sys
sys.path.append('/content/linear-regression-from-scratch/models')
```
## Usage
```python
from linear_regression import LinearRegression

# Initialize and train
model = LinearRegression(learning_rate=0.01, n_iterations=1000)
model.fit(X_train, y_train)

# Predict
predictions = model.predict(X_test)

# Inspect learned weights
print("Weights:", model.weights)
print("Bias:", model.bias)

Key Methods
fit(X, y): Trains the model on feature matrix X and target y

predict(X): Returns predictions for new data

feature_importance(): Returns weights sorted by absolute value
```
