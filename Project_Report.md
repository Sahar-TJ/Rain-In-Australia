# Project Report

## [Rain in Australia](https://github.com/Sahar-TJ/Rain-In-Australia)

<img alt="Name" src="https://img.shields.io/badge/Name-Sahar%20Tosif%20Jamal-orange"/>    

## Introduction
This is the report of Rain in Australia Project where I analyzed Australia's weather data which had various features. The objective of the project was to understand the rain patterns and predict the possibility of rain on the following day using various models. The target variable here is RainTomorrow. The report will discuss the key aspects of the data, including data cleaning, feature analysis, model selection, and evaluation.

### Reason for choosing the dataset:
It's been a while since I moved to Sydney and one thing that I noticed is the weather here is the most unpredictable one. Since then I have been curious about what the weather would be the next day or even in the next few hours. As I was exploring, I came across the [Rain in Australia](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package) dataset, which attracted me. My interest in working on the data rose because of the fact that I have been too intrigued with the weather in Australia.

### Identify the problem
After importing the data, it was important to understand what all features were present and how they were related to the other features. Another thing that had to be understood was the effect of a certain feature on the target variable, i.e. RainTomorrow. It is always taught to first understand the data, by checking what the data is trying to say, find the missing values, then analyze the data and lastly perform suitable modeling techniques which allows you to gather the right insights. Some of the major challenges were: first I had to understand how the data is set, how many missing values are present and how can they be treated. Others include finding the outliers and treating them, and finally selecting the right model and evaluating the results.

### Dealing with the problems
Once the problems were identified, it was time to deal with them. I first had to understand the data and find the total number of missing values. For numerical and categorical columns, the median and mean of the columns were taken respectively, and replaced with the missing values. The outliers were also identified and removed by using IQR. The correlation of the dataset was analyzed and identified the features with strong relationships with the Rainfall column. An Exploratory Data Analysis of the data was performed to understand the data features separately in depth. Some visualizations of the data also eased the tasks.  The distribution of Rainfall over the period of time and location was visualized. 

Once the data was cleaned and visualized, it was time to split it into train and test dataset and analyze further by using different models. 70% of the cleaned data was split into training data while 30% was reserved for testing. To predict the likelihood of rain, a few models were considered, including Gaussian Naive Bayes, Linear Regression, Logistic Regression, and K-Nearest Neighbors (KNN). The accuracy of each model was compared and Cross-validation was then conducted with 5 to 9 folds for the best models to further evaluate the performance of the models.

### Models
4 models were used to predict the Rain on the following day and their performance was compared: Gaussian Naive Bayes, Linear Regression, Logistic Regression, and KNN.

- **Gaussian Naive Bayes:** It is a very common machine learning classification algorithm that assumes naive independence between features. It simplifies the modeling process, is efficient, and can handle large datasets with many features. In the Rainfall data, some of the features, such as temperature, humidity, and wind speed, can be assumed to follow a Gaussian distribution. Gaussian NB takes advantage of this assumption to estimate the likelihood of rain.  The probabilistic nature allows for easy interpretation and understanding of the model's predictions. The model was evaluated using a classification report that told about the model was 81% accurate.

- **Linear Regression:** Linear regression allows us to assess the linear relationship between the independent variables and the dependent variable (RainTomorrow). It is efficient and simple compared to other complex modeling techniques. It is used for predictive purposes by estimating the probability of rain tomorrow based on other features. The model was evaluated using various metrics like Mean Squared Error, R-square, and Root Mean Square.

- **Logistic Regression:** This statistical technique is widely used for binary classification problems. It models the relationship between predictor variables (e.g., temperature, humidity) and the probability of rain. It can handle imbalanced datasets, capture non-linear relationships, and allows the modeling of complex relationships. We evaluated the model by extracting the classification report of the model that tells us about the accuracy, F1 score, precision, and Recall. However a cross-validation was performed on the model with 9 folds and the results were quite better as compared to the other models, 86%. 

- **K-Nearest Neighbors:** KNN is a versatile machine learning model for classification and regression tasks. It is a non-parametric algorithm that doesn't assume an underlying data distribution. KNN identifies clusters by considering the nearest neighbors. The key hyperparameter is K, representing the number of neighbors considered. Here the K was set as 5 and 9 and checked where the KNN model performs well. A classification report and cross-validation technique was used to evaluate the performance of the model. The accuracy of k=5 was 85% whereas k=9 had a better accuracy, 86%. 

### Conclusion 

The very first step, Data Cleaning plays a critical role in any project. In order to clean, there are various techniques one can use. Understanding what data is trying to tell is another important step, we use EDA to understand it. Even after cleaning not all data is ready to be fit for training or testing, that's where the data preprocessing comes in and allows us to make the data usable. It involves treating the outliers, normalization, and converting into the same format. The cleaned and processes data is ready for training and testing. We can then use various types of models and evaluate the results. Feature selection and evaluation techniques helps in understanding their value in any project. 

Overall, this project teaches how to analyze Australia's rainfall patterns and develop a predictive model. The project involved data cleaning, exploratory data analysis, feature analysis, model selection, and evaluation. Through this project, I gained hands-on experience in data preprocessing, model training, and cross-validation. This project enhanced my understanding of how to get the best-performing model for the data.

## Thank You!