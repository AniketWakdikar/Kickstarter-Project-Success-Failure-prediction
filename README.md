# Kickstarter-Project-Success-Failure-prediction

# About Dataset
The dataset contains information about past Kickstarter projects, including features such as project category, funding goal, project launch and deadline date, project backers and historical project outcomes.

# Problem Statement
The objective of this project is to develop a machine learning model that can predict whether a Kickstarter project will be successful or not based on various project attributes and historical data.

Source of the dataset: https://www.kaggle.com/datasets/kemical/kickstarter-projects

# Data Dictionary
Features in Original dataset-- id: A unique identifier for each Kickstarter project. name: The name or title of the project. category: The category of the project. sub_category: The sub-category of the project. currency: The currency used for the funding goal and pledges. deadline: The date and time by which the project needs to reach its funding goal. goal: The funding goal set by the project creator. launched: The date and time when the project was launched on Kickstarter. pledged: The amount pledged by backers so far. state: The current state of the project (successful, failed, live, etc.). backers: The number of backers who have supported the project. country: The country where the project creator is located. usd_pledged:The amount pledged by backers converted to USD. usd_goal: The funding goal converted to USD.

Features Added- days: The difference between launch-date and deadline of project. backer_goal:The target usd_goal to be fulfilled by each backer. year: The year when the project was launched. quarter: The quarter of the year when the project was launched. Major Cat: The major category of the project. GDP (current US ): 𝑇ℎ𝑒 𝐺𝑟𝑜𝑠𝑠𝐷𝑜𝑚𝑒𝑠𝑡𝑖𝑐𝑃𝑟𝑜𝑑𝑢𝑐𝑡(𝐺𝐷𝑃) 𝑜𝑓 𝑡ℎ𝑒 𝑐𝑜𝑢𝑛𝑡𝑟𝑦 𝑖𝑛 𝑐𝑢𝑟𝑟𝑒𝑛𝑡 𝑈𝑆𝑑𝑜𝑙𝑙𝑎𝑟𝑠. 𝐺𝐷𝑃𝑝𝑒𝑟𝑐𝑎𝑝𝑖𝑡𝑎(𝑐𝑢𝑟𝑟𝑒𝑛𝑡𝑈𝑆): The GDP per capita of the country in current US dollars.

# SUMMARY OF PROBLEM STATEMENT, DATA AND FINDINGS

The project involves the analysis of Kickstarter projects, leveraging a dataset containing information about various project attributes such as project category, funding goals, launch dates, historical outcomes, and more. The primary goal is to develop a machine learning model that predicts the success or failure of Kickstarter projects based on these attributes and historical data.
Data:
The dataset encompasses a variety of features, including:
Original Features:
Project identifier (id).
Project name or title (name).
Project category.
Sub-category.
Currency used for funding goals and pledges.
Project deadline.
Funding goal set by the creator.
Launch date of the project.
Amount pledged by backers.
Current project state (e.g., successful, failed).
Number of backers.
Country of the project creator.
Pledged amount converted to USD.
Funding goal converted to USD.
Additional Features:
Time duration of the project (days).
Backer's individual USD funding goal (backer_goal).
Year of project launch.
Quarter of the year when the project was launched.
Major category of the project.
Current US GDP (Gross Domestic Product) for the country.
GDP per capita for the country in current US dollars.
Findings:
The capstone project likely involved the analysis and exploration of the provided dataset, along with the development and evaluation of machine learning models for predicting Kickstarter project success. Detailed findings may include insights into which project attributes significantly influence project outcomes, the effectiveness of the machine learning model, and any correlations between economic factors (such as GDP) and Kickstarter success rates.

These findings may have practical implications for Kickstarter creators, investors, and stakeholders, offering guidance on how to improve project success rates and make more informed decisions.

# OVERVIEW OF THE FINAL PROCESS
Methodology Overview:

Descriptive Analysis:
The analysis began with an exploration of the dataset to understand its structure, distributions, and key characteristics.
Data Type Transformation:
Data types were adjusted as needed to ensure proper data handling and analysis.
Analysis and Treatment of Target Variable:
The target variable, which originally had multiple states, was transformed into a binary classification problem. Some states like "cancelled" and "suspended" were merged into the "failed" state, while others were dropped.
Treatment of Missing Values:
Missing values in the dataset were addressed using appropriate techniques, which could include imputation, removal, or other strategies.
Dropping Redundant Columns:
Columns that were deemed redundant or irrelevant for the analysis and modeling were dropped to streamline the dataset.
Analysis of Column "Main Category":
The "category" feature was merged into 10 major categories for ease of analysis and modelling, simplifying the feature space.
Treatment of Outliers:
Outliers, especially extreme ones, were identified, removed, and treated using suitable techniques.
Multicollinearity Check:
The presence of multicollinearity among independent variables was assessed to ensure the model's stability and interpretability.
Univariate and Bivariate Analysis:
Analysis of individual variables and their relationships with the target variable was conducted to gain insights.
Normality Check:
The normality of the data distribution was examined to guide model selection and assumptions.
Statistical Tests for Categorical Variables:
Relevant statistical tests were applied to categorical variables to determine their significance in predicting project outcomes.
Data Preparation for Modelling:
After all preprocessing steps, the data was ready for modelling.
Feature Selection:
Forward and backward feature selection techniques were applied to identify the most relevant features for modelling.
Model Selection and Application
A variety of machine learning algorithms were used, including logistic regression, K-nearest neighbors (KNN), Naive Bayes, decision tree, random forest, ADA boost, gradient boost, and XG boost.

The methodology involved a systematic approach to data preprocessing, exploratory analysis, and model selection, with a focus on optimizing the dataset for effective binary classification. The use of various algorithms allowed for model comparison and selection of the most suitable one for predicting Kickstarter project success or failure.
