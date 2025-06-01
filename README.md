# bias-variance-decomposition
Bias–Variance trade-off project using polynomial regression. Explains theory and code.

# Bias–Variance Decomposition Project 

This project demonstrates the **bias–variance trade-off** in machine learning using **polynomial regression** and synthetic data.

We generate multiple noisy datasets, fit models of varying complexity, and visualize:

- Bias²
- Variance
- Total error
- Decomposition formula:  
  Expected Error = Bias² + Variance + Irreducible Noise

---

## How It Works

- Simulate noisy data from y = sin(x)
- Train 100 models with different random samples
- Compute and visualize:
  - Average prediction
  - Prediction variance
  - Bias² vs. true function

---

## Key Concepts Covered

- Mean Squared Error (MSE)
- Bias²: Systematic underfitting error
- Variance: Model sensitivity to data
- Irreducible noise: Data uncertainty
- Regularization intuition (lambda in Ridge)

---

## Skills Demonstrated

- Data simulation
- Bias–variance decomposition
- Model diagnostics
- Matplotlib visualizations
- Pipeline modeling with scikit-learn


**Interpretation:**

- The model has **low bias**, meaning it learns the true function's overall pattern well.
- The **moderate variance** suggests that predictions shift slightly depending on the training dataset — which is expected in ensemble models like Random Forests.
- The **total mean squared error (MSE)** is low, indicating a strong overall fit.
- Since most of the error is shared between small bias and manageable variance, the model is well-balanced for generalization.

This validates the earlier bias–variance theory and shows how `mlxtend` can streamline evaluation in real projects.
