# LASSO with K-fold cross-validation method for Diabetes Dataset


Used all of the datasets for K-fold cross-validation method.
Standarized the design matrix $X$ to compare the impact of each weight for y_predict.

## Method
Analyze the dataset of diabetes using LASSO Regression where it adds a regularization penalty to the model. This regularization penalty is based on the L1 norm.

The key aspect of LASSO is its ability to produce sparse solutions. Many of the regression coefficients are exactly zero.

The L1 penalty is the sum of the absolute values of the coefficients, mathematically expressed as $λ ∑ | β_j |$, where $𝛽_j$are the coefficients and $𝜆$ is a tuning parameter that controls the strength of the penalty.

Determine $𝜆$ Using K-fold Cross-Validation Methods.

## Features and target
Ten numeric predictive values (age, sex, bmi etc..) are features to predict diabetes predictability.
![image](https://github.com/HanaHirose/ML_Self_Study/blob/main/LASSO_K-fold_CrossVal_Diabetes/Images/dataset.png)

## Optimization using K-fold cross-validation method
検証誤差 Validation Error　$E_{valid}(λ)$　is expressed as cross-validation score (cv_score) in this K-fold cross-validation method.
**Optimized &\alpha$: 1.1623**

![image](https://github.com/HanaHirose/ML_Self_Study/blob/main/LASSO_K-fold_CrossVal_Diabetes/Images/optimize_alpha.png)


## Optimized LASSO model
Using the best $\alpha$, now you can have the optimized LASSO model loasso_opt. After fitting with the model, you get coefficients as follow:

![image](https://github.com/HanaHirose/ML_Self_Study/blob/main/LASSO_K-fold_CrossVal_Diabetes/Images/coefficient.png)


## Results
Because all the dataset was used for optimizing the LASSO model, you cannot simply evaluate how good this model is.

To compare this model to other models, like linear regression for example, I did more in [Compare_Linear_LASSO_Diabetes](https://github.com/HanaHirose/ML_Self_Study/tree/main/Compare_Linear_LASSO_Diabetes).

![image](https://github.com/HanaHirose/ML_Self_Study/blob/main/LASSO_K-fold_CrossVal_Diabetes/Images/scatter.png)



## Dataset info


Target: a quantitative measure of disease progression one year after baseline

Features: ten numeric predictive values

- age: age in years
- sex 
- bmi: body mass index
- bp: average blood pressure
- s1 tc: total serum cholesterol
- s2 ldl: low-density lipoproteins
- s3 hdl: high-density lipoproteins
- s4 tch: total cholesterol / HDL
- s5 ltg: possibly log of serum triglycerides level
- s6 glu: blood sugar level

Source URL: [link here](https://www4.stat.ncsu.edu/~boos/var.select/diabetes.html)

