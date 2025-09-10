# Gradient-Descent-for-Linear-Regression

**Student Name**: Ainavole Hasini Reddy
**Student ID**: 700773828



Comparing Gradient Descent with Normal Equation for Linear Regression
======================================================================

Step 1: Creating our synthetic dataset
----------------------------------------
Generated 200 data points
True relationship: y = 3 + 4*x + noise
x values range from 0.0 to 5.0
y values range from 3.0 to 22.9
Design matrix X has shape: (200, 2) (200 rows, 2 columns)

Step 2: Solving with Normal Equation (Closed-Form)
--------------------------------------------------
Normal equation results:
  Estimated intercept: 2.9226 (true value: 3)
  Estimated slope:     4.0228 (true value: 4)

Step 3: Solving with Gradient Descent
------------------------------------------
Starting gradient descent with:
  Initial guess: θ₀ = 0.0, θ₁ = 0.0
  Learning rate: 0.05
  Max iterations: 1000

Iteration progress:
  Iteration  100: Cost = 0.274665, θ₀ = 2.4401, θ₁ = 4.1713
  Iteration  200: Cost = 0.220427, θ₀ = 2.7714, θ₁ = 4.0694
  Iteration  300: Cost = 0.215096, θ₀ = 2.8752, θ₁ = 4.0374
  Iteration  400: Cost = 0.214572, θ₀ = 2.9077, θ₁ = 4.0274
  Iteration  500: Cost = 0.214520, θ₀ = 2.9180, θ₁ = 4.0242
  Iteration  600: Cost = 0.214515, θ₀ = 2.9212, θ₁ = 4.0233
  Iteration  700: Cost = 0.214515, θ₀ = 2.9222, θ₁ = 4.0229
  Iteration  800: Cost = 0.214515, θ₀ = 2.9225, θ₁ = 4.0228
  Iteration  900: Cost = 0.214515, θ₀ = 2.9226, θ₁ = 4.0228
  Iteration 1000: Cost = 0.214515, θ₀ = 2.9226, θ₁ = 4.0228

Gradient descent final results:
  Estimated intercept: 2.9226 (true value: 3)
  Estimated slope:     4.0228 (true value: 4)

Step 4: Comparing the two methods
-------------------------------------
Summary of all results:
  True parameters:      θ₀ = 3.0000, θ₁ = 4.0000
  Normal equation:      θ₀ = 2.9226, θ₁ = 4.0228
  Gradient descent:     θ₀ = 2.9226, θ₁ = 4.0228
  Intercept difference: 0.000014
  Slope difference:     0.000004
 Gradient descent converged very close to the normal equation solution!

Step 5: Creating visualizations
-----------------------------------
<img width="1389" height="590" alt="image" src="https://github.com/user-attachments/assets/fb8a23b9-7285-413d-a23d-e1dd4ba917ce" />



Step 6: Final analysis and conclusions
----------------------------------------
Performance metrics:
  Normal equation    - R²: 0.993740, MSE: 0.214515
  Gradient descent   - R²: 0.993740, MSE: 0.214515

Final Summary:
• Both methods successfully recovered parameters close to the true values
• Normal equation gave us the exact optimal solution instantly
• Gradient descent took 1000 iterations but reached nearly the same answer
• Final cost after gradient descent: 0.214515
• Both methods achieved very high R² scores (> 0.99), showing excellent fit
YES - Gradient descent converged to essentially the same solution as the normal equation.
The tiny differences are due to the iterative nature of gradient descent.
