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