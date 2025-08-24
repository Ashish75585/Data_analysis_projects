# Sales Data Insight - A Power BI Project

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

Welcome to the repository for my "Sales Data Insight" project. This project involves the analysis of sales data to uncover trends, track key performance indicators (KPIs), and provide actionable insights through an interactive Power BI dashboard.

## 📊 Dashboard Preview

![Sales Dashboard Screenshot](./Images/dashboard_preview.png)

*[**Note:** To make the image above appear, create a folder named "Images" in your repository and upload a screenshot of your dashboard named "dashboard_preview.png".]*

---

## 📝 Project Overview

This project aims to solve the common business problem of having vast amounts of sales data with no easy way to interpret it. The interactive dashboard centralizes key metrics and provides a user-friendly interface for stakeholders to explore sales performance across different dimensions like region, product, and time.

### 🎯 Key Objectives
- To develop a comprehensive sales report to monitor KPIs like Total Revenue, Profit Margin, and Sales Growth.
- To identify top-performing products, regions, and sales representatives.
- To analyze sales trends on a monthly, quarterly, and yearly basis.
- To provide a dynamic and interactive dashboard for data-driven decision-making.

---

## Dataset

The dataset used for this analysis is a [e.g., fictional retail sales dataset, public sales dataset from Kaggle, etc.]. It contains transactional data including information on:
- **Order Details:** Order ID, Order Date, Ship Date.
- **Product Details:** Product Name, Category, Sub-Category.
- **Customer & Location:** Customer Name, City, State, Country/Region.
- **Sales Figures:** Sales, Quantity, Discount, Profit.

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI:** The primary tool for data modeling, analysis, and visualization.
- **Power Query:** Used for Extracting, Transforming, and Loading (ETL) the data.
- **DAX (Data Analysis Expressions):** Used for creating complex calculations and custom measures.

---

## 🔄 Project Workflow (ETL Process)

1.  **Data Extraction:** Connected to the source data from [e.g., an Excel file, a CSV file, a SQL database].
2.  **Data Transformation & Cleaning (Power Query):**
    - Handled missing values and removed duplicates.
    - Corrected data types for columns (e.g., converting text to date).
    - Created conditional columns to segment data [e.g., created a 'Profitability Status' column based on profit].
    - Merged/Appended queries as needed [mention if you did this].
3.  **Data Modeling:**
    - Designed a **Star Schema** with one fact table (Sales) and multiple dimension tables (Date, Product, Customer).
    - Established relationships between tables based on primary and foreign keys.
    - Optimized the data model for performance.
4.  **DAX Calculations:**
    - Created over [e.g., 20+] DAX measures to calculate key business metrics.
    - Implemented Time Intelligence functions to analyze Year-over-Year (YoY) Growth and Year-to-Date (YTD) Sales.
    - Example of a key measure:
      ```dax
      YoY Revenue Growth % = 
      VAR CurrentYearRevenue = [Total Revenue]
      VAR PreviousYearRevenue = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('Date'[Date]))
      RETURN
      DIVIDE(CurrentYearRevenue - PreviousYearRevenue, PreviousYearRevenue)
      ```
5.  **Report & Visualization:**
    - Designed an intuitive and visually appealing multi-page report.
    - Used a variety of visuals (bar charts, line charts, maps, cards, slicers) to represent the data effectively.
    - Implemented interactive features like drill-throughs, bookmarks, and tooltips for an enhanced user experience.

---

## 📈 Key Insights & Findings

- **Top Performing Region:** The [e.g., West] region consistently generated the highest revenue, contributing to over [e.g., 35%] of total sales.
- **Most Profitable Product Category:** The [e.g., Technology] category, despite having fewer sales in quantity, yielded the highest profit margin.
- **Seasonal Trends:** A significant spike in sales was observed during [e.g., Q4], likely due to holiday promotions.
- **Impact of Discounts:** Analysis showed that discounts above [e.g., 20%] had a negative impact on profitability for certain sub-categories.

---

## 🚀 How to Use This Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)[YourUsername]/[YourRepoName].git
    ```
2.  **Download the `.pbix` file:**
    - The main Power BI file is `Sales Data Insight.pbix`.
3.  **Open in Power BI Desktop:**
    - You will need Microsoft Power BI Desktop installed on your machine.
    - Open the `.pbix` file to view the report, data model, and DAX calculations.

*[Optional: If you published your report to the web]*
You can also view and interact with the live dashboard here: [Link to your published Power BI report]

---

## 🔗 Connect with Me

- **Author:** [Your Name]
- **LinkedIn:** [Your LinkedIn Profile URL]

Feel free to reach out if you have any questions or would like to collaborate on future projects!
