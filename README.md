# 📊 Customer Behavior & Analytics
Project Overview
This project is an end-to-end data analysis solution designed to decode the shopping behavior of 3,900 customers. Using a hybrid approach of Python for data engineering and SQL for analytical querying, I transformed raw transactional data into strategic business insights regarding customer loyalty, subscription propensity, and revenue drivers.

# 🛠️ Technical Workflow
1.Data Engineering & Preprocessing (Python)
Before analysis, I used Pandas to ensure the dataset was "analysis-ready":

- Data Cleaning: Handled missing values in the Review Rating column by imputing the median rating specific to each product category.
- Feature Engineering: * Created an age_group segment (Young Adult, Adult, Middle-aged, Senior) using quartile binning. Mapped categorical purchase frequencies into numerical purchase_frequency_days for quantitative modeling*.
- Database Integration: Built a localized data pipeline using SQLAlchemy and PyMySQL to programmatically load the processed data into a MySQL database named Customer_Behaviour.
2. Advanced Analytical Querying (SQL)
With the cleaned data in MySQL, I executed 10 high-impact business queries to extract behavioral insights:

- Segmentation: Used CTEs and Case Statements to categorize the 3,900 customers into New, Returning, and Loyal tiers based on historical purchase counts.
- Product Performance: Applied Window Functions (ROW_NUMBER()) to rank the top 3 products in every category by order volume.
- Financial Analysis: Compared spending habits between subscribers and non-subscribers and calculated revenue contribution by gender and age group.
- Discount Efficiency: Developed a query to identify products with the highest "discount-to-purchase" ratio to measure promotional impact.
# 📈 Key Insights Found
- Loyalty Distribution: Automated the count of customers across loyalty segments to identify the size of the "Loyal" base.
- Subscription Value: Compared the average spend (avgspend) and total revenue between subscribed and non-subscribed members.
- Shipping Impact: Analyzed if "Express Shipping" users showed significantly different spending patterns than "Standard Shipping" users.
# 🎯 Outcome
This project highlights a full-stack data proficiency:

- Data Engineering: Automating cleaning and feature creation.
- Analytical Thinking: Translating raw data into segmented customer tiers.
- Visualization: Creating "At-a-glance" intelligence for executive leadership.
# 📂 Project Structure
- Customer_Shopping_Behaviour_Analysis.ipynb: Python notebook for cleaning, feature engineering, and DB loading.
- customer_behaviour_project_SQL.sql: The full analytical suite of 10 SQL business queries.
- customer_shopping_behavior.csv: The core dataset containing 3,900 customer records.
