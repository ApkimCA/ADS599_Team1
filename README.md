# From Data to Justice: Analyzing San Diego Community Review Board on Police Practice Cases for Insights and Predictive Modeling

## Team members:

-Ben Earnest

-Andrew Kim

-Grigor Tashchyan

## Objective:

-The goal of this project is to bridge the gap between the City of San Diego's efforts in sharing data and cases that investigates officer-involved shootings, in-custody deaths, and public complaints against the San Diego Police Department (SDPD) with implementing comprehensive analysis and intuitive visual representations towards each case. This, in turn, would make it simpler and accessible for the citizens of San Diego to gain insights of each police case investigated by the Community Review Board (CRB) and draw conclusions while also unlocking the potential of the Citizens' Review Board data. By implementing and enhancing the use of transparency, we aim to provide insightful data analysis and visualizations related to public complaints aginst the police in San Diego to the public.

## Data source:

https://data.sandiego.gov/datasets/crb-cases/

## Description of data:

The Complaints Evaluated by the Commission on Police Practices dataset features 12 csv files and includes all cases and incidents involving officer-involved shootings, in-custody deaths, and additional incidents that are transparent and accountable to the San Diego community the Commission on Police Practices (CPP) reviewed since the launch of FY in 2019 through 2022. The data files were acquired from the City of San Diego Open Data Portal. In each dataset, the variable “id” represents a police case number that involves a single or multiple officers per complaint. The “pid” variable labels officers being investigated towards a case “id” as anonymous person id. 

The crb case FY2019 file features 20 variables and includes rows that represents one allegation and finding per officer in the complaint. The remaining files that start from FY2020 to FY2022 contain 16 variables, with cases and allegations being separated into separate files that can coincide with “id” and “case_number” fields. Files that are labeled “case” include the number of officers involved during a case, the number of days an incident occurred, the allegation made towards officer(s), complaints involving race and/or gender, changes that were either made or not made and whether rulings were made by unanimous decision, and the police department division involved towards an incident.

Files that are labeled “allegations” contain a total of eight variables, with the key features being “allegation”, which labels the type of incident being charged towards officer(s); and “unanimous_vote, which indicates if officer(s) involved in the allegation or incident was charged, labeled “YES” or “NO”.

Files that are labeled “bwc” (body worn camera) lists police officers “pid” per complaint and assesses whether officers had a body worn camera on or off during the incident under review.

## Methods/Models used:

Predictive Modeling

## Programming Language(s):

Python through Jupyter Notebook and Visual Studio Code.
