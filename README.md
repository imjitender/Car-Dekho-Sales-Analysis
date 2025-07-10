# Car-Dekho-Sales-Analysis

## Project Overview

The goal of this project is to analyze the Car Dekho dataset to understand the factors that influence the selling price of used cars. We perform a detailed Exploratory Data Analysis (EDA) to uncover trends and relationships within the data. Subsequently, we build and evaluate several machine learning models to predict the selling price of a used car based on its features. The performance of these models is then compared to identify the most effective one for this prediction task.

## The dataset used in this project is the "Car Dekho" dataset, which contains information about used cars listed on the platform. The key features of the dataset include:

Feature :- car name ,year ,selling price ,present price, km driven,fuel type ,seller type , transmission ,  owner 
Selling_Price :-The price the car is being sold for (in lakhs). (Target Variable)

## 💻 Technologies Used
Programming Language: Python 3

Libraries:

Pandas: For data manipulation and analysis.

NumPy: For numerical operations.

Matplotlib & Seaborn: For data visualization.

Scikit-learn: For machine learning model implementation and evaluation.

## 📊 Exploratory Data Analysis (EDA)
The EDA phase focused on understanding the distribution of the data and the relationships between different features. Key visualizations and findings include:

Distribution of Selling Price: The distribution of the target variable, Selling_Price, was found to be right-skewed, indicating that most cars have a lower selling price. A log transformation was applied to normalize the distribution for better model performance.

Correlation Heatmap: A heatmap was generated to visualize the correlation between numerical features. Present_Price showed a strong positive correlation with Selling_Price.

## ⚙️ Data Preprocessing and Feature Engineering
Before building the models, the following preprocessing steps were performed:

Handling Categorical Features: Categorical features like Fuel_Type, Seller_Type, and Transmission were converted into numerical format using one-hot encoding and label encoder.
Dropping Unnecessary Features: The Car_Name and Year columns were dropped as they were no longer needed after feature engineering.

Train-Test Split: The dataset was split into training and testing sets to evaluate the performance of the models on unseen data.

## 🤖 Model Building and Comparison
Several regression models were trained on the preprocessed data to predict the Selling_Price. The models evaluated are:

Linear Regression: A baseline model to establish initial performance.
Decision Tree Regressor: A non-linear model that makes predictions by learning simple decision rules.
Random Forest Regressor: An ensemble model that fits multiple decision trees and aggregates their predictions to improve accuracy and control overfitting.

Gradient Boosting Regressor: An ensemble technique that builds models sequentially, with each new model correcting the errors of the previous one.

## The models were evaluated using the following metrics:

Mean Squared Error (MSE): The average of the squared differences between the predicted and actual values.

R-squared (R2) Score: The proportion of the variance in the dependent variable that is predictable from the independent variables.

## 🏆 Results and Conclusion
Based on the comparison of the model evaluation metrics, the Random Forest Regressor performed the best with the lowest MSE, and the highest R-squared score. This indicates that the ensemble approach of Random Forest was most effective in capturing the complex relationships within the data to make accurate price predictions.

The key factors influencing the selling price of a used car were found to be the present price, the age of the car, and whether the transmission is automatic or manual.
