## 📊 TTOL Power BI Dashboard

This project presents an interactive Power BI dashboard developed to analyze customer activity, account balances, transactions, and demographics effectively.
The objective is to provide data-driven insights into user behavior, spending patterns, and inactive accounts, enabling stakeholders to make strategic decisions.

The dataset (~10,000+ records) was created and processed using MySQL and AI tools, with intentional inconsistencies included to practice data cleaning and transformation in Power Query Editor.
The dashboard highlights 10 KPIs across 2 pages (5 KPIs per page), focusing on transaction analysis, customer segmentation, and account trends.

📌 Steps Followed

Step 1: Collected and generated a synthetic dataset (~10,000 records) using MySQL and AI-generated queries.

Step 2: Designed the database schema and inserted sample records for multiple related tables.

Step 3: Cleaned and validated the data using SQL queries to handle nulls, formatting, and invalid entries.

Step 4: Combined datasets from three tables (e.g., Customers, Accounts, Transactions) using SQL joins.

Step 5: Imported the dataset into Power BI Desktop for modeling and visualization.

Step 6: Used Power Query Editor to handle data cleaning, remove duplicates, and correct inconsistent values.

Step 7: Built a 2-page dashboard with 10 KPIs distributed evenly across the pages.

Step 8: Created DAX measures to calculate total transactions, balances, customer counts, and averages.

Step 9: Designed interactive visualizations including bar charts, donut charts, line charts, cards, and tree maps.

Step 10: Added slicers and filters (by account type, time period, and demographics) for user-friendly navigation.

📌 KPIs & Visualizations
Page 1: Transaction Insights

Total Transactions by Type → Clustered Bar Chart

Monthly Transaction Trends → Line Chart

Top Customers by Transaction Volume → Table / Bar Chart

Total Balance by Account Type → Donut Chart

Inactive Accounts Over Time → Stacked Column Chart

Page 2: Customer Insights

Customer Count by Gender → Clustered Column Chart

Age Group Distribution → Pie Chart

Transactions by Age Group → Tree Map

Average Balance per Customer → KPI Card

Total Active Customers → KPI Card

📌 Sample DAX Measures
-- Total Customers
Total Customers = COUNT(Customer[CustomerID])

-- Total Transactions
Total Transactions = COUNT(Transactions[TransactionID])

-- Total Balance
Total Balance = SUM(Accounts[Balance])

-- Average Balance
Average Balance = AVERAGE(Accounts[Balance])

-- Monthly Transactions
Monthly Transactions = COUNTROWS(Transactions)

📸 Dashboard Snapshot
![Dashboard Page 1](assets/dashboard-page1.png)




(Place your Power BI screenshots inside an assets/ folder and update the image paths above.)

📌 Key Insights

📈 Transaction Patterns – Shows overall transaction distribution and trends.

🏦 Account Analysis – Tracks balances and highlights inactive accounts.

👥 Customer Demographics – Segments customers by gender and age groups.

🏆 Top Customers – Identifies highest-value customers by transaction volume.

🛠️ Tools & Technologies Used
Tool / Technology	Purpose
Power BI	Dashboard creation & visualization
MySQL	Dataset creation & data preparation
Power Query	Data cleaning & transformation
DAX	KPI calculations & metrics
📧 Contact

Jadhav Akshay Kumar
🎓 B.Tech, Electronics & Communication Engineering
📍 IIT(ISM) Dhanbad
