# Walmart_Sales_Data_Analysis


### **Project Overview**

This project analyzes Walmart’s sales data to uncover insights into store performance, product popularity, sales trends, and customer purchasing behavior. The primary objective is to identify the key factors that influence overall sales performance and develop data-driven strategies to enhance business outcomes.

The dataset, sourced from a Kaggle competition, includes historical sales data from multiple Walmart branches across different cities. Each store contains several departments, and the analysis particularly focuses on understanding how holiday markdown events influence sales patterns and customer buying behavior.

---

### **Project Objectives**

This project aims to:

* Determine the top-performing stores and departments.
* Identify seasonal trends and product-wise sales patterns.
* Evaluate the impact of promotions and holiday markdowns.
* Analyze customer behavior, preferences, and profitability.
* Generate actionable recommendations to optimize future sales.

---

### **About the Dataset**

The dataset originates from the **Kaggle Walmart Sales Forecasting Competition** and contains records from three Walmart branches located in **Mandalay, Yangon, and Naypyitaw**.

Dataset Overview:
* Rows: 1000
* Columns: 17

 | Column |	Description|	Data Type|
| :-------:|:---------:|:----------|
|invoice_id |	Invoice of the sales made	|VARCHAR(30)|
|branch	|Branch at which sales were made	|VARCHAR(5)|
|city	|The location of the branch|	VARCHAR(30)|
|customer_type	|The type of the customer|	VARCHAR(30)|
|gender	|Gender of the customer making purchase	|VARCHAR(10)|
|product_line	|Product line of the product solf	|VARCHAR(100)|
|unit_price|	The price of each product	|DECIMAL(10, 2)|
|quantity	|The amount of the product sold	|INT|
|VAT	|The amount of tax on the purchase	|FLOAT(6, 4)|
|total|	The total cost of the purchase	|DECIMAL(10, 2)|
|date|	The date on which the purchase was made|	DATE|
|time	|The time at which the purchase was made	|TIMESTAMP|
|payment_method	|The total amount paid	|DECIMAL(10, 2)|
|cogs	|Cost Of Goods sold	|DECIMAL(10, 2)|
|gross_margin_percentage|	Gross margin percentage	|FLOAT(11, 9)|
|gross_income|	Gross Income|	DECIMAL(10, 2)|
|rating	|Rating	|FLOAT(2, 1)|
---

### **Analysis Approach**

#### **1. Data Wrangling**

* Checked and handled missing values.
* Created and populated structured database tables.
* Applied NOT NULL constraints to preserve data integrity.

#### **2. Feature Engineering**

New attributes were created to support deeper insights:

* **time_of_day:** Segmented sales into Morning, Afternoon, and Evening.
* **day_name:** Extracted weekday names to analyze peak shopping days.
* **month_name:** Extracted month names to study monthly sales trends.

#### **3. Exploratory Data Analysis (EDA)**

Conducted EDA to answer key business questions related to product performance, customer behavior, and revenue trends.

---

### **Business Questions Addressed**

#### **A. General**

* Number of unique cities
* In which city is each branch located?

#### **B. Product Analysis**

* How many unique product lines exist?
* What is the most common payment method?
* What is the best-selling product line?
* What is the total revenue by month?
* Which month had the largest COGS?
* Which product line had the highest revenue?
* Which city generated the highest revenue?
* Which product line had the largest VAT?
* Fetch each product line and add a column labeled “Good” or “Bad” based on whether its sales exceed the average.
* Which branch sold more products than the average quantity sold?
* What is the most common product line by gender?
* What is the average rating of each product line?

#### **C. Sales Analysis**

* Number of sales made during each time of the day per weekday.
* Which customer type generates the most revenue?
* Which city has the highest VAT percentage?
* Which customer type pays the most VAT?


#### **D. Customer Analysis**

* How many unique customer types exist?
* How many unique payment methods exist?
* What is the most common customer type?
* Which customer type buys the most?
* What is the gender of most customers?
* What is the gender distribution per branch?
* During which time of the day do customers give the most ratings?
* Which time of the day receives the highest ratings per branch?
* Which day of the week has the best average ratings?
* Which day of the week has the best average ratings per branch?

---

### **Conclusion**

This analysis delivers valuable insights into Walmart’s store and product performance, customer demographics, and seasonal sales patterns. The findings can be leveraged to:

* Improve product availability and inventory planning
* Tailor marketing and promotional strategies
* Enhance customer experience through targeted engagement
* Increase overall revenue and operational efficiency

---

