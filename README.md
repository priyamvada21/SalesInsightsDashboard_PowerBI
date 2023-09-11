# ATLIQ HARDWARE Sales Insights

Welcome to the ATLIQ HARDWARE Sales Insights project README. This project provides a comprehensive overview of the sales data for ATLIQ HARDWARE in India. I've created a powerful report and dashboard using Microsoft Power BI to analyze sales patterns throughout the years and months.

## Table of Contents

- [Project Description](#project-description)
- [Report Features](#report-features)
- [Tools Used](#tools-used)
- [Skills Required](#skills-required)
- [Queries](#queries)

## Project Description

ATLIQ HARDWARE is a major player in the Indian market, selling millions of products each year. To gain valuable insights into its sales and revenue, I've developed a robust Power BI-based report and dashboard. These tools allow me to track live sales data and analyze trends over time.

## Report Features

My report provides various key insights into ATLIQ HARDWARE's sales data:

1. **Revenue per Year:** Analyze annual revenue trends.
2. **Revenue per Month:** Understand how revenue fluctuates each month.
3. **Revenue per Customer:** Identify the top-performing customers.
4. **Revenue per Region:** Gain insights into sales performance across different regions.
5. **Top 5 Customers:** Discover the top five customers generating the most revenue.
6. **Top 5 Sales Quantities:** Identify the products with the highest sales quantities.
7. **Sales by Customer:** Analyze sales data for specific customers.
8. **Sales by City:** Examine sales data by city.
9. **Sales by Year:** Understand sales trends over different years.
10. **Sales by Month:** Explore sales patterns month by month.
11. **Overall Sales/Revenue:** Get a comprehensive overview of total sales and revenue.

## Tools Used

I utilized the following tools to develop this project:

1. **Microsoft Power BI Desktop:** Used to create interactive reports and dashboards.
2. **MYSQL Workbench:** For managing and querying the database.
3. **Microsoft Power BI Web Version:** To share and collaborate on reports online.

## Skills Required

To successfully complete this project, you need the following skills:

1. **Data Cleansing:** Ensuring data accuracy and quality.
2. **DAX Language:** Used for creating custom calculations and expressions in Power BI.
3. **Analytical Skills:** The ability to interpret data and draw meaningful insights.
4. **SQL Query Language:** For querying and retrieving data from the database.
5. **Business Intelligence Knowledge:** Understanding how to use data for informed business decisions.

## Queries

Here are some example queries that helped me verify the accuracy of my report and dashboard results:

1. Calculate the sum of total sales amount for the year 2020:

    ```sql
    SELECT SUM(transactions.sales_amount)
    FROM date
    INNER JOIN transactions ON date.date = transactions.order_date
    WHERE date.year = '2020'
    AND (transactions.currency = 'INR' OR transactions.currency = 'USD');
    ```

2. Check total sales in a specific region, such as Chennai:

    ```sql
    SELECT SUM(sales.transactions.sales_amount)
    FROM sales.markets
    INNER JOIN sales.transactions ON sales.markets.markets_code = sales.transactions.market_code
    WHERE sales.markets.markets_name = "Chennai";
    ```

Feel free to explore the report and dashboard to gain valuable insights into ATLIQ HARDWARE's sales performance. If you have any questions or need assistance, please don't hesitate to contact me.
