# Predictive-Analysis-Supervised-Learning---Electricity-Price-Prediction
The aim of this task is to predict the daily price of electricity based on the daily consumption of heavy machinery used by businesses. 

This project will describe the approach taken to solve this problem using Decision Tree Regressor and Support Vector Machine. The report will cover the following topics: data exploration and analysis, data pre-processing and transformation, implementation of the classifiers, evaluation of the performance of the classifiers, and actionable insights and recommendations for businesses based on the findings.

### Data Exploration and Analysis
The dataset used for this task is the 'energy_dataset.csv'. The dataset contains information on the daily electricity consumption of heavy machinery used by businesses. A new dataframe was created by selecting specific columns, which were found to be relevant to the problem at hand. The correlation between the selected variables was visualized using a heatmap. It was found that there was a positive correlation between 'ActualWindProduction' and 'ForecastWindProduction' and a negative correlation between 'SystemLoadEP2' and 'CO2Intensity'.There is positive correlation with month and the WeakofYear.
![Boxplot of distribution of variables](https://github.com/zarifshawon/Predictive-Analysis-Supervised-Learning---Electricity-Price-Prediction/blob/main/boxplot.png)

### Data Pre-processing and Transformation

The dataset contained missing values represented by '?' which were replaced with the mean of the respective column. The columns were then converted to a float data type. Categorical features were converted to numeric, and discrete features were converted to binary. The dataset was then split into training and testing sets with a test size of 20% and a random state of 42.
Implementation of the Classifiers: Two classifiers, Decision Tree Regressor and Support Vector Machine, were implemented to predict the price of electricity based on consumption data. The Decision Tree Regressor was created with a random state of 42. The Support Vector Machine was created without any parameters.

### Evaluation of the Performance of the Classifiers

The performance of the classifiers was evaluated using the Mean Squared Error, R^2 Score, and Explained Variance Score. The performance of the Decision Tree Regressor was found to have a Mean Squared Error of 936.6185, an R^2 Score of 0.218491, and an Explained Variance Score of 0.219437. On the other hand, the performance of the Support Vector Machine was found to have a Mean Squared Error of 895.3875, an R^2 Score of 0.25289, and an Explained Variance Score of 0.285522. The Support Vector Machine performed better than the Decision Tree Regressor.

## Actionable Insights and Recommendations
The analysis revealed that the 'ActualWindProduction' and 'ForecastWindProduction' had a positive correlation with the price of electricity while 'SystemLoadEP2' and 'CO2Intensity' had a negative correlation. Businesses can use this information to understand the factors affecting the price of electricity and make informed decisions regarding their energy consumption. Based on the performance of the classifiers, businesses can use the Support Vector Machine to predict the price of electricity based on consumption data.

## Conclusion
The analysis of the electricity price prediction problem using Decision Tree Regressor and Support Vector Machine showed that the Support Vector Machine performed better. The analysis also revealed the factors affecting the price of electricity, which can be useful for businesses to make informed decisions regarding their energy consumption. The findings of this analysis can be used to make recommendations for businesses to predict the price of electricity based on consumption data.


