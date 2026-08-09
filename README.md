# 🛒 Olist E-Commerce Sales & Business Performance Analysis

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![Excel](https://img.shields.io/badge/Excel-Data%20Preparation-green)
![DAX](https://img.shields.io/badge/DAX-Data%20Modeling-blue)
![E-Commerce](https://img.shields.io/badge/Domain-E--Commerce-orange)

## 📌 Project Overview

This project analyzes the sales and operational performance of the Olist Brazilian e-commerce marketplace using Power BI.

The objective was to transform transactional marketplace data into actionable business insights across:

- Revenue growth
- Customer behavior
- Order fulfillment
- Delivery performance
- Product categories
- Seller performance
- Geographic contribution

The analysis follows a business-oriented approach, focusing not only on **what happened**, but also on identifying areas that may require management attention.

---

## 🎯 Business Objectives

The analysis was designed to answer key business questions:

1. How has marketplace revenue evolved over time?
2. Which customer states contribute the most revenue?
3. Which seller regions generate the highest revenue?
4. How strong is customer retention and repeat purchasing?
5. How efficiently are orders being fulfilled?
6. Which regions experience higher delivery times?
7. Which product categories contribute the most revenue?
8. How is the seller base distributed across regions?
9. Are there potential operational bottlenecks affecting customer experience?

---

# 📊 Dashboard

## Executive Overview

The Executive Overview provides a high-level view of marketplace performance across revenue, orders, customers, sellers, AOV, customer ratings and fulfillment.

![Executive Overview](images/executive_overview.png)

### Key Insights

- Total revenue generated was approximately **13.59M**.
- The marketplace processed approximately **98.67K orders**.
- Average Order Value was approximately **137.75**.
- Overall customer rating was approximately **4.09 / 5**.
- Order fulfillment rate was approximately **97%**.
- Revenue showed strong growth during the observed period, although the dataset contains incomplete data for 2018.

---

# 👥 Customer Analysis

The Customer Analysis page focuses on customer behavior, geographic contribution and purchasing patterns.

![Customer Analysis](images/customer_analysis.png)

### Key Insights

- **São Paulo (SP)** is the largest customer revenue contributor by a significant margin.
- The top customer states are concentrated in a relatively small number of regions.
- Customer repeat rate is relatively low, indicating an opportunity to improve customer retention.
- Health & Beauty, Watches & Gifts and Bed/Bath/Table were among the leading revenue-generating product categories.
- Several states show particularly low repeat customer rates and may require targeted retention initiatives.

---

# 🚚 Orders & Delivery Analysis

This page evaluates marketplace fulfillment and delivery performance.

![Orders and Delivery Analysis](images/orders_delivery_analysis.png)

### Key Insights

- Approximately **97.02% of orders were delivered**, indicating strong overall fulfillment performance.
- Late deliveries represent a smaller but meaningful operational issue.
- Delivery performance varies significantly across states.
- Certain states show higher median delivery times and may require deeper investigation.
- The relationship between actual delivery time and late-delivery rate highlights regional differences in operational performance.

### Management Implication

Rather than treating delivery performance as a marketplace-wide issue, management should investigate **specific high-delay regions and their underlying logistics constraints**.

---

# 📦 Product Analysis

The Product Analysis page examines product categories and their contribution to marketplace revenue.

![Product Analysis](images/product_analysis.png)

### Key Insights

- Revenue is distributed across several major product categories.
- Health & Beauty was among the leading revenue-generating categories.
- Category-level performance can help identify areas for assortment expansion and promotional opportunities.
- Category performance should be evaluated together with customer demand and seller availability before making expansion decisions.

---

# 🏪 Seller Analysis

The Seller Analysis page evaluates seller distribution, revenue contribution and seller productivity.

![Seller Analysis](images/seller_analysis.png)

### Key Insights

- The marketplace has approximately **3.1K sellers**.
- São Paulo has the largest seller base.
- Seller revenue contribution is geographically concentrated.
- Average revenue per seller varies substantially across states.
- A relatively small proportion of sellers operate across multiple categories, indicating a predominantly single-category seller base.

### Management Implication

The difference between **seller count and revenue contribution** suggests that seller density alone does not determine regional revenue performance.

This creates an opportunity to investigate seller productivity, category mix and regional demand-supply alignment.

---

# 🔍 Data Model

The project uses a relational data model connecting customers, orders, order items, sellers, products, payments, reviews, geography and product categories.

![Data Model](images/data_model.png)

### Main Tables

- `olist_customers_dataset`
- `olist_orders_dataset`
- `olist_order_items_dataset`
- `olist_order_payments_dataset`
- `olist_order_reviews_dataset`
- `olist_products_dataset`
- `olist_sellers_dataset`
- `olist_geolocation_dataset`
- `product_category_name`
- `Calendar`

---

# 🧮 Key KPIs

| KPI | Value |
|---|---:|
| Total Revenue | 13.59M |
| Total Orders | 98.67K |
| Total Customers | 96.10K |
| Total Sellers | 3.10K |
| Average Order Value | 137.75 |
| Average Customer Rating | 4.09 / 5 |
| Order Fulfillment Rate | 97.02% |
| Late Delivery Rate | 7.74% |
| Customer Lifetime Value | 142.44 |

---

# 🛠️ Tools & Technologies

### Data Preparation
- Microsoft Excel
- Power Query

### Data Analysis & Visualization
- Microsoft Power BI
- DAX

### Data Modeling
- Star-schema / relational modeling concepts
- Dimension and fact table relationships
- Calendar table

---

# 📈 Analytical Approach

The project followed a structured analytical workflow:

**Raw Data → Data Cleaning → Data Modeling → DAX Measures → KPI Analysis → Visualization → Business Insights**

### 1. Data Preparation
- Cleaned and structured marketplace datasets.
- Handled missing and inconsistent values.
- Prepared categorical and date fields for analysis.

### 2. Data Modeling
- Connected transactional tables with customer, seller, product and geographic dimensions.
- Created a dedicated Calendar table.
- Established relationships required for cross-functional analysis.

### 3. KPI Development
Created measures for:

- Revenue
- Orders
- Customers
- Sellers
- Average Order Value
- YoY Growth
- Fulfillment Rate
- Late Delivery Rate
- Average Delivery Time
- Customer Lifetime Value
- Repeat Customer Rate
- Average Revenue per Seller

### 4. Business Analysis
The dashboard was structured around four major business areas:

**Customer → Orders & Delivery → Products → Sellers**

---

# 💡 Key Business Takeaways

### 1. Revenue is geographically concentrated

São Paulo is the dominant customer revenue market, significantly outperforming other states.

**Potential implication:**  
The marketplace may benefit from protecting its position in high-value markets while identifying scalable opportunities in underpenetrated regions.

---

### 2. Strong fulfillment but regional delivery gaps

Overall fulfillment is approximately 97%, suggesting strong marketplace execution. However, delivery performance varies considerably by region.

**Potential implication:**  
Operational improvement should focus on specific high-delay regions rather than applying a uniform marketplace-wide solution.

---

### 3. Customer retention remains an opportunity

The repeat customer rate is relatively low despite strong marketplace activity.

**Potential implication:**  
Customer retention initiatives such as personalized recommendations, targeted promotions and post-purchase engagement could potentially improve repeat purchasing.

---

### 4. Seller productivity varies significantly

Seller count does not necessarily translate into proportional revenue contribution.

**Potential implication:**  
Seller productivity should be analyzed alongside category mix, regional demand and order volume to identify high-potential seller segments.

---

### 5. Marketplace growth is strong but requires contextual interpretation

Revenue demonstrates substantial growth over the observed period. However, the dataset contains incomplete information for 2018.

**Important analytical limitation:**  
2018 should not be directly compared with complete years without accounting for the limited observation period.

---

# ⚠️ Data Limitations

This analysis is based on the publicly available Olist Brazilian e-commerce dataset and therefore has several limitations:

- 2018 data is available only through September.
- The dataset represents historical marketplace activity rather than current Olist performance.
- The analysis identifies correlations and patterns but does not establish causality.
- Low repeat-customer rates may require additional customer-level behavioral data to determine underlying causes.
- Delivery issues would require logistics-partner and warehouse-level data for root-cause analysis.

Therefore, the dashboard should be interpreted as a **business diagnostic analysis rather than a causal study**.

---

# 🚀 Potential Next Steps

If additional data were available, the analysis could be extended into:

- Customer cohort analysis
- Customer segmentation
- Seller churn analysis
- Profitability analysis
- Logistics partner benchmarking
- Category-level margin analysis
- Regional market expansion analysis
- Customer retention modeling
- Seller productivity benchmarking

---

# 📁 Repository Structure

```text
Olist-Ecommerce-Analysis/
│
├── README.md
│
├── Dashboard/
│   └── Olist_Dashboard.pbix
│
├── Data/
│   └── Dataset_Source.txt
│
├── Images/
│   ├── executive_overview.png
│   ├── customer_analysis.png
│   ├── orders_delivery_analysis.png
│   ├── product_analysis.png
│   ├── seller_analysis.png
│   └── data_model.png
│
└── Documentation/
    └── Olist_Analysis_Report.pdf
