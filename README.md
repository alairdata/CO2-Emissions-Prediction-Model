
# CO2-Emissions-Prediction-Model ++

# Overview
This is a supervised machine learning project where Regression is used to predict continuous values for CO2 emissions in Canada. The goal of this project was to use data analysis and visualization to understand patterns in the data, and then use those insights to train a model that can accurately predict CO2 emissions.

The project began by importing several libraries that would be used for data handling, processing, and visualization. These included pandas and numpy for data handling, seaborn and matplotlib for visualization, and missingno for identifying missing data. The project also included a step to reduce the number of warnings that appear during execution.

Once the libraries were imported, the data was imported and described. The data contained information about various vehicle makes and models, including their engine size, number of cylinders, fuel consumption, and CO2 emissions.

The first step in the data analysis was to check for missing values and duplicates in the data. It was realized that there were no missing values, except duplicates that needed to be removed. After removing duplicates, the data was further visualized using a pairplot, which further helped to identify relationships between different features in the data.

The project then used box plots and a heatmap to understand the distribution of values in the data and identify any correlations between different features. Based on these analysis, it was determined that certain features had high correlations hence the dropping of such to avoid multi-colinearity.

The final step was to encode the non-numeric features in the data, such as "Fuel Type" and "Vehicle Class". This was done using the pd.get_dummies() function, which converts categorical variables into a set of binary variables that can be used in machine learning models.

The end result of the data analysis was a cleaned and encoded dataset that was ready to be used for machine learning modeling. The data analysis process helped to identify patterns in the data and make better predictions using machine learning by removing duplicates, identifying and removing correlated features, and encoding non-numeric features.

Now that the data had been cleaned and ready for modeling, The process of building the regression model and training it with the cleaned data was started. 

In this project, multiple regression models were used to predict CO2 emissions based on the cleaned and encoded dataset that was prepared in the data analysis process. The models that were used in this project include:
 - Linear Regression: Linear regression is a simple and widely used model that assumes a linear relationship between the independent variables and the dependent variable. This model was trained on the data and the results were evaluated using metrics such as mean squared error and R-squared.
 - Ridge Regression: Ridge regression is a variation of linear regression that uses L2 regularization to prevent overfitting. The regularization term adds a penalty term to the cost function, which helps to keep the coefficients of the model small. This model was trained on the data and the results were evaluated using metrics such as mean squared error and R-squared.
 - Lasso Regression: Lasso regression is another variation of linear regression that uses L1 regularization to prevent overfitting. The regularization term adds a penalty term to the cost function, which helps to keep the coefficients of the model small. This model was trained on the data and the results were evaluated using metrics such as mean squared error and R-squared.
 - ElasticNet Regression: ElasticNet regression is a combination of L1 and L2 regularization, it combines the penalties of L1 and L2 by adding both penalties to the cost function. The regularization term helps to keep the coefficients of the model small. This model was trained on the data and the results were evaluated using metrics such as mean squared error and R-squared.
 - After training and evaluating the models, the best performing model was selected based on the evaluation metric, in this case, mean squared error and R-squared. The final model can be used to make predictions on new data, with a good level of accuracy and robustness.

It's worth mentioning that, cross-validation techniques could be used to validate the results, and other more complex models could be used for prediction.

In summary, multiple regression models were used in this project to predict CO2 emissions in Canada based on the cleaned and encoded dataset. The models used include Linear Regression, Ridge Regression, Lasso Regression and ElasticNet Regression. The results of each model were evaluated using metrics such as mean squared error and R-squared, and the best performing model was selected based on these results.

It is worth noting that the **GradientBoosting model (gdabpipe)** emerged as the best model **(0.995 and 17.36)** in terms of both r-squared score and mean squared error respectively

# Requirements
The code was written in python 3.8 and requires the following libraries:
 - pandas
 - numpy
 - seaborn
 - matplotlib
 - missingno

# Usage
 - Download the repository
 - Install the required libraries
 - Run the code

# Additional notes
This is a simple example of how to use machine learning to predict continuous values. In a real-world scenario, there would be more data cleaning, feature engineering and model selection involved to improve the performance of the model.


