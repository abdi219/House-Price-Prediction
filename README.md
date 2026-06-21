# House Price Prediction

This project was completed as part of the AI/ML Engineering Internship at DevelopersHub Corporation.

---

## Project Overview
This project focuses on predicting house prices using machine learning techniques based on various property features such as area, number of bedrooms, bathrooms, stories, parking, and location-related attributes. The goal is to build a regression model that can estimate house prices with reasonable accuracy.

---

## Dataset
The dataset used is `Housing.csv`, which contains information about residential properties including both numerical and categorical features.

Target variable:  
- price

Features used:  
- area  
- bedrooms  
- bathrooms  
- stories  
- parking  
- mainroad  
- guestroom  
- basement  
- hotwaterheating  
- airconditioning  
- prefarea  

---

## Data Preprocessing
The following preprocessing steps were performed:

- Selected relevant features for modeling
- Converted categorical variables (yes/no) into numerical format (1/0)
- Handled missing values using median imputation for numeric columns
- Created a cleaned dataset for training and testing

---

## Exploratory Data Analysis
- Distribution of house prices was analyzed and found to be right-skewed
- Relationship between area and price shows a positive correlation, indicating that larger houses generally have higher prices

---

## Model Used
A Gradient Boosting Regressor was used for prediction. This ensemble model builds multiple decision trees sequentially to improve prediction accuracy.

Model parameters:
- n_estimators = 200
- learning_rate = 0.1
- max_depth = 4
- random_state = 42

---

## Model Training
The dataset was split into training and testing sets using an 80/20 ratio. The model was trained on the training data and evaluated on the test data.

---

## Evaluation Metrics
- Mean Absolute Error (MAE): approximately 986,120
- Root Mean Squared Error (RMSE): approximately 1,331,352
- R-squared Score: approximately 0.65

---

## Results Interpretation
- The model explains around 65% of the variance in house prices
- Average prediction error is around 1 million
- Area, bathrooms, and air conditioning were found to be the most influential features

---

## Conclusion
The model demonstrates moderate predictive performance. Further improvements can be achieved by feature engineering, hyperparameter tuning, and handling outliers more effectively.
