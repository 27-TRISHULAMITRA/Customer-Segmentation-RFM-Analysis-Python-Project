# customer-rfm-Data Analysis-python

# Project Overview

This data analytics project focused on customer behavior analysis using Python, Pandas, NumPy, and Matplotlib. The project was completed as part of a customer data analysis assessment based on retail transaction data. The main objective was to clean, process, analyze, and visualize customer data to generate meaningful business insights.
# The analysis includes:

Data cleaning and preprocessing
Customer transaction analysis
RFM (Recency, Frequency, Monetary) analysis
Customer segmentation
Data visualization
Pareto analysis
The project uses synthetic retail customer data containing:
1,000 unique customers
23,050 transaction records
The original project requirements included customer segmentation, identification of high-value customers, and business insight generation through visual analytics. �
project questions.pdf.pdf
Project Objectives
Analyze customer demographics and purchasing behavior
Clean and validate customer datasets
Perform RFM analysis for customer segmentation
Identify valuable and inactive customers
Generate business-focused insights
Visualize customer segments and revenue contribution
Technologies Used
Python
Pandas
NumPy
Matplotlib
Jupyter Notebook
Dataset Information
Customer Master Dataset
Contains customer demographic information such as:
CustomerID
Name
Email
Gender
Age
City
MaritalStatus
NumChildren
JoinDate
Transaction Dataset
Contains transaction-level information such as:
CustomerID
TransactionDate
TransactionAmount
The datasets were merged using CustomerID for customer-level analysis. �
project_report.pdf.pdf
Key Steps Performed
1. Data Loading
Imported both datasets using Pandas
Checked shape, structure, and data types
Validated dataset consistency
2. Data Cleaning
Converted date columns into datetime format
Checked missing values
Removed null values
Validated unique CustomerIDs
Verified transaction records matched customer records
The project confirmed that all 23,050 transaction records contained valid customer references. �
project_report.pdf.pdf
3. RFM Analysis
Calculated:
Recency → Days since last purchase
Frequency → Total number of transactions
Monetary → Total customer spending
RFM scores were assigned using quantile-based scoring.
4. Customer Segmentation
Customers were segmented into groups such as:
Champions
Big Spenders
Frequent Customers
Recent Customers
Lost Customers
Others
The project identified that only 35 customers belonged to the Champion segment, making them the most valuable customers. �
project_report.pdf.pdf
5. Data Visualization
Created visualizations including:
Customer segment distribution
Revenue contribution by segment
Recency vs Monetary scatter plot
Pareto analysis
Key Business Insights
Big Spenders
The “Big Spender” segment contributed approximately 22.3% of total revenue despite representing a relatively small customer group. �
project_report.pdf.pdf
Champion Customers
Champion customers showed:
High transaction frequency
Recent purchases
High monetary value
These customers represent the most loyal and profitable customer segment. �
project_report.pdf.pdf
Pareto Analysis Insight
The dataset did not follow the traditional 80/20 Pareto principle. Instead, revenue was distributed more evenly across customers, indicating the business depends on a broader customer base rather than a small set of high-value customers. �
project_report.pdf.pdf
Repository Structure
Bash
├── Customer Data Analysis for Business Insights.ipynb
├── Customer_Master_Data.csv
├── Customer_Transactions.csv
├── project_report.pdf
├── README.md
How to Run the Project
Clone the repository
Open the Jupyter Notebook
Install required libraries:
Bash
pip install pandas numpy matplotlib
Run the notebook cells step by step
Project Outcome
This project demonstrates practical skills in:
Data cleaning
Exploratory Data Analysis (EDA)
Customer segmentation
RFM analysis
Business insight generation
Data visualization using Python
Author
Solo Project by Trishula
Dataset Link Section (Add This to GitHub)
Create a section like this in your README so users can access the dataset files easily:
Markdown
## Dataset Files

Click below to access the datasets used in this project:

- [Customer Master Dataset](./Customer_Master_Data.csv)
- [Customer Transactions Dataset](./Customer_Transactions.csv)
- [Project Notebook](./Customer%20Data%20Analysis%20for%20Business%20Insights.ipynb)
- [Project Report](./project_report.pdf)
After uploading all files to your GitHub repository, these links will automatically become clickable.

📁 Dataset

Click Here
