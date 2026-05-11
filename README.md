# Melbourne House Price Prediction Using Machine Learning
This project dives into predicting the prices of houses in Melbourne using real estate data and machine learning. Multiple regression methods were used including linear regression, decision trees and random forests, utilising hyperparameter tuning and cross validation to improve performance.

### **The goal**
The goal is to accurately predict house prices based on property attributes such as location, size, number of rooms, and other features. This can help understand the drivers of housing prices in Melbourne.

### **The data**
The [data]("https://www.kaggle.com/datasets/anthonypino/melbourne-housing-market?resource=download") used included a multitude of predictors (check notebook for full list and details) and contained 34,857 entries. Many columns had lots of missing entries which were handled using scikit learn's KNN imputer. The few categorical variables were encoded.

 ### **Some things to consider**
The although the data was thorough in terms of number of features and entries, the main limiting factor was the dates in which the data was collected. The historical data only ranged from 2016 to 2018, meaning we only have a very small window to train the model with. This ultimately means the model won't know price trends over a longer period of time, inflation factors and the current housing market. However, this does not mean the model is completely useless, it is still trained on factors that objectively make a house more expensive such as distance to CBD and size (number of rooms, bathrooms, carspots etc).
