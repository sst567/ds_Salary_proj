# Salary Estimator
Built a tool to estimate salaries based on glassdoor job posting (MAE ~ 14K)
Performed data cleaning, Exploratory Data Analysis and Model Building as part of the project.

#Web Scraping and dataset used is from 2020

Web Scraping code: https://github.com/arapfaik/scraping-glassdoor-selenium

#Data Cleaning

As part of Data Cleaning removed rows which didn't contain salary.
Added a column to identify if job posting was at the same location as the company headquarters.
Made columns for skillsets based on job description including (Python, SQL, AWS, R Studio, Excel)
Simplified seniority and job roles.
Identified age of the company. 
Modified company text to not contain rating.
Column to check description length

#EDA -- Exploratory Data Analysis

Explored how job title, seniority, skills, location etc.. had an influence on the salary. 
Analyzed the number of job postings based on sector, type of company, location, rating, skill type.

#Model Building

Transformed categorical variables to dummy variables. Split the data into 80:20 ratio (Train:Test).
Verified using 3 different models, liner regression, lasso regression and Random Forest. 

Random forest outperformed the other 2 models with an MAE of approximately 14.

#Finally converted the model to a pickle file which could be integrated with an API such as Flask in the future.

Language: Python

Libraries Used: Numpy, Pandas, Matplotlib, Seaborn, Scikit-learn
