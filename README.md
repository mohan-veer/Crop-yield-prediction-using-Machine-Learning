# Crop-yield-prediction-using-Machine-Learning
An approach to estimate the yield of crops

**Goal**: To estimate the crop yield(production) when provided the demographic features like State_Name, District_Name, Crop_Year, Season, Crop_Year, Crop, Rainfall(estimated) and Area.

**Datasets used are** 
* Crop_yield information("apy.csv")
* Rainfall data("rainfall.csv")

## Technical Overview

### 1. Data Preprocessing: 
* It includes maintaining consistency in data and filling the missing values. Moreover, adding a new feature to crop_yield data called "Rainfall". 
* Using different encoding techniques like Label, One-Hot and Binary encoding for converting the categorical values to model understanding numerical data.

### 2. Model Definition
* Defining 3 models using 3 different techniues
* **Random Forest Regressor**: It generates multi decision trees from which each decison tree uses a part of data sample and predicts the result. Then the result which was achieved by maximum number of trees is considered as the final prediction.
* **Decision Tree Regressor**: Decision trees are constructed through an algorithmic approach that identifies ways to split the data set based on different conditions and predicts the ouput.It is a non-parametric method.
* **Gradient Boosting Regressor**: Gradient boosting method converts the weak learners into strong learners by boosting their capability. A sequential process of learning from the previous trees and increasing the model accuracy.

### 3. Prediction
* The data is split into 80% for training and 20% for testing.
* The testing data is sent into the model for prediction and the accuracy,error rate are calculated thorugh R^2 method

#### From the observations Random Forest Regressor is the best approach for Crop_yield prediction with an R^2 value of ~0.88.
