# Insurance-Cost-Estimation
Insurance cost estimation analysis using decision tree, linear regression, Cross Validatioon, r squared.
we used get_dummies to convert categorical features to numberical variable for both X,y. and created a decision tree model to predict if a person smokes or not. we chose smoker as target variable for this model.

Import numpy as np: Imports the NumPy library and gives it an alias np for easier reference in the code.

Import matplotlib.pyplot as plt: Imports the pyplot module from the Matplotlib library and gives it an alias plt for easier reference in the code.

Import seaborn: Imports the Seaborn library for statistical visualization.

From scipy.stats import shapiro, ttest_ind: Imports the shapiro() and ttest_ind() functions from the scipy.stats module.

shapiro(insurance['charges']): This code line runs the Shapiro-Wilk test for normality on the insurance charges data using the shapiro() function. The insurance['charges'] part of the code refers to the charges column in the insurance data frame or data set. The output of the shapiro() function will be a tuple containing the test statistic and the p-value of the test.

shapiro(insurance['bmi']): This code line runs the Shapiro-Wilk test for normality on the insurance charges data using the shapiro() function. The insurance['bmi'] part of the code refers to the charges column in the insurance data frame or data set. The output of the shapiro() function will be a tuple containing the test statistic and the p-value of the test.

shapiro(insurance['age']): This code line runs the Shapiro-Wilk test for normality on the insurance charges data using the shapiro() function. The insurance['age'] part of the code refers to the charges column in the insurance data frame or data set. The output of the shapiro() function will be a tuple containing the test statistic and the p-value of the test.

shapiro(insurance['children']): This code line runs the Shapiro-Wilk test for normality on the insurance charges data using the shapiro() function. The insurance['children'] part of the code refers to the charges column in the insurance data frame or data set. The output of the shapiro() function will be a tuple containing the test statistic and the p-value of the test.

Report: However, upon closer inspection, it appears that the scatterplot of charges vs. bmi has a stronger linear relationship than the scatterplot of charges vs. age. This is because the points in the scatterplot of charges vs. bmi are more tightly clustered around a linear trend, while the points in the scatterplot of charges vs. age are more spread out and less tightly clustered.
Based on the results of the cross-validation, the model DecisionTreeRegressor (with an r2 score of 0.7) outperformed both the model LinearRegression (with an r2 score of 0.74) and the DummyRegressor model (with an r2 score of -0.001). Therefore, r2 score is a good scoring metric for regression models and LinearRegression is the best model for this dataset.
