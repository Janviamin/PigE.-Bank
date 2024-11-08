# ATM Transaction Monitoring for Suspicious Cross-Border Activity
## Project Overview
This project aims to detect suspicious cross-border ATM transaction activity that could be related to money laundering by Mexican drug cartels. The model we are developing will identify unusual transaction patterns in ATM deposits near the US-Mexico border and corresponding withdrawals in Mexico. Alerts generated by the model will be routed to Pig E. Bank’s Investigations Department for further analysis.

## Data Collection
The dataset includes:  

ATM deposits made in US Dollars within 100 miles of the US-Mexico border.  
Subsequent ATM withdrawals in Mexico.  
Variables such as transaction amount, time between deposits and withdrawals, and customer demographics.  
Note: Some of the historical ATM transaction data was pre-cleaned in a previous project, allowing us to focus on model development and testing.  

## Model Training
To train the model, we need to distinguish normal from suspicious transaction activity. The Investigations Department provided 10 analysts, each scoring 1,000 instances as "positive" (suspicious) or "negative" (normal). This human input will help train the model to identify characteristics common in both types of activity.

## Analyst Results
The total score of suspicious transactions (positives) from the test set was 3,066 out of 10,000 transactions. Individual analyst scores are shown in the bar graph below, indicating variability in suspicious transaction identification, which will guide further model iteration.

## Requirements 
To reproduce this project:  

Python (for data analysis and model development)  
SQL knowledge for data querying  
Data visualization libraries (e.g., Matplotlib, Seaborn)  
Basic machine learning knowledge  
## Project Structure
data/: Contains ATM transaction data used in the project.  
scripts/: Includes Python scripts for querying data, cleaning, and initial analysis.  
notebooks/: Jupyter notebooks for data exploration and visualization.  
results/: Final analysis results, including graphs and tables.   
README.md: Project description, methodology, and instructions for replicating the study.  
