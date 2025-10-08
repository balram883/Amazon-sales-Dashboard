# Amazon-sales-Dashboard
📊 Amazon Product Data Analysis — Power BI Dashboard
📁 Project Overview

This Power BI project analyzes Amazon product data to uncover insights related to pricing, ratings, and customer preferences. The dashboard provides an interactive and visual representation of product performance, enabling data-driven decisions for e-commerce growth and product optimization.

The dataset used in this project is Amazon_Combined_Data.xlsx, which contains details such as product names, categories, prices, ratings, and reviews.

🧠 Key Objectives

Understand product distribution across categories

Analyze pricing trends and identify outliers

Explore the relationship between product ratings and pricing

Compare top-performing and underperforming products

Build custom Power BI measures for deeper insights

⚙️ Features and Components
1. Data Processing

Cleaned and formatted Amazon product data

Handled missing values and inconsistent entries

Created calculated columns for better grouping and categorization

2. DAX Measures Used

Custom Power BI measures were created to enhance insights, including:

Average Rating = AVERAGE('Data'[Rating])

Total Products = COUNTROWS('Data')

Average Price = AVERAGE('Data'[Price])

Top Rated % = DIVIDE(CALCULATE(COUNTROWS('Data'), 'Data'[Rating] >= 4.5), [Total Products])

Total Reviews = SUM('Data'[Review Count])

Revenue Estimate = SUMX('Data', 'Data'[Price] * 'Data'[Review Count])


📈 Dashboard Insights

The Power BI report provides multiple pages and visuals, such as:

Category-wise product distribution

Price vs. Rating scatter analysis

Top 10 products by rating and review count

Monthly sales trend visualization (if applicable)

Dynamic slicers for filtering by category, price range, or rating

🖥️ Tools and Technologies

Power BI Desktop (for data modelling and dashboard creation)

Excel (.xlsx) for data storage

DAX (Data Analysis Expressions) for measures and KPIs

🚀 How to Use

Download the .pbix file (Amazon Product Data.pbix).

Open it in Power BI Desktop.

Load or refresh the dataset (Amazon_Combined_Data.xlsx) if prompted.

Interact with visuals using filters and slicers for detailed insights.

📊 Key Takeaways

Visual storytelling helps understand Amazon product trends efficiently.

DAX measures make it possible to calculate KPIs dynamically.

Interactive dashboards simplify comparative and performance analysis.

👨‍💻 Author

Balram Singh Thakur
Data Analyst | Power BI | SQL | Python | Excel

🏞️ Screenshot
![Dashboard Overview](https://github.com/balram883/Amazon-sales-Dashboard/blob/main/Dashboard.png)
