# Flam-R&D-Assignment

### Parametric Curve Fitting – Finding θ, M, and X
The goal is to find the unknown parameter values Theta(θ), M, and X using the given parametric equation and dataset provided for 6<t<60.

## Approach
1. Import the libraries
2. Load the dataset that is provided, containing the given curve points of x and y
3. Assume the parameter t is uniformly spaced in a range between 6 and 60
4. Define the parametric equations of x(t) and y(t)
5. Calculate the L1 distance of the actual and predicted values as the loss function
6. Take an initial guess of the parameters within their boundaries, which are provided
7. Optimize θ, M, and X using the method "L-BFGS-B"
8. Compute the MAE, RMSE, and L1 distance to measure accuracy
9. Visualize the fitted curve against the actual data points

## Mathematical Formulation
### Parametric equation of the curve:
$x = t\cos(\theta) - e^{M|t|}\sin(0.3t)\sin(\theta) + X$

$y = 42 + t\sin(\theta) + e^{M|t|}\sin(0.3t)\cos(\theta)$

## Final Outcomes
### Optimized Parameters
Theta (degrees): 28.1184
M: 0.021389
X: 54.9008
Optimization Success: True
Final L1 Distance: 37865.0939

### Error Metrics
MAE (x): 16.4221
MAE (y): 8.8213
Total MAE: 12.6217
RMSE (x): 20.0540
RMSE (y): 10.7559
Total RMSE: 15.4050

### Final Equation for Submission format
$$\left(t*\cos(0.4908)-e^{0.021389\left|t\right|}\cdot\sin(0.3t)\sin(0.4908)+54.9008,\ 
42+t*\sin(0.4908)+e^{0.021389\left|t\right|}\cdot\sin(0.3t)\cos(0.4908)\right)$$

### Fitted curve plot
![plotting](https://github.com/user-attachments/assets/ef539d21-6f94-4202-b9b3-c98fe9baa7e8)

### References
"https://www.desmos.com/calculator"
