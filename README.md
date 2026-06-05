# 📊 Sales Insights Dashboard – Power BI

## 🏢 Project Overview

An end-to-end **Sales & Profit Analytics Dashboard** built in Power BI to help a multi-market Indian business uncover revenue trends, profitability gaps, and market-level performance. The dashboard enables business stakeholders to make data-driven decisions on market strategy, product focus, and customer prioritisation.

---

## 📁 Data Model

A **Star Schema** with 1 fact table and 4 dimension tables:

| Table | Type | Key Columns |
|---|---|---|
| `Fact_Transactions` | Fact | sales_amount, sales_qty, cost_price, profit_margin, order_date |
| `Dim_Products` | Dimension | product_code, product_type |
| `Dim_Customers` | Dimension | customer_name, customer_code, customer_type |
| `Dim_Markets` | Dimension | market, markets_code, zone |
| `Date` | Date Table | date, month_name, fiscal_quarter, year, year hierarchy |

---

## 🛠️ Tools & Techniques

- **Power BI Desktop** — data modelling, visualisation, report design
- **Power Query (M)** — data transformation and cleaning
- **DAX** — custom measures and calculated columns

### DAX Measures Built

| Measure | Description |
|---|---|
| `Revenue` | Total sales amount |
| `Profit` | Revenue minus cost price |
| `Profit Margin %` | Profit as % of Revenue |
| `Profit YTD` | Year-to-date profit using TOTALYTD |
| `Profit PY` | Prior year profit using SAMEPERIODLASTYEAR |
| `Profit YOY` | Year-over-year profit variance |
| `AOV` | Average Order Value |
| `ASP` | Average Selling Price |
| `Revenue per Customer` | Revenue divided by unique customers |
| `Total Orders` | Count of distinct transactions |

---

## 📄 Dashboard Pages

### Page 1 — Sales Analysis (Dashboard)
> Overview of overall sales performance across markets, products, and customers

- **KPIs:** Revenue ₹985M | Sales Quantity 2M | Total Orders 148K
- Revenue by Market (bar chart) — Delhi NCR leads all markets
- Sales Quantity by Market — Delhi NCR and Mumbai dominate volume
- Top 5 Customers by Revenue — Electricalsara Stores leads at ₹413M
- Top 5 Products by Revenue — Prod318 and Prod316 are top performers
- Annual Revenue Trend (2017–2020) — peaked at ₹414M in 2018, declining to ₹142M in 2020
- **Tooltip Page** — hovering over any year on the revenue trend reveals a monthly revenue breakdown for that year, showing seasonal peaks in Aug–Sep (₹35–36M) and dips in Apr–May and December

---

### Page 2 — Profit Analysis
> Deep-dive into profitability across time, geography, and product

- **KPIs:** Profit ₹25M | Profit Margin % 2.50% | Profit YTD ₹2.1M
- Year slicer: 2017 | 2018 | 2019 | 2020
- Profit vs Profit PY by Month — trend line comparison against prior year
- Profit by Fiscal Quarter — steady growth from Q1 (₹3.8M) to Q4 (₹7.7M)
- Profit by Zone (pie chart) — North dominates at **61.14%**, Central 34.76%, South 4.09%
- Market-wise Profit Contribution (Top 8) — Delhi NCR leads at ₹1.19Cr
- Top 8 Products by Profit — Prod329 and Prod318 are most profitable

---

### Page 3 — Performance Insights
> Market-level profitability matrix with business interpretation

- **KPIs:** Profit Margin % 2.50% | AOV ₹6.64K | ASP ₹405
- Market-level table: Revenue, Profit, **Profit Margin % (colour-coded)**, ASP
- Top 5 Markets by Profit Margin % — Surat (4.86%), Patna (4.12%), Bhubaneshwar (3.98%)
- Top 5 Markets by Revenue — Delhi NCR dominates at 56.74% share
- Loss-making markets highlighted in red: **Bengaluru (-20.78%)** and **Kanpur (-0.49%)**

### 💡 Key Business Insights
- **Delhi NCR** contributes ~57% of total revenue but profit margin is only **2.3%** — high volume, low efficiency
- **Surat** has the highest profit margin at **4.86%** despite lower revenue
- **Bengaluru and Kanpur are loss-making markets** — immediate review needed
- **Mumbai** delivers strong profit with a healthy margin of **3.25%**
- Overall business profit margin stands at a thin **2.50%** — margin improvement is a priority
- Revenue peaked in **2018 at ₹414M** and has been declining — needs strategic intervention
- **North Zone drives 61%** of total profit, indicating geographic over-dependence

---

## 📂 Files in This Repository

| File | Description |
|---|---|
| `Sales_Insights.pbix` | Power BI dashboard file |
| `README.md` | Project documentation |
| `screenshots/` | Dashboard page screenshots |

---

## 🚀 How to Use

1. Download `Sales_Insights.pbix`
2. Open in **Power BI Desktop** (free download from Microsoft)
3. Use the year slicer (2017–2020) to filter across all pages
4. Navigate pages using buttons: **Dashboard → Profit Analysis → Performance Insights**

---

## 👩‍💼 About the Author

**Padmaja Akella** | Banking Professional with Data Analytics Skills
- 8 years of experience in Public Sector Banking — Retail Credit, Credit Appraisal & Risk, Customer Service
- Skills: Power BI | DAX | SQL | Python | Advanced Excel | EDA
- 📧 [akellapadmaja@gmail.com] | 🔗 [www.linkedin.com/in/padmajaakella]

---

*This project is part of a data analytics portfolio combining domain expertise in banking and finance with data visualisation skills.*
