#### Feature Selection Techniques

Feature selection is the process of reducing the number of input variables when developing a predictive model. It is desirable to reduce the number of input variables to both reduce the computational cost of modeling and, in many cases, to improve the performance of the model. Statistical-based feature selection methods involve evaluating the relationship between each input variable and the target variable using statistics and selecting those input variables that have the strongest relationship with the target variable. These methods can be fast and effective, although the choice of statistical measures depends on the data type of both the input and
output variables.


**There are two main types of Feature Selection:**

**Supervised Selection:**  

Use the target variable (e.g. remove irrelevant variables). it is further categorized into three main categories. 
    
    - Filter Method
    Select subsets of features based on their relationship with the target.
        - Basics: (Constant, Quasi-Constant, Duplicated)
        - Correlation 
        - Statistical measures: (Fisher Score, Univariate method, mutual information)

    - Wrapper method:
    Search subsets of features that perform according to a predictive model.
        - Step forward Selection 
        - Step Backward Selection 
        - Exhaustive Search 
        - Feature shuffling 

    - Embedded Methods:
        - LASSO
        - Decision tree derived importance 
        - Regression Coefficients 

    - Hybrid Methods:
        - Recursive Feature Elimination 

**Unsupervised Learning**

Do not use the target variable (e.g. remove redundant variables). Unsupervised feature selection techniques ignore the target variable, such as methods that
remove redundant variables using correlation or features that have few values or low variance(i.e. data cleaning).


#### Detail Listing 

1. **Basic Selection Methods**
	1. Removing Constant Features
	2. Removing Quasi-Constant Features
	3. Removing Duplicated Features

2. **Correlation Feature Selection**
	1. Removing Correlated Features 
	2. Basic Selection Methods + Correlation - Pipeline

3. **Filter Methods: Univariate Statistical Methods**
	1. Mutual Information
	2. Chi-square distribution
	3. Anova
	4. Basic Selection Methods + Statistical Methods - Pipeline

4. **Filter Methods: Other Methods and Metrics**
	1. Univariate roc-auc, mse, etc
	2. Method used in a KDD competition - 2009

5. **Wrapper Methods**
	1. Step Forward Feature Selection
	2. Step Backward Feature Selection
	3. Exhaustive Feature Selection

6. **Embedded Methods: Linear Model Coefficients**
	1. Logistic Regression Coefficients
	2. Linear Regression Coefficients
	3. Effect of Regularization on Coefficients
	4. Basic Selection Methods + Correlation + Embedded - Pipeline 

7. **Embedded Methods: Lasso**
	1. Lasso 
	2. Basic Selection Methods + Correlation + Lasso - Pipeline 

8. **Embedded Methods: Tree Importance**
	1. Random Forest derived Feature Importance
	2. Tree importance + Recursive Feature Elimination
	3. Basic Selection Methods + Correlation + Tree importance - Pipeline

9. **Hybrid Feature Selection Methods**
	1. Feature Shuffling
	2. Recursive Feature Elimination
	3. Recursive Feature Addition