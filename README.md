# Banking-Analysis-Power-Bi-Dashboard
This project showcases a comprehensive Banking Analysis Dashboard created in Power BI, designed to analyze client financial behavior, deposits, loans, relationships, and advisor performance across multiple dimensions like gender, year, and account type.

# Overview:
The dashboard provides a clear and interactive interface for stakeholders to explore key banking metrics. By leveraging dynamic visuals, filters, and slicers, it allows decision-makers to uncover trends, compare segments, and monitor performance KPIs effectively.

# Dataset Details:
The analysis is powered by multiple structured .csv files:

File Name	Description
banking-clients.csv    ----    Client information and demographics.

banking-realationships.csv    ----    Type of banking relationships (Retail, Institutional, etc.)

gender.csv    ----    Gender categorization for segmentation.

investment-advisors.csv    ----    Assigned investment advisors per client.

# Dashboard Pages & Features:
Home Page --
* Year & Gender slicers for interactive filtering
* KPIs:
      Total Clients: 3000
      Total Deposit: 3.77bn
      Total Loan: 4.38bn
      Business Lending, Checking, and Savings Breakdown

Loan Analysis Page --
* Segmentation by:
      Banking Relationship
      Gender
      Advisor
* KPIs:
      Bank Loan, Credit Card Balance, Business Lending
* Visuals:
      Loan by Branch, Occupation, Nationality, Income Band

Deposit Analysis Page --
* KPIs:
      Total Deposit, Checking & Savings Amounts
* Visuals:
      Deposit by Branch, Occupation, Nationality, Income Band

Summary Page --
* Net Balance Calculation (Deposit - Loan)
* Deposit vs Loan by Year
* Savings by Continent
* Deposit by Gender and Relationship
* Top 10 income bands by Net Balance

# Key Insights:
📈 High-Income groups dominate both loans and deposits.

🏦 Private and Retail Banking show the largest deposit volumes.

📉 Net Balance trends vary sharply year over year, showing fluctuations in savings vs lending.

🧑‍💼 Occupation plays a major role in financial behavior (loan/deposit).

🔧# Tools & Technologies:

Tool	Purpose

Power BI	Data modeling, visualization

Power Query	Data transformation

DAX	Measures & KPIs

CSV Files	Data Source

# Sample DAX Measures:
Net Balance = SUM('Deposit') - SUM('Loan')

Total Customers = DISTINCTCOUNT(ClientID)

Deposit vs Loan % = 
DIVIDE(SUM('Loan'), SUM('Deposit'), 0)

Avg Savings = AVERAGE('SavingsAccount')



