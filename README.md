## 📊Toll Collection Analysis Dashboard

This project presents an interactive Power BI dashboard developed to analyze customer activity, account balances, transactions, and demographics effectively.
The objective is to provide data-driven insights into user behavior, spending patterns, and inactive accounts, enabling stakeholders to make strategic decisions.

The dataset (~10,000+ records) was created and processed using MySQL and AI tools, with intentional inconsistencies included to practice data cleaning and transformation in Power Query Editor.
The dashboard highlights 10 KPIs across 2 pages (5 KPIs per page), focusing on transaction analysis, customer segmentation, and account trends.
This Power BI dashboard provides an in-depth analysis of toll collection activities across different locations in Madhya Pradesh.
It highlights transaction patterns, revenue generation, vehicle distribution, and traffic flow using visualizations, KPIs, and interactive slicers.

The dataset (~10,000+ records) was sourced from Madhya Pradesh Toll Collection Data and cleaned using Power Query Editor.
The dashboard highlights 10 KPIs across 3 pages (5 KPIs each), enabling authorities to monitor toll revenue, vehicle categories, and traffic trends effectively.

Through this dashboard, authorities can:

Track toll revenue collections over time.

Analyze traffic distribution across toll plazas.

Monitor vehicle type-wise toll contributions.

Identify high-revenue and low-revenue locations.

Optimize toll operations using data-driven insights.

### 📌 Steps Followed

Step 1: Collected toll collection dataset from Madhya Pradesh dataset (~10,000+ records).

Step 2: Performed data cleaning using Power Query Editor (null removal, date formatting, duplicate handling).

Step 3: Transformed columns and created calculated fields for KPIs.

Step 4: Designed a 2-page Power BI Dashboard with interactive visuals.

Step 5: Created DAX measures for KPIs (e.g., Total Toll Collected, Average Toll Per Vehicle, Vehicle Count).

Step 6: Added slicers for filtering by plaza, vehicle type, and date range.

Step 7: Applied conditional formatting and designed visuals for better storytelling.

### 📌 KPIs & Visualizations

Total Toll Collected by Month 

Toll Revenue by Plaza 

Top 5 High-Revenue Locations 

Vehicle Type-wise Toll Collection 

Revenue Trends Over Time 

Total Vehicle Count by Plaza 

Vehicle Distribution by Type 

Average Toll Per Vehicle 

Peak Traffic Hours 
Low Revenue vs High Revenue Plazas

### 📌 Sample DAX Measures
-- Total Toll Collected
Total Toll = SUM(TollData[TollAmount])

-- Total Vehicle Count
Total Vehicles = COUNT(TollData[VehicleID])

-- Average Toll Per Vehicle
Average Toll = DIVIDE([Total Toll], [Total Vehicles])

-- Monthly Toll Collection
Monthly Toll = CALCULATE(SUM(TollData[TollAmount]), ALLEXCEPT(TollData, TollData[Month]))

-- Top 5 Locations by Revenue
Top Locations = TOPN(5, SUMMARIZE(TollData, TollData[Plaza], "Revenue", SUM(TollData[TollAmount])), [Revenue], DESC)


### 📸 Dashboard Snapshot
![Dashboard Page 1](https://github.com/Akshayjadhav04/Toll-Gate-Dashboard/blob/dbfe21ee78a9721670bd9d01c3192a9fae2b34a4/ttol-1.png)

![Dashboard Page 1](https://github.com/Akshayjadhav04/Toll-Gate-Dashboard/blob/a8a92f137a748385ae241acf25cda5ee2dfb12a4/ttol-2.png)

![Dashboard Page 1](https://github.com/Akshayjadhav04/Toll-Gate-Dashboard/blob/dbfe21ee78a9721670bd9d01c3192a9fae2b34a4/ttol-3.png)


(Place your Power BI screenshots inside an assets/ folder and update the image paths above.)

### 📌 Key Insights

From the Toll Collection Dashboard, the following insights can be drawn:

[1] Revenue Patterns

Highest revenue is generated in peak festive months.

Some toll plazas contribute 70%+ of the total revenue.

[2] Traffic Insights

Heavy vehicles contribute the highest toll amount despite fewer counts.

Small vehicles dominate overall traffic but contribute lesser revenue.

[3] Location-Wise Analysis

Top-performing plazas contribute significantly more than low-performing ones.

Certain locations require policy intervention to improve toll collection efficiency.

[4] Optimization Opportunities

Traffic flow and toll rates can be optimized based on vehicle category and peak timings.

#### 🛠️ Tools & Technologies Used
Tool / Technology	Purpose
Power BI	Dashboard creation & visualization
Power Query	Data cleaning & transformation
DAX	KPI calculations & metrics

### 📧 Contact

## 👨‍💻 Author
**Jadhav Akshay Kumar**  
🎓 B.Tech – Electronics & Communication Engineering, IIT (ISM) Dhanbad  
🌐 Connect with me:  
🔗 [![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/jadhav-akshay-kumar-835b22289/)  
💻 [![GitHub](https://img.shields.io/badge/GitHub-black?style=flat&logo=github)](https://github.com/Akshayjadhav04)

