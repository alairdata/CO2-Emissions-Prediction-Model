# CO2-Emissions-Prediction-Model

### Overview
This is a supervised machine learning project where Regression is used to predict continuous values for CO2 emissions in Canada. The goal of this project was to use data analysis and visualization to understand patterns in the data, and then use those insights to train a model that can accurately predict CO2 emissions.

The project began by importing several libraries that would be used for data handling, processing, and visualization. These included pandas and numpy for data handling, seaborn and matplotlib for visualization, and missingno for identifying missing data. The project also included a step to reduce the number of warnings that appear during execution.

Once the libraries were imported, the data was imported and described. The data contained information about various vehicle makes and models, including their engine size, number of cylinders, fuel consumption, and CO2 emissions.

The first step in the data analysis was to check for missing values and duplicates in the data. It was realized that there were no missing values, except duplicates that needed to be removed. After removing duplicates, the data was further visualized using a pairplot, which further helped to identify relationships between different features in the data.

The project then used box plots and a heatmap to understand the distribution of values in the data and identify any correlations between different features. Based on these analysis, it was determined that certain features had high correlations hence the dropping of such to avoid multi-colinearity.

The final step was to encode the non-numeric features in the data, such as "Fuel Type" and "Vehicle Class". This was done using the pd.get_dummies() function, which converts categorical variables into a set of binary variables that can be used in machine learning models.

The end result of the data analysis was a cleaned and encoded dataset that was ready to be used for machine learning modeling. The data analysis process helped to identify patterns in the data and make better predictions using machine learning by removing duplicates, identifying and removing correlated features, and encoding non-numeric features.

Now that the data had been cleaned and ready for modeling, The process of building the regression model and training it with the cleaned data was started. 

### Requirements
The code was written in python 3.8 and requires the following libraries:

pandas
numpy
seaborn
matplotlib
missingno

### Usage
Download the repository
Install the required libraries
Run the code

### Additional note
This is a simple example of how to use machine learning to predict continuous values. In a real-world scenario, there would be more data cleaning, feature engineering and model selection involved to improve the performance of the model.
