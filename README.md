# 🛒 Target Brazil E-Commerce Data Analysis  

This project analyzes the **Target Brazil E-Commerce dataset** containing over **100,000 orders placed between 2016 and 2018**.  
The analysis provides actionable insights into customer behavior, order trends, payments, delivery performance, and the overall impact of e-commerce operations in Brazil.  

---

## 📂 Dataset Overview  

The dataset is publicly available and consists of **8 CSV files**, each representing a different business dimension:  

- **customers.csv** → Customer details (location, unique IDs)  
- **sellers.csv** → Seller details (location, IDs)  
- **order_items.csv** → Items within each order (price, freight, product, seller)  
- **geolocation.csv** → Zip codes, lat/long, city, and state mappings  
- **payments.csv** → Payment methods, installments, values  
- **reviews.csv** → Customer review scores, comments, and timestamps  
- **orders.csv** → Order-level details (status, purchase, delivery, estimated delivery)  
- **products.csv** → Product-level attributes (category, weight, dimensions)  

📌 Dataset Source: [Google Drive Link](https://drive.google.com/drive/folders/1TGEc66YKbD443nslRi1bWgVd238gJCnb)  

---

## 📝 Problem Statement  

As a **data analyst/scientist at Target**, the goal is to:  

- Explore customer, order, and seller trends in Brazil.  
- Understand the evolution of Target’s e-commerce operations from 2016–2018.  
- Assess the **economic impact** of orders (prices, freight, payments).  
- Evaluate **delivery efficiency** and **customer satisfaction**.  
- Generate actionable insights for **business decision-making**.  

---

## 🔍 Key Analyses Performed  

### 1. Data Exploration  
- Data types and schema validation.  
- Order timeline: earliest and latest purchases.  
- Distribution of customers across **cities and states**.  

### 2. Order Trends & Seasonality  
- Growth in number of orders year by year.  
- **Monthly seasonality** in order placement.  
- **Time-of-day analysis** (Dawn, Morning, Afternoon, Night).  

### 3. Geographic Insights  
- Month-on-month orders by **state**.  
- Customer distribution heatmap across Brazil.  

### 4. Economic Analysis  
- % increase in order cost from **2017 to 2018 (Jan–Aug)**.  
- Total & average **order prices** per state.  
- Total & average **freight costs** per state.  

### 5. Delivery Performance  
- **Time to deliver** = `order_delivered_customer_date - order_purchase_timestamp`  
- **Delivery difference** = `order_delivered_customer_date - order_estimated_delivery_date`  
- Top 5 states with:  
  - Highest & lowest **average freight value**  
  - Highest & lowest **average delivery time**  
  - Fastest deliveries vs estimated timelines  

### 6. Payment Insights  
- Month-on-month **payment type trends** (credit card, boleto, vouchers, etc.).  
- Distribution of **installment-based purchases**.  

---

## 📊 Expected Outcomes  

- Identification of **fastest & slowest states** in delivery.  
- Insights into **customer shopping patterns** by season, month, and hour.  
- Analysis of **freight costs vs order value** across regions.  
- Evaluation of **payment preferences** among Brazilian customers.  
- Recommendations for improving **delivery efficiency** and **customer satisfaction**.  

---

## 🛠️ Tech Stack  

- **SQL** (MySQL / PostgreSQL)  
  - Joins (INNER, LEFT, RIGHT, FULL)  
  - Window Functions (ROW_NUMBER, RANK, DENSE_RANK, NTILE)  
  - Aggregate Functions (SUM, AVG, COUNT, MIN, MAX)  
  - String Functions (CONCAT, SUBSTRING, LENGTH)  
  - Date & Time Functions (DATEDIFF, EXTRACT, DATE_FORMAT)  
  - Conditional Expressions (CASE WHEN)  
  - Grouping & Filtering (GROUP BY, HAVING, WHERE)  
  - Subqueries & CTEs (WITH clause)  
  - Ordering & Limiting (ORDER BY, LIMIT)  


---

## 🚀 How to Use  

1. Clone this repository  
   ```bash
   git clone https://github.com/your-username/target-brazil-analysis.git
   cd target-brazil-analysis
