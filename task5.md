# Linear Regression From Scratch – Project Report

## Objective
In this task, I implemented Linear Regression from scratch using Python and NumPy. The goal was to understand how gradient descent works and compare my custom implementation with the LinearRegression model from scikit-learn.

---

## Dataset
I used the California Housing dataset provided by scikit-learn.  
The dataset contains:

- 20,640 samples (houses)
- 8 input features
- Target variable: house price

Example features include median income, house age, average rooms, population, latitude, and longitude.

---

## Data Preparation
First, I split the dataset into training and testing sets.

- 80% training data
- 20% testing data

After that, I applied feature scaling using StandardScaler. This step is important because gradient descent works better when all features are in a similar range.

---

## Implementing Linear Regression From Scratch
I created my own Linear Regression class using NumPy.

The model uses the formula:

y = Xw + b

Where:
- **w** = weights
- **b** = bias
- **X** = input features

I used gradient descent to update the weights and bias. During each iteration the model:

1. Predicts house prices
2. Calculates the error
3. Computes gradients
4. Updates the weights and bias

This process repeats until the error is minimized.

---

## Model Evaluation
To evaluate the model, I used three common regression metrics:

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score

### Scratch Model Results
- MSE: 0.5546  
- MAE: 0.5352  
- R²: 0.5768  

### Scikit-learn Model Results
- MSE: 0.5559  
- MAE: 0.5332  
- R²: 0.5758  

---

## Graph Analysis
I plotted a scatter graph of actual house prices vs predicted prices.

Most points were around a diagonal trend line, which shows that the model predictions were reasonably close to the real values.

---

## Comparison
The performance of my scratch model was almost identical to the scikit-learn model. The small differences happen because my model uses gradient descent while scikit-learn uses a more optimized mathematical solution.

This shows that my manual implementation worked correctly.

---

## Conclusion
In this project, I implemented linear regression from scratch and trained it using gradient descent. I learned how weights are updated during training, why feature scaling is important, and how to evaluate regression models using standard metrics. Comparing my model with scikit-learn helped me understand how machine learning libraries simplify the process while still using the same core concepts.
