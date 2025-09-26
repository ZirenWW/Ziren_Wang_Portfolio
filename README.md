# Ziren Wang's Portfolio

Welcome to my portfolio!  
Here you will find some of my projects and skills showcased as part of my work in **Machine Learning, Data Analysis, and Finance**.

---

## 🧑‍🎓 About Me
I am currently pursuing a **Master of Engineering in Mechanical and Industrial Engineering** at the **University of Toronto**.  
I specialize in **Machine Learning**, **Data Analytics**, and **Financial Modeling**, with a strong foundation in **mathematics and statistics**.

---

## 💼 Projects

### 1. Electrical Grid Stability Prediction  
- **Goal:**  
  Developed a mathematical model to predict **electrical grid stability** using **Linear Regression** and **Gradient Descent** techniques.  
  The project analyzes the **Electrical Grid Stability dataset** (10,000 instances, 12 features) and evaluates the impact of **batch size** and **learning rate** on convergence.

- **Technologies:**  
  Python, NumPy, SciPy, Scikit-learn, Matplotlib

- **Process:**  
  - **Data Preparation:** Standardized the dataset manually and split into training (80%) and validation (20%) sets.  
  - **Direct Linear Regression:** Solved using the closed-form solution with matrix inversion.  
  - **Gradient Descent:** Implemented Full-batch, Mini-batch, and Stochastic Gradient Descent with convergence checks and data shuffling after each epoch.  
  - **Hyperparameter Tuning:** Investigated the effect of batch size and learning rate on RMSE and training time.

- **Results:**  
  - Analyzed **RMSE vs. Epoch** and **RMSE vs. Time** for different batch sizes and learning rates.  
  - Achieved optimal convergence with carefully tuned learning rates and batch sizes.

- **Visualizations:**  
  - Training/Validation RMSE vs. Epoch  
  - Training/Validation RMSE vs. Time  
  - Total Training Time vs. Batch Size  

- **Link:**  
  [GitHub Repository](https://github.com/ziren1/Ziren_Wang_Portfolio/blob/main/Grid_Stability_Prediction/F24_APS1070_Project_4%20(1).ipynb)

---

### 2. Salary Analysis and Hypothesis Testing  
- **Goal:**  
  Analyzed salary distributions based on **education level**, **years of coding experience**, and **work mode** (remote vs. in-person).  
  Performed **hypothesis testing** (two-sample t-test, ANOVA) and applied **bootstrap resampling** to investigate statistical differences between groups.

- **Technologies:**  
  Python, Pandas, NumPy, Matplotlib, SciPy  

- **Process:**  
  - **Data Cleaning:**  
    - Dropped missing values to ensure clean and complete data.  
    - Removed outliers using the **Interquartile Range (IQR)** method for robust analysis.  
  - **Statistical Analysis:**  
    - Conducted **two-sample t-tests** (manual and automated) to compare salary means between remote and in-person workers.  
    - Performed **ANOVA** to analyze salary variations across education levels (Bachelor’s, Master’s, Professional degrees).  
    - Applied **bootstrap resampling (10,000 samples)** to assess robustness and statistical confidence.  
  - **Data Visualization:**  
    - Created **bar plots** to visualize salary trends by education level and years of experience.  
    - Plotted **bootstrapped mean differences** to reveal hidden trends.

- **Results:**  
  - Remote workers earn slightly more on average, though not statistically significant (**p > 0.05**).  
  - Professional degree holders have significantly higher salaries than others (**p < 0.05**).  

- **Visualizations:**  
  - Bar plots by education level and work mode  
  - Bootstrapped salary distributions and mean differences  

- **Link:**  
  [GitHub Repository](https://github.com/ziren1/Ziren_Wang_Portfolio/blob/main/Grid_Stability_Prediction/wang_1007004386_assignment1.ipynb)

---

### 3. Risk Parity and Robust Portfolio Optimization  
- **Goal:**  
  Designed and compared multiple **risk-based portfolio optimization models**, including **Equal Risk Contribution (ERC)**, **Minimum Variance**, and **Robust Mean-Variance Optimization**.  
  The project focuses on achieving stable portfolio performance under estimation uncertainty and explores the relationship between **risk decomposition** and **return efficiency**.

- **Technologies:**  
  Python, NumPy, Pandas, cvxpy, Matplotlib  

- **Process:**  
  - **Model Implementation:**  
    - Built the **Equal Risk Contribution (ERC)** model ensuring each asset contributes equally to total portfolio risk.  
    - Developed **Robust Mean-Variance Optimization** using **box and ellipsoidal uncertainty sets** to mitigate estimation errors in expected returns.  
    - Constructed the **classical Markowitz MVO** for baseline comparison.  
  - **Mathematical Formulation:**  
    - Derived **KKT conditions** to verify model equivalence and ensure numerical stability.  
    - Formulated optimization problems as convex programs solvable via `cvxpy`.  
  - **Performance Evaluation:**  
    - Compared Sharpe ratios, portfolio volatility, and allocation stability across models.  
    - Conducted sensitivity analysis on uncertainty bounds to study robustness against parameter variation.

- **Results:**  
  - The **ERC portfolio** achieved the most **balanced risk distribution**, reducing sensitivity to input noise.  
  - The **Robust MVO** showed superior **out-of-sample stability** under parameter perturbations.  
  - Demonstrated that incorporating uncertainty sets yields **more resilient efficient frontiers** compared to classical MVO.  

- **Visualizations:**  
  - Efficient frontiers under nominal vs. robust assumptions  
  - Risk contribution decomposition plots  
  - Sensitivity analysis of Sharpe ratio and volatility  

- **Link:**  
  [GitHub Repository](wang_assignment2.ipynb)

---

### 4. Credit Risk Modeling via Monte Carlo Simulation  
- **Goal:**  
  Simulated credit portfolio losses to assess **capital adequacy** under extreme market conditions.  
  Compared **sampling-based (MC1, MC2)** and **analytical (Normal Approximation)** methods for estimating **Value-at-Risk (VaR)** and **Conditional VaR (CVaR)**.

- **Technologies:**  
  Python, NumPy, Matplotlib, SciPy  

- **Process:**  
  - **Simulation Design:**  
    - Modeled correlated credit defaults using **systematic and idiosyncratic factors** for 100 counterparties.  
    - Conducted **Monte Carlo simulations** with in-sample (5,000) and out-of-sample (100,000) loss distributions.  
  - **Error Analysis:**  
    - Identified **sampling error** (limited paths) and **model error** (inaccurate normal assumptions).  
    - Compared **MC1 (low sample)**, **MC2 (high sample)**, and **Normal Approximation** methods.  
  - **Risk Metrics:**  
    - Computed **99% and 99.9% VaR/CVaR** for different models.  
    - Evaluated **fat-tailed loss distributions** and their regulatory implications.  
  - **Mitigation Techniques:**  
    - Suggested **bootstrapping**, **stress testing**, and **non-parametric estimation** to enhance robustness.

- **Results:**  
  - Normal approximation **underestimated extreme losses**, implying **capital shortfalls** in high-stress scenarios.  
  - **Empirical simulations** with larger sample sizes provided more accurate tail risk estimates.  
  - Improved capital adequacy insights for **banking risk management**.  

- **Visualizations:**  
  - True vs. simulated loss distributions  
  - VaR/CVaR estimation comparisons  
  - Sampling and model error decomposition charts  

- **Link:**  
  [GitHub Repository](mie1622_assignment3.ipynb)

---

### 5. Option Pricing with Monte Carlo and Black-Scholes Models  
- **Goal:**  
  Priced **European** and **barrier options** using both **Black-Scholes** analytical formulas and **Monte Carlo simulations**.  
  Explored **path dependency**, **time-step resolution**, and **volatility sensitivity** in stochastic pricing.

- **Technologies:**  
  Python, NumPy, SciPy, Matplotlib  

- **Process:**  
  - **Analytical Benchmark:** Implemented the **Black-Scholes model** to validate results.  
  - **Monte Carlo Simulation:**  
    - Simulated **50,000 paths** with **100 time steps** to model geometric Brownian motion.  
    - Compared **one-step** vs. **multi-step** simulations for efficiency and accuracy.  
  - **Barrier Option Modeling:** Analyzed **knock-in barrier activation** probabilities and payoff variations.  
  - **Parameter Sensitivity:**  
    - Tested **volatility shifts (±10%)** and observed changes in option pricing.  
    - Conducted **grid search** for optimal balance between computational cost and accuracy.

- **Results:**  
  - Multi-step Monte Carlo produced option prices within **$0.02 of Black-Scholes** benchmarks.  
  - Barrier options exhibited strong **path dependency**, increasing in price with volatility.  
  - Achieved optimal **accuracy-runtime trade-off** for simulation parameters.

- **Visualizations:**  
  - Monte Carlo convergence plots (RMSE vs. steps/paths)  
  - Volatility sensitivity analysis  
  - Price comparison: Black-Scholes vs. Monte Carlo  

- **Link:**  
  [GitHub Repository](option_pricing.ipynb的副本)

---

## 🧠 Skills
- **Programming Languages:** Python, MATLAB  
- **Tools & Libraries:** Scikit-learn, cvxpy, SHAP, NumPy, Pandas, Matplotlib  
- **Core Skills:** Data Visualization, Machine Learning, Statistical Analysis, Optimization, Financial Modeling  

---

## 📬 Contact
- **Email:** jeffziren.wang@mail.utoronto.ca  
- **LinkedIn:** [www.linkedin.com/in/子仁-王-3a3987338](#)  
- **GitHub:** [github.com/ziren1](https://github.com/ziren1)

---
