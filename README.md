# Smartphone-Analysis
Smartphone Analysis using Python and Web Scraping
📱 Smartphone Market Analysis Using Web Scraping
📌 Project Overview

Smartphones have become an important part of everyday life, and the smartphone market contains a wide range of brands, prices, specifications, discounts, and customer ratings.

This project focuses on analyzing smartphone market data collected from Flipkart using web scraping techniques.

The main purpose of this project is to understand smartphone pricing patterns, brand-wise differences, discounts, ratings, RAM, storage, battery capacity, and other important specifications.

Python is used for web scraping, data cleaning, data preprocessing, exploratory data analysis, visualization, and correlation analysis.
💼 Business Statement

The objective of this project is to analyze smartphone market data scraped from Flipkart in order to understand:

Brand-wise smartphone pricing
Smartphone discounts
Customer ratings
RAM and storage specifications
Battery capacity
Relationship between specifications and price
Market trends and useful patterns

The analysis can help understand product positioning and pricing patterns in the smartphone market.

🎯 Project Objectives

The main objectives of this project are:

Scrape smartphone data from Flipkart.
Collect smartphone information from multiple pages.
Extract important smartphone specifications.
Clean and transform the collected data.
Handle missing values.
Identify and remove duplicate records.
Perform Exploratory Data Analysis (EDA).
Analyze smartphone prices across different brands.
Study the relationship between RAM, storage, battery and price.
Analyze discounts and customer ratings.
Perform correlation analysis.
Generate useful business insights.

🛠️ Technologies Used

The following tools and Python libraries were used:

Python
Requests
BeautifulSoup
Regular Expressions (Regex)
Pandas
NumPy
Matplotlib
Jupyter Notebook
🌐 Data Collection – Web Scraping

Smartphone information was collected from Flipkart using Python web scraping techniques.

The Requests library was used to send requests to Flipkart pages and retrieve the HTML content.

BeautifulSoup was used to parse the HTML content and identify the required product information.

Regular Expressions were used to extract specific information such as RAM, storage, battery capacity, and camera details.

The project scraped data from 10 pages and initially collected 240 smartphone products.

📋 Data Collected

The following information was extracted from the smartphone listings:

Column	Description
Brand	Smartphone brand
Name	Smartphone name
Color	Smartphone color
RAM	RAM capacity in GB
Storage	Storage capacity in GB
Battery(mAh)	Battery capacity
Camera	Camera information
Price(in Rs)	Current selling price
Original Price(in Rs)	Original/MRP price
Discount	Discount percentage
Rating	Customer rating

These fields were created while extracting the smartphone details from the scraped product information.

🔄 Project Workflow

The overall project workflow is:

Flipkart → Web Scraping → Data Collection → DataFrame → Data Cleaning → Missing Value Handling → Duplicate Removal → EDA → Visualization → Correlation Analysis → Business Insights

🧹 Data Cleaning & Preprocessing

After collecting the raw data, data cleaning was performed to make the dataset suitable for analysis.

Cleaning steps:
Removed unwanted symbols such as ₹.
Removed commas from price values.
Removed units such as GB and mAh where required.
Converted relevant columns from text into numeric data types.
Checked missing values.
Filled missing values using appropriate statistical methods.
Calculated missing discount values using original price and selling price.
Checked duplicate records.
Removed duplicate records.
Missing Value Handling

Different methods were used depending on the column.

For example:

Mode was used for Brand.
Median was used for RAM, Storage and Battery.
Mean was used for Price and Rating.
Missing Discount values were calculated from Original Price and Price where possible.

🔁 Duplicate Record Handling

The dataset initially contained duplicate records.

The duplicate check identified 52 duplicate records.

After removing duplicates, the dataset was reduced from 240 records to 188 records with 11 columns.

📊 Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand different patterns in the smartphone market.

1. Brand-wise Pricing

The average smartphone price was calculated for each brand.

This analysis helps compare the average price levels of different smartphone brands.

For example, the calculated results show differences in average pricing between brands such as Apple, Google, IQOO, vivo, OnePlus, Samsung, realme, and others.

2. RAM vs Price

The relationship between RAM capacity and smartphone price was analyzed.

Average price was calculated for different RAM categories.

The analysis shows that smartphones with higher RAM capacities generally have higher average prices in this dataset.

A scatter plot was also created to visualize the relationship between RAM and price.

3. Storage vs Price

Storage capacity was compared with the average smartphone price.

The analysis considered storage categories such as:

64 GB
128 GB
256 GB
512 GB

The average price increased across these storage categories in the analyzed dataset.

4. Brand-wise Battery Analysis

Average battery capacity was calculated for different smartphone brands.

This analysis helps compare battery capacities across brands and understand differences in battery specifications.

A bar chart was created to visualize brand-wise average battery capacity.

5. Discount Analysis

Discount percentages were analyzed across different smartphone brands.

The average discount was calculated for each brand to understand discount patterns in the collected listings.

6. Rating Analysis

Average customer ratings were calculated for different smartphone brands.

This analysis helps understand rating patterns across the brands included in the dataset.

7. Price Distribution

A histogram was created to understand how smartphone prices are distributed in the dataset.

This helps identify the concentration of smartphones across different price ranges.

8. Rating Distribution

A KDE plot was created to understand the distribution of smartphone ratings.

Mean and median ratings were also visualized on the distribution.

9. Battery vs Price

A scatter plot was created to analyze the relationship between battery capacity and smartphone price.

This helps understand whether smartphones with larger battery capacities tend to have different price levels.

10. Rating vs Price

The relationship between smartphone rating and price was analyzed using a scatter plot.

This helps understand how ratings are distributed across different price levels.

🔗 Correlation Analysis

Correlation analysis was performed using the following numerical variables:

Price
Discount
Rating
RAM
Storage
Battery

A correlation matrix and heatmap were created to understand the relationships between these variables.

The calculated correlation values show:

Price and Rating: 0.607
Price and RAM: 0.573
Price and Storage: 0.517
Price and Battery: 0.339
RAM and Storage: 0.795

These values describe the relationships observed within this particular dataset.

📈 Key Insights

Based on the analysis, the project provides insights into:

Differences in average smartphone prices across brands.
Higher RAM categories having higher average prices in the dataset.
Higher storage categories having higher average prices in the dataset.
Differences in battery capacity across brands.
Different discount patterns among brands.
Rating patterns across smartphone brands.
Distribution of smartphone prices and ratings.
Relationships between price and other numerical specifications.
Strong relationship between RAM and Storage in the analyzed dataset.

📂 Dataset

The cleaned dataset was saved as:

Smartphone-Market-Analysis.csv

The final dataset contains 188 rows and 11 columns after duplicate removal.

📁 Project Files

This GitHub repository contains the main files related to the project:

Python / Jupyter Project File – Web scraping, cleaning and analysis code.
HTML File – Related to the web scraping/data collection process.
CSV File – Scraped and processed smartphone dataset.
README.md – Project documentation.

🚧 Challenges Faced

During the project, some challenges were involved in:

Collecting data from web pages.
Extracting required information from HTML.
Handling missing values.
Cleaning currency and percentage values.
Converting text values into numeric values.
Identifying duplicate records.
Extracting specifications using Regular Expressions.

🚀 Future Enhancements

This project can be further improved by:

Adding data from other e-commerce websites.
Comparing smartphone prices across multiple platforms.
Performing customer review sentiment analysis.
Building an interactive dashboard using Power BI.
Automating the data collection and analysis process.
Adding more advanced statistical or machine learning analysis.

🏁 Conclusion

The Smartphone Market Analysis Using Web Scraping project demonstrates an end-to-end data analysis workflow.

The project starts with collecting real-world smartphone data through web scraping and continues with data cleaning, preprocessing, exploratory analysis, visualization, and correlation analysis.

This project provided practical experience in Python, Web Scraping, Pandas, NumPy, BeautifulSoup, Regular Expressions, Matplotlib, and Data Analysis.

It also helped in understanding how raw web data can be transformed into meaningful information and business insights.
