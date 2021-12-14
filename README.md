# Agriculture - Project

![alt text](https://github.com/immanuvelprathap/Agriculture-Project/blob/main/farmer.jpg)

Project: Predicting Crops Yield : A Machine Learning Approach.
Problem: Predict crops yield for 10 of most consumed crops worldwide.

Environment
OS: Mac OS
Python : 3
Anaconda 64 bit 

Install
This project requires Python and the following Python libraries installed:

NumPy
Pandas
matplotlib
scikit-learn 
seaborn
pydot
graphviz

Code is provided in the prediction_model_yield.ipynb. 


Dataset:
http://www.fao.org/home/en/  
https://data.worldbank.org/ 


# Domain Background

Yield prediction is a very important issue in agricultural. Any farmer is interested in knowing how much yield he is about to expect. In the past, yield prediction was performed by considering farmer's experience on field and crop. The yield prediction is a major issue that remains to be solved based on available data.
Problem Statement
The basic ingredients that sustain humans are similar. We eat a lot of corn, wheat, rice and other simple crops. In this project the prediction of top 10 most consumed yields all over the world is established by applying machine learning techniques.
The science of training machines to learn and produce models for future predictions is widely
used, and not for nothing. Agriculture plays a critical role in the global economy. With the
continuing expansion of the human population understanding worldwide crop yield is central to
addressing food security challenges and reducing the impacts of climate change
Information can be converted into knowledge about historical patterns and future trends, the goal of this project is to predict crops yield from topmost consumed crops worldwide.
Crop yield prediction is an important agricultural problem. The Agricultural yield primarily depends on weather conditions (rain, temperature, etc), pesticides and accurate information about history of crop yield is an important thing for making decisions related to agricultural risk management and future predictions.
 yield worldwide for 10 most consumed crops. It is a regression problem.
In this project I will predict crops
  
# Datasets and Inputs

 In this project, machine learning methods are applied to predict crop yield using publicly available data from FAO and World Data Bank.
These corps include:
 • Cassava
• Maize
• Plantains and others
• Potatoes
• Rice, paddy
 • Sorghum
• Soybeans
• Sweet potatoes
• Wheat
• Yams

# Input Data fields:
•
 The final dataframe will have: Item collected, country, yield, rain, pesticides and temperature
 values:
 crops yield of ten most consumed crops around the world was downloaded from FAO
 website. The collected data includes; country, item, year starting from 1961 to 2016 and
 yield value for these years.
 • The climatic factors include rainfall and temperature. They’re abiotic components, including pesticides and soil, of the environmental factors that influence plant growth and development.
• Rain has a dramatic effect on agriculture, for this project rain fall per year information was gathered from World Data Bank.
• Pesticides used for each item and country was also collected from FAO database.
 • Average Temperature for each country was collected from World Bank Data.
 
# Solution Statement

The solution is predictions of yield of crops worldwide based on collected data. First, I will clean the collected data, merge the dataframes together based on common columns and explore relations between the different variables for correlation. Then I will perform normalization to establish a common scale for all the features, transform any categorical data such as country and crops name to numerical form.
 For training I will split the data 70% training to 30% testing and apply different machine learning algorithms to compare which delivers best results.
The total size of the dataset is expected to be 200MB, the files that contain the data has been collected, and final datafame is expected to have: item (crop) country, year, yield value, average rainfall, pesticides and average temperature.

# Models that will be used: For this project, we'll compare between the following models:
 • Gradient Boosting Regressor
• Random Forest Regressor
• SVM
• Decision Tree Regressor

# Benchmark Model

Evaluation Metrics
Function: sklearn.metrics.r2_score

# Project Design

After cleaning and exploring the relationship between the features, the final dataframe that contains all the features that will be used for the prediction process can be seen below in the screenshots:
• Area: country of production.
• Item: type of crop.

 Default SciKit-Learn Gradient Boosting Regressor and Random Forest Regressor will be used as benchmarks. Several models will then be explored to improve over the benchmark including Decision Tree Regressor and Support-Vector Machines (SVM).
 This function computes subset accuracy: the set of labels predicted for a sample
must exactly match the corresponding set of labels in y_true. For this problem, a model that will preferably achieve an accuracy over 90%.

# The evaluation metric will be the R^2 (coefficient of determination) regression score function, that will represents the proportion of the variance for items (crops) in the regression model.

• Year: year of production.
• Average_rain_fall_mm_per_year: Average amount of rain recorded that year.
• Hg/ha_yield: country’s yearly production of the crop that year.
• Pesticides_tonnes: Amount of pesticides used on the crop that year.
• Avg_temp: Average temperature recorded for that year.
