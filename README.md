# From Data to Justice: Analyzing San Diego Community Review Board on Police Practice Cases for Insights and Predictive Modeling


## Team members:

+ Benjamin Earnest

+ Andrew Kim

+ Grigor Tashchyan

## Abstract:

Transparency and accountability serve as major decades-long issues in policing amid a growing rate of misconduct reports directed to the police departments. The city of San Diego has established a Citizen and Community Review Boards (CRB) to address police department accountability. The data from CRB decisions is provided on the City of San Diego website in raw form. This makes it difficult for the public to reasonably draw conclusions about CRB outcomes. Our study showed that valuable and interpretable insights can be easily generated and made available to the public, beyond just providing the raw data. We also showed that machine learning can be used to predict CRB outcomes, and show the most important variables in predicting CRB outcomes.  Using data from the City of San Diego’s website, the data were processed and balanced for use in predictive modeling through Python. Many different classification models were trained and tested, and throughout our modeling process,  we found that the SVM (with a linear kernel) model performed the best. We were also able to show the most important features in predicting CRB outcomes, which included allegations of Force, Discrimination, or failure to follow procedure. To further promote transparency and bridge this knowledge gap, we recommend using additional data related to the cases.  We also suggest the city provide results of data analyses on their website via interactive dashboards, and deploy a similar machine learning model on their website.  The city can also create a web application that would enable residents to file, review, and track the progress of reported cases.  The application can provide interactive information similar to our study, including the ability to predict an outcome based on user data.

## Background:

In November 2020, the citizens of San Diego approved the passing of Measure B, which mandated the creation of a Commission on Police Practices (CPP) that would be rebranded from the city’s original Community Review Board on Police Practices and be tasked to oversee and conduct impartial investigations into officer-involved shootings, officer misconduct, and in-custody deaths toward the San Diego Police Department (SDPD) (City of San Diego Open Data Portal, 2019). In addition to providing more robust community oversight of law enforcement, the measure was also created to evaluate public complaints against the SDPD and make recommendations on police officer discipline, which would ensure accountability and transparency in police practices amid negotiations with the San Diego Police Officers Association (SDPOA) for months. Two-and-a-half years after its approval, the commission stopped reviewing police-incident cases. As a result, the SDPD closed multiple internal police investigations and provided no input, including intuitive visual representations pertaining to cases and properly reviewed outcomes, from the city’s oversight commission to the public. Since the cessation, the commission’s membership has dwindled and the commission is dealt with a stock load of cases, which is compromising its ability to function properly and leaving San Diegans dry of thorough analysis and supportive information toward police-incident cases.

## Problem Identification/Summary:

The City of San Diego does not provide comprehensive analysis and intuitive representations of cases brought to the CRB. The City of San Diego also does not depict any insights on features (i.e., Internal Affairs’ finding, body-worn camera footage, complaints involving race and gender, CRB’s voting process unanimous or not unanimous, etc.) or supportive evidence that play contributing factors toward CRB’s final decisions. This, in turn, makes it difficult for the city’s residents to gain insights from CRB actions, properly draw insightful conclusions, or see trends related to complaints and CRB outcomes.

## Objective:

The objective of this project is to bridge the gap between the City of San Diego’s efforts to share data on cases brought to the CRB, and the public’s ability to understand it. We will provide a comprehensive analysis and intuitive visual representations. We will uncover patterns, trends, and distributions within the data, enabling the public to gain a deeper understanding of CRB outcomes. We will also build a predictive model, which will forecast the likelihood of outcomes based on data in a complaint. This will allow us to identify and report to the public which variables play a significant role in predicting CRB outcomes.

## Scope of Analysis:

Our project will include every element within our selected data sets, and will not include IA Findings and CRB Decision columns for deep analysis since we will craete a feature to capture CRB outcomes.

## Approach:

Our analysis focuses on analyzing patterns, trends, and distributions within the data to gain a candid comprehension of key factors that lead to outcomes of CRB rulings and for the public to better comprehend in society. 


## Data source:

https://data.sandiego.gov/datasets/crb-cases/

## Data set(s) used:
The Complaints Evaluated by the Commission on Police Practices data sets were made available from the City of San Diego’s public website in CSV format.

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

## Limitations: 

This study was limited by the data available for each CRB case.  It did not include any details specific to each complaint.  It only included demographic or geographical information. In addition, the data used for our analysis goes as far back as 2019. We believe these limitations have no impact on the outcome of our study. Future work should consider additional factors  specific to each complaint, beyond just demographic and geographic data.

## Solution Details:

Our analysis showed a number of things, including an increase in the number of complaints each year since 2019, with the number almost tripling from 2019 to 2022.  It also showed that the complaints are predominantly made by males, who are either black or hispanic.  This information is worthy of reporting clearly to the public in an easy to understand format, similar to the analysis we provided.  We also noted the complaints are largely related to procedure.  Publicly identifying this in easy to understand graphics would build trust in the information gap, highlighting transparency and opportunities to improve. In addition, we were able to show that predictive modeling tools can be used to predict CRB outcomes.  Our modeling results generated a high accuracy reporting toward predicting the likelihood of a complaint directed toward the police department being labeled as an act of misconduct. The majority of results from our conducted models generated accuracy scores within the 0.90 and recall scores of at least 0.60, which suggest that our models generalized well and they can predict CRB outcomes.  Our chosen model (SVM with linear kernel) also produced the most important features in predicting CRB outcomes. Our project has demonstrated the City of San Diego can  accurately report data related to CRB outcomes. This can be made publicly and bridge the gap between just providing data and interpretable information.


## Concluding Summary:

Our study met the defined objective of bridging the gap between the City of  San Diego’s effort to make CRB data publicly available, and the public’s ability to interpret the results.  We did this by showing visualizations on outcomes that can be easily generated, and informing the public on trends in CRB decisions. We also demonstrated that machine learning tools can be used to predict CRB outcomes. The model we built can be used to predict the likelihood a complaint of misconduct is affirmed and highlight the variables that contribute the most to predicting this CRB outcome.  These tools should be made more readily available for public consumption in an interpretable manner, improving transparency and accountability of both the SDPD and CRB.

## Call to Action (CTA):

Although our analysis provided valuable insights, several recommendations can be made for future work:
+  Incorporate additional data sources, including use of force records, crime data, and socioeconomic metrics to enable more advanced analyses of factors that may lead to misconduct.
+  Build interactive data visualizations and a public dashboard for residents to explore CRB data. This will keep residents up to date with CRB data.
+  Develop a smartphone app that enables residents to easily file complaints and track status through the review process. This will help the public gain trust that their voices are being heard.


