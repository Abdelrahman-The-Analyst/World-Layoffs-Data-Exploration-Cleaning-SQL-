📌 Project Overview
This project involves a deep-dive analysis of global layoffs data spanning from the COVID-19 pandemic era to 2023. The goal was to clean a raw dataset and perform exploratory data analysis (EDA) to uncover trends, patterns, and insights regarding which industries and companies were most impacted.

🛠️ Tech Stack
Database: MySQL

SQL Concepts: - Data Cleaning (Removing Duplicates, Standardizing, Null Handling)

Common Table Expressions (CTEs)

Window Functions (DENSE_RANK, SUM OVER)

Aggregate Functions

Complex Joins & Filtering

🧼 Data Cleaning Highlights
Before analysis, the data underwent a rigorous cleaning process:

Duplicate Removal: Used ROW_NUMBER() to identify and delete duplicate entries.

Standardization: Fixed inconsistent naming in industries (e.g., merging "Crypto" variations) and trimmed whitespace.

Date Conversion: Converted text-based dates into proper DATE format for time-series analysis.

Null Management: Populated missing industry data by joining the table with itself based on company names.

📈 Key Insights (EDA)
The Giant Impact: Google recorded the highest single layoff event in 2023 with 12,000 employees.

Industry Vulnerability: The Consumer and Retail industries were hit hardest overall.

Time-Series Trend: Using a Rolling Total, I identified that layoffs accelerated significantly in early 2023 compared to previous years.

Geographic Hit: San Francisco (Bay Area) remained the epicenter of tech layoffs globally.

Yearly Winners/Losers: Utilized DENSE_RANK to filter the Top 5 companies with the most layoffs for each specific year.

🚀 How to Use
Clone the repository.

Import the layoffs.csv into your MySQL environment.

Run the cleaning.sql script first.

Execute the analysis.sql to see the insights.

📝 Conclusion
This project demonstrates the power of SQL in transforming messy, raw data into actionable business intelligence. It highlights the shift from Post-IPO stability to the volatility seen in the 2023 tech landscape.
