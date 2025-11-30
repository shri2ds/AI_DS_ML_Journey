# AI_DS_ML_Journey

Welcome to my personal journey transitioning from a **Software Engineer** to an aspiring **AI/ML/Data Scientist**. This repo will be continuously updated with my progress, code, notes, and projects.


---

## 📁 Repository Structure
```
📦AI-ML-Journey
├── LeetCode/              # Python solutions to coding problems
├── SQL/                   # SQL queries and exercises
├── ML_Algorithm/           # Implementing ML Algorithm with mathematical foundations
├── KaggleNotebooks/       # Notebooks explored from Kaggle
├── Projects/              # Weekly structured projects
├── Quizzes/               # Periodic self-assessment quizzes
└── README.md              # This file
```

---
## Linear Regression
### Model Performance: Convergence Check
We used Gradient Descent to optimize the parameters. The graph below shows the cost function ($J(\theta)$) decreasing over iterations, confirming that the learning rate was tuned correctly.

![Gradient Descent Loss Curve](./ML_Algorithm/loss_curve.png)

*Observation: The loss drops exponentially and stabilizes around iteration 200, indicating convergence.*

## Logistic Regression
### Mathematical Foundation: Binary Cross Entropy (Log Loss)
For binary classification, we model the target $y$ as a Bernoulli distribution. Instead of Mean Squared Error (MSE), which results in a non-convex loss surface for sigmoid activation, we use **Log Loss**.

**The Cost Function:**
$$J(\theta) = - \frac{1}{m} \sum_{i=1}^{m} [y^{(i)} \log(\hat{y}^{(i)}) + (1-y^{(i)}) \log(1 - \hat{y}^{(i)})]$$

**Why this works:**
1.  **Convexity:** It guarantees a global minimum, allowing Gradient Descent to converge.
2.  **Maximum Likelihood:** Minimizing this loss is mathematically equivalent to maximizing the likelihood of the observed data.
3.  **Penalty:** It heavily penalizes "confident but wrong" predictions (e.g., predicting 0.99 probability for a negative class).

## 🧵 Contact
For discussions, improvements or collaborations, reach me via [LinkedIn](https://www.linkedin.com/in/shridhar-bhandar/).
