# Gradient-Descent-for-Linear-Regression

**Student Name**: Ainavole Hasini Reddy
**Student ID**: 700773828



# Comparing Gradient Descent with Normal Equation for Linear Regression

This project demonstrates the comparison between **Gradient Descent** and the **Normal Equation** for solving linear regression. We generate a synthetic dataset and solve for parameters using both methods, then compare their performance and convergence.

---

## Step 1: Creating the Synthetic Dataset

- Generated **200 data points**
- True relationship: `y = 3 + 4*x + noise`
- `x` values range from 0.0 to 5.0
- `y` values range from 3.0 to 22.9
- Design matrix `X` shape: `(200, 2)` (200 rows, 2 columns)

---

## Step 2: Solving with Normal Equation (Closed-Form)

**Normal equation results:**

- Estimated intercept: **2.9226** (true value: 3)  
- Estimated slope: **4.0228** (true value: 4)

---

## Step 3: Solving with Gradient Descent

**Settings:**

- Initial guess: `θ₀ = 0.0`, `θ₁ = 0.0`
- Learning rate: `0.05`
- Max iterations: `1000`

**Iteration progress:**

| Iteration | Cost     | θ₀      | θ₁      |
|-----------|---------|---------|---------|
| 100       | 0.274665 | 2.4401  | 4.1713  |
| 200       | 0.220427 | 2.7714  | 4.0694  |
| 300       | 0.215096 | 2.8752  | 4.0374  |
| 400       | 0.214572 | 2.9077  | 4.0274  |
| 500       | 0.214520 | 2.9180  | 4.0242  |
| 600       | 0.214515 | 2.9212  | 4.0233  |
| 700       | 0.214515 | 2.9222  | 4.0229  |
| 800       | 0.214515 | 2.9225  | 4.0228  |
| 900       | 0.214515 | 2.9226  | 4.0228  |
| 1000      | 0.214515 | 2.9226  | 4.0228  |

**Final Gradient Descent Results:**

- Estimated intercept: **2.9226** (true value: 3)  
- Estimated slope: **4.0228** (true value: 4)

---

## Step 4: Comparing the Two Methods

| Parameter        | True Value | Normal Equation | Gradient Descent | Difference |
|-----------------|------------|----------------|-----------------|------------|
| θ₀ (intercept)   | 3.0000     | 2.9226         | 2.9226          | 0.000014   |
| θ₁ (slope)       | 4.0000     | 4.0228         | 4.0228          | 0.000004   |

> Gradient descent converged very close to the normal equation solution!  

---

## Step 5: Creating Visualizations

- Visualizations can include scatter plots of the data and regression lines for both methods.
- Cost function convergence plot for gradient descent.

  <img width="1389" height="590" alt="image" src="https://github.com/user-attachments/assets/57487a00-1097-4297-83d5-66485afc3d96" />

---

## Step 6: Final Analysis and Conclusions

**Performance Metrics:**

| Method              | R²       | MSE       |
|--------------------|-----------|-----------|
| Normal Equation    | 0.993740  | 0.214515  |
| Gradient Descent   | 0.993740  | 0.214515  |

**Summary:**

- Both methods successfully recovered parameters close to the true values.
- Normal equation provides the exact optimal solution instantly.
- Gradient descent reached nearly the same solution after 1000 iterations.
- Final gradient descent cost: 0.214515
- Both achieved high R² scores (> 0.99), indicating excellent fit.
- Tiny differences are due to the iterative nature of gradient descent.

**Conclusion:** Gradient descent converged to essentially the same solution as the normal equation.

---
