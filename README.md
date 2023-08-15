# From Data to Justice: Analyzing San Diego Community Review Board on Police Practice Cases for Insights and Predictive Modeling


## Team members:

+ Benjamin Earnest

+ Andrew Kim

+ Grigor Tashchyan

## Objective:

The objective of this project is to bridge the gap between the City of San Diego’s efforts to share data on cases brought to the CRB, and the public’s ability to understand it. We will provide a comprehensive analysis and intuitive visual representations. We will uncover patterns, trends, and distributions within the data, enabling the public to gain a deeper understanding of CRB outcomes. We will also build a predictive model, which will forecast the likelihood of outcomes based on data in a complaint. This will allow us to identify and report to the public which variables play a significant role in predicting CRB outcomes.


## Data source:

https://data.sandiego.gov/datasets/crb-cases/

## Data set(s) used:
The Complaints Evaluated by the Commission on Police Practices data sets were made available from the City of San Diego’s public website in CSV format and can be accessed at the following link. 
https://data.sandiego.gov/datasets/crb-cases/

## Description of data set(s):
The data features 12 csv files and includes all cases and incidents involving officer-involved shootings, in-custody deaths, and additional incidents that are transparent and accountable to the San Diego community the Commission on Police Practices (CPP) reviewed since the launch of FY in 2019 through 2022. In each dataset, the variable “id” represents a police case number that involves a single or multiple officers per complaint. The “pid” variable labels officers being investigated towards a case “id” as anonymous person id. 

The crb case FY2019 file features 20 variables and includes rows that represents one allegation and finding per officer in the complaint. The remaining files that start from FY2020 to FY2022 contain 16 variables, with cases and allegations being separated into separate files that can coincide with “id” and “case_number” fields. Files that are labeled “case” include the number of officers involved during a case, the number of days an incident occurred, the allegation made towards officer(s), complaints involving race and/or gender, changes that were either made or not made and whether rulings were made by unanimous decision, and the police department division involved towards an incident.

Files that are labeled “allegations” contain a total of eight variables, with the key features being “allegation”, which labels the type of incident being charged towards officer(s); and “unanimous_vote, which indicates if officer(s) involved in the allegation or incident was charged, labeled “YES” or “NO”.

Files that are labeled “bwc” (body worn camera) lists police officers “pid” per complaint and assesses whether officers had a body worn camera on or off during the incident under review.

## Methods/Models used:


+ AUC-ROC Curve

+ Data Acquisition

+ Data Aggregation

+ Data Cleaning

+ Decision Tree

+ Exploratory Data Analysis (EDA)

+ Feature Engineering

+ K-Nearest Neighbors

+ Logistic Regression

+ Predictive Modeling

+ Random Forest

+ Support Vector Machine (SVM)

+ Variable Encoding

## Programming Language(s):
Python through Visual Studio Code, SQL connection.
