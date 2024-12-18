# Ziren_Wang_Portfolio

Welcome to my portfolio! Here you will find some of my projects and skills showcased as part of my work in Machine Learning, Data Analysis, and Finance.

## About Me
I am currently pursuing a Master of Engineering in Mechanical and Industrial Engineering at the University of Toronto. I specialize in Machine Learning, Data Analysis, and Financial Modeling, with a strong foundation in mathematics and statistics.

## Projects
### 1. Electrical Grid Stability Prediction  
- **Goal**:  
  Developed a mathematical model to predict **electrical grid stability** using Linear Regression and Gradient Descent techniques. The project analyzes the **Electrical Grid Stability dataset** (10,000 instances, 12 features) and evaluates the impact of **batch size** and **learning rate** on convergence.

- **Technologies**:  
  Python, NumPy, SciPy, Scikit-learn, Matplotlib  

- **Process**:  
  - **Data Preparation**: Standardized the dataset manually and split into training (80%) and validation (20%) sets.  
  - **Direct Linear Regression**: Solved using the closed-form solution with matrix inversion.  
  - **Gradient Descent**: Implemented Full-batch, Mini-batch, and Stochastic Gradient Descent, with convergence checks and data shuffling after each epoch.  
  - **Hyperparameter Tuning**: Investigated the effect of batch size and learning rate on RMSE and training time.  

- **Results**:  
  - Analyzed RMSE vs. Epoch and RMSE vs. Time for different batch sizes and learning rates.  
  - Achieved optimal convergence with carefully tuned learning rates and batch sizes.  

- **Visualizations**:  
  - Training/Validation RMSE vs. Epoch  
  - Training/Validation RMSE vs. Time  
  - Total Training Time vs. Batch Size  

- **Link**: [GitHub Repository](https://github.com/ziren1/Ziren_Wang_Portfolio/blob/main/Grid_Stability_Prediction/F24_APS1070_Project_4%20(1).ipynb)  


### 2. Salary Analysis and Hypothesis Testing
- **Goal**:  
  Analyzed salary distributions based on education level, years of coding experience, and work mode (remote vs. in-person). Performed hypothesis testing (two-sample t-test and ANOVA) and applied bootstrap resampling to investigate statistical differences between groups.

- **Technologies**:  
  Python, Pandas, NumPy, Matplotlib, Scipy  

- **Process**:  
  - **Data Cleaning**:  
    - Dropped missing values to ensure no incomplete data affected the analysis.  
    - Removed outliers using the **IQR (Interquartile Range)** method for robust trend analysis.  
  - **Statistical Analysis**:  
    - Performed **two-sample t-tests** (manual and automated) to compare salary means between remote and in-person workers.  
    - Conducted **ANOVA** to compare salaries among education levels (Bachelor's, Master's, Professional degrees).  
    - Utilized **bootstrap resampling** (10,000 samples) to verify results and assess statistical robustness.  
  - **Data Visualization**:  
    - Created bar plots to visualize salary trends by education level, years of coding, and work mode.  
    - Plotted bootstrapped distributions and mean differences for deeper insights.  

- **Results**:  
  - **Work Mode**: Remote workers tend to earn more than in-person workers, though the difference was not statistically significant (p > 0.05).  
  - **Education Levels**: Professional degree holders had the highest salaries, followed by Bachelor's and Master's degree holders. The ANOVA test indicated significant differences in salaries (p < 0.05).  

- **Visualizations**:  
  - Bar plots for education levels, years of coding vs. average salary.  
  - Bootstrapped distributions and mean difference plots.  

- **Link**: [GitHub Repository](#)  


## Skills
- **Programming Languages**: Python, MATLAB
- **Tools**: SHAP, Scikit-learn, Quadratic Programming
- **Core Skills**: Data Visualization, Machine Learning, Statistical Analysis

## Contact
- **Email**: jeffziren.wang.@mail.utoronto.ca
- **LinkedIn**: [www.linkedin.com/in/子仁-王-3a3987338](#)  
- **GitHub**: [github.com/ziren1](#)
