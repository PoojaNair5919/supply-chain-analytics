# Supply Chain Analytics Dashboard

![Dashboard Demo](dashboard_gif.gif)

This project analyzes global supply chain performance using data analytics and interactive dashboards.

The analysis focuses on understanding delivery delays, product performance, logistics efficiency, and customer purchasing behavior across more than **180,000 orders**.

---

## Project Overview

Supply chain operations involve multiple moving parts, including inventory management, shipping processes, product demand, and customer behavior.

While exploring this dataset, one operational metric immediately stood out:

**Nearly 35% of orders were delivered later than scheduled.**

To investigate this further, I built an interactive analytics dashboard that examines financial performance, shipping operations, product demand, and customer behavior.

---

## Dataset

Dataset Source:

**DataCo Smart Supply Chain for Big Data Analysis**

https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis

The dataset includes information related to:

- Orders  
- Shipments  
- Products  
- Customers  
- Delivery performance  

Total records: **~180,000 order items**

---

## Data Preparation

Initial data exploration and preprocessing were performed using **Python and Pandas**.

Key steps included:

- Inspecting dataset structure and data types  
- Validating dataset grain (order-item level)  
- Removing irrelevant and sensitive columns  
- Converting date fields to proper datetime format  
- Creating derived metrics such as **Delivery Delay**  
- Generating a simplified **Delivery Status classification**

After preprocessing, the cleaned dataset was imported into **Power BI** for modeling and dashboard development.

---

## Data Model

The dataset was structured using a **star schema** to support flexible analytics.

### Fact Table

- `Fact_Order_Items`

### Dimension Tables

- `Dim_Product`
- `Dim_Customer`
- `Dim_Location`
- `Dim_Shipping`
- `Dim_Date`

This modeling approach improves query performance and simplifies analysis across multiple business dimensions.

![Data Model](star_schema.jpg)

---

## Key Metrics

The dashboard tracks several business and operational KPIs.

### Financial Metrics

- **Total Revenue**
- **Total Profit**
- **Average Order Value (AOV)**

### Operational Metrics

- **Delayed Orders %**
- **Average Delivery Delay**

### Customer Metrics

- **Total Customers**
- **Revenue per Customer**
- **Orders per Customer**

---

## Dashboard Views

The Power BI report is organized into four analytical dashboards.

### Executive Supply Chain Overview

Provides a high-level summary of revenue, orders, profitability, and delivery performance.

![Executive Dashboard](executive_supply_chain_overview.jpg)

---

### Logistics Performance

Analyzes shipping efficiency, delay distribution, and operational performance across shipping modes and markets.

![Logistics Dashboard](logistics_performance.jpg)

---

### Product Performance

Evaluates revenue and profitability across product categories and individual products.

![Product Dashboard](product_performance.jpg)

---

### Customer & Market Insights

Explores customer purchasing patterns and revenue distribution across markets and segments.

![Customer Insights](customer_market_insights.jpg)

---

## Key Insights

Some key observations from the analysis include:

- Approximately **35% of orders are delivered later than scheduled**
- Revenue is concentrated in a small number of product categories
- **Standard Class** accounts for the majority of shipments
- Customer revenue follows a **long-tail distribution**

---

## Tools Used

- **Python (Pandas)** – data exploration and preprocessing  
- **Power BI** – dashboard development  
- **DAX** – KPI calculations  
- **Dimensional Data Modeling** – star schema design  

---

## Related Links

### Medium Article  
(Add Medium article link here)

### Portfolio Project Page  
(Add HTML portfolio page link here)

### GitHub Repository  
(You are currently here)

---

## Author

**Pooja Nair**

Business Intelligence & Analytics Enthusiast
