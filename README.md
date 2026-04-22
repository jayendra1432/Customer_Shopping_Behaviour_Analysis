# Customer_Shopping_Behaviour_Analysis
Data Analytics Project showcasing customer shopping behaviour analysis using Python, SQL and PowerBI.

Customer Shopping Behavior Analysis
📌 Project Overview
This project provides a comprehensive analysis of consumer shopping patterns to help businesses optimize marketing strategies and improve customer retention. Using a dataset of 3,900 records, I performed an end-to-end data pipeline—cleaning and transforming raw data in Python, performing complex relational queries in PostgreSQL, and building an interactive dashboard in Power BI.

The final phase involved generating a professional report and a PPT presentation using Gamma AI to communicate findings to stakeholders.

📊 Dataset
Source: shopping_behavior_updated.csv

Size: 3,900 rows, 16 initial features.

Key Attributes: Customer ID, Age, Gender, Purchase Amount, Category, Location, Review Rating, Subscription Status, and Frequency of Purchases.

🛠️ Tools & Technologies
Language: Python (Pandas, NumPy)

Database: PostgreSQL (SQLAlchemy for data migration)

Visualization: Power BI

Reporting: Gamma AI (PPT), Markdown (Report)

Environment: Jupyter Notebook / VS Code

⚙️ Project Steps
1. Data Cleaning & EDA (Python)
Handling Missing Values: Identified and filled missing Review Rating values using the median rating per category to maintain data integrity.

Standardization: Lowercased all column headers and replaced spaces with underscores for SQL compatibility.

Feature Engineering: * Segmented age into four groups: Young Adult, Adult, Middle Age, Senior.

Mapped categorical purchase frequencies (e.g., "Fortnightly") to numerical values (e.g., 14 days) for quantitative analysis.

Data Migration: Used SQLAlchemy to load the cleaned DataFrame directly into a PostgreSQL database.

2. Business Intelligence Queries (SQL)
Developed a series of SQL scripts to answer critical business questions, including:

Revenue Analysis: Calculating total revenue split by gender.

Customer Segmentation: Classifying users as New, Returning, or Loyal based on previous purchase history.

Product Performance: Identifying top-rated products and those with the highest discount-to-purchase ratios.

Behavioral Trends: Comparing the spending habits of subscribers vs. non-subscribers.

3. Dashboarding & Visualization (Power BI)
Built an interactive dashboard to visualize the SQL-derived insights:

KPI Cards: Total Revenue, Average Rating, and Total Customers.

Revenue by Age Group: A bar chart showing which demographic contributes most to the bottom line.

Category Drill-down: Analyzing the top 3 most purchased items per category.

4. Presentation (Gamma)
Synthesized findings into a professional slide deck using Gamma.

Focused on actionable insights: "Do repeat buyers actually subscribe?" and "Which products drive the highest engagement?"

📈 Key Results & Insights
Demographic Leads: The Middle Age group represents a significant portion of total revenue, suggesting a target for premium marketing.

Subscription Impact: Analysis revealed whether subscribed customers actually spend more on average compared to non-subscribers.

Loyalty Segment: Successfully segmented the customer base, identifying a "Loyal" group that can be targeted for exclusive rewards.

🚀 How to Run
Clone the Repository:

Bash
git clone https://github.com/yourusername/shopping-behavior-analysis.git
Environment Setup:

Ensure Python 3.x is installed.

Install dependencies: pip install pandas sqlalchemy psycopg2-binary.

Data Cleaning:

Run the customer_shopping_data cleaning.ipynb notebook to clean the data and export it to your local PostgreSQL instance.

Database Queries:

Import the pr 1.sql file into your SQL editor (pgAdmin/MySQL Workbench) and run the queries against the customer table.

Visualization:

Open the .pbix file in Power BI Desktop to view the interactive dashboard.
