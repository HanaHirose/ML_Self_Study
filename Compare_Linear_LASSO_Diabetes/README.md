# Analysis of Comparative Performance between LASSO and Linear Regression for Diabetes Dataset


## Comparison between two models
- LASSO with K-fold cross-validation method
- Simple linear regeression

Used 80 % of datasets as training data and 20 % as test data.

**Compared $R^2$ (coefficient of determination) between the two models**
- LASSO: 0.45605
- Linear regression: 0.45260

## Comparative Insights into LASSO and Linear Regression Models for the Diabetes Dataset
The coefficient of determination $R^2$ was almost same with LASSO (0.45605) and Linear Regression (0.45260) for the diabetes dataset. This means the performance of LASSO and linear regression is almost same here. 

This may mean that this dataset is not so complex so that simple linear regression can work enough for the dataset while Regularization applied by LASSO is not particularly effective for this specific dataset.




![image](/Images/compare_lesso_linear.png)


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


