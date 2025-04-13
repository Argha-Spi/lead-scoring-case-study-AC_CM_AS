Lead Scoring Case Study - README
Project Overview
This project aims to improve the lead conversion rate for X Education, an online course provider. Currently, the company converts only 30% of leads, and the goal is to develop a Lead Scoring Model that helps the sales team focus on high-potential leads, improving efficiency and boosting conversions to 80%.

Project Objectives
Develop a Logistic Regression Model to predict lead conversion.
Assign a Lead Score (0-100) to each lead based on probability.
**Prioritize Hot Leads ** for focused sales efforts.
Provide business recommendations to optimize marketing and sales strategies.
Dataset Information
The dataset contains 9,240 records with lead information.
Key features include Lead Source, Last Activity, Total Time Spent on Website, Specialization, etc.
The target variable is Converted (1 = Converted, 0 = Not Converted).
Steps Followed
Data Cleaning & Preprocessing:

Removed columns with excessive missing values.
Handled missing values using mode/median imputation.
Encoded categorical variables using One-Hot Encoding.
Exploratory Data Analysis (EDA):

Analyzed conversion trends based on Lead Source, Last Activity, and Specialization.
Identified that Total Time Spent on Website is a strong predictor of conversion.
Model Building:

Used Logistic Regression for classification.
Achieved an Accuracy of 78% and an ROC-AUC score of 0.86.
Generated Lead Scores (0-100) to rank leads by conversion probability.
Business Insights & Recommendations:

Hot Leads (>70 Score) should be prioritized for sales calls.
Referrals & Welingak Website leads convert at a higher rate.
Bounced Emails negatively impact conversion, requiring better follow-up strategies.
Key Files in This Repository
Leads.csv → Raw dataset containing lead information.
Lead Scoring Model.ipynb → Jupyter Notebook with the full analysis and model implementation.
Assignment Subjective Questions.docx → Answers to business-related questions.
Lead Scoring Presentation.pdf → PPT summarizing findings and recommendations.
Lead Scoring Summary.pdf → A detailed report covering the entire project.
How to Run This Project
Clone the repository: git clone (https://github.com/Argha-Spi/lead-scoring-case-study-AC_CM_AS)

Install required dependencies:

pip install -r requirements.txt

Open the Jupyter Notebook and run all cells:

jupyter notebook Lead Scoring Model.ipynb

Future Enhancements
Experiment with Decision Trees & Random Forest for improved accuracy.
Implement Automated Lead Categorization with AI-driven recommendations.
Develop a Web Dashboard to visualize lead scores in real-time.
Build a logistic regression model to assign a lead score between 0 and 100 to each of the leads which can be used by the company to target potential leads. A higher score would mean that the lead is hot, i.e. is most likely to convert whereas a lower score would mean that the lead is cold and will mostly not get converted.
There are some more problems presented by the company which your model should be able to adjust to if the company's requirement changes in the future so you will need to handle these as well. These problems are provided in a separate doc file. Please fill it based on the logistic regression model you got in the first step. Also, make sure you include this in your final PPT where you'll make recommendations.
