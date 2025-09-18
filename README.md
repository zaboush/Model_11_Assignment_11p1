# What drives the price of a car?
**Assignment Jupyter Notebook URL Address:** https://github.com/zaboush/Model_11_Assignment_11p1/blob/main/prompt_II_091725.ipynb
## Note: I couldn't upload vehicles data file due its size (50.5MB) exceeding Github maximum limit of 25MB, therefore I zipped the data file and uploaded it. Please decompress the data file prior to executing my Jupyter notebook.
## Project Objectives
The business problem of identifying key drivers for used car prices can be reframed as a data problem:
Given a dataset of used cars with various features (e.g., make, model, year, mileage, condition), build a regression model to predict the price of a used car based on these features.
The goal is to identify which features have the most significant impact on the predicted price, thereby revealing the key drivers of used car prices.
## Data Description
The provided data came from Kaggle. The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing. 
## Problem Statement
The goal is to understand what factors make a car more or less expensive. As a result of our analysis, we should provide clear recommendations to our client -- a used car dealership -- as to what consumers value in a used car.
Todo that, we need to explore the data provided using our knowledge of plotting, statistical summaries, and visualization using Python. Then use various linear regression models and evaluate then to understand how each car feature contribute to the rice. We then publish our findings in a public facing github repository alongside Pthon code used to analyse the data and conclusions drawn.
## Data Understanding
**Steps for Data Understanding and Quality Assessment:**  
1. Load the dataset and display the first few rows to get a sense of the data structure and content.
2. Check the data types of each column to ensure they are appropriate for analysis.
3. Get a summary of the dataset, including the number of rows and columns, and non-null values.
4. Check for missing values in each column and visualize the missing data pattern.
5. Calculate descriptive statistics for numerical columns (mean, median, standard deviation, min, max, etc.).
6. Explore the distribution of categorical variables using value counts and visualizations (e.g., bar plots).
7. Identify potential outliers in numerical columns using visualizations (e.g., box plots, histograms).
8. Analyze the relationships between variables using correlation matrices and scatter plots.
9. Understand the meaning of each feature and how it relates to the target variable (price).
10. Document any observations, assumptions, and potential issues found during the exploration.
## Key Findings
**Based on our analysis and the Lasso model, the following features were found to be the most significant drivers of used car prices:**
- Vehicle Age and Odometer Reading: As expected, older cars with higher mileage tend to have lower prices. These are strong negative predictors of price.
- Vehicle Condition: The condition of the car has a substantial impact on its price. Cars in 'like new' or 'new' condition command higher prices, while those in 'fair' or 'salvage' condition are significantly less expensive.
- Manufacturer: The brand of the car plays a crucial role in pricing. High-end manufacturers and those with strong market demand generally have higher average prices.
- Vehicle Type: The type of vehicle (e.g., truck, SUV, sedan) is a key determinant of price, with certain types like trucks and SUVs tending to be more expensive.
- Fuel Type and Drive Type: Diesel vehicles and those with 4-wheel drive (4WD) tend to have higher prices.
- Number of Cylinders: Cars with more cylinders (often indicating larger engines) are generally more expensive.
- These findings align with common intuition about used car values and highlight the most important aspects for the dealership to consider.
## Recomendation
**Based on our analysis of the key price drivers, here are some recommendations for the used car dealership:**
- Inventory Focus: Consider stocking more diesel trucks, pickups, and SUVs, especially from manufacturers with higher positive coefficients (e.g., Toyota, Honda, Ram, GMC, BMW).
- Condition Matters: Emphasize acquiring cars in 'like new' or 'new' condition, as they command significantly higher prices. Be mindful that 'fair' and 'salvage' conditions drastically reduce value.
- Mileage and Age are Key: Educate buyers that lower mileage and newer cars are generally more valuable, which aligns with the negative impact of 'odometer' and 'age' on price.
- Highlight Desirable Features: When marketing cars, highlight features with positive price impacts like 4WD, higher cylinder counts, and desirable body types.
- Pricing Strategy: Use the insights from the coefficients to inform pricing strategies for different makes, models (implicitly captured by manufacturer and type), conditions, and mileages.
