# Madhav Store E-Commerce Sales Dashboard
> Analyzed 1,500 transactions and ₹4.38L in revenue across 3 categories and 5 states using Power BI to uncover profitability patterns, loss-making months, and payment behaviour for an Indian e-commerce store.

---

## Problem
Madhav Store had sales data but no clear view of:
- Which months were profitable and which were making losses — and why
- Which product sub-categories and states were draining profit
- How customers prefer to pay, and which payment modes drive more volume

This project builds a 2-page Power BI dashboard answering all three questions with quarterly drill-through filters.

---

## Dataset
| File | Description | Size |
|---|---|---|
| `Orders.csv` | Order ID, Date, Customer, State, City | 500 rows |
| `Details.csv` | Amount, Profit, Quantity, Category, Sub-Category, Payment Mode | 1,500 rows |

- **Period:** 2018
- **Joined on:** Order ID (1 order → multiple line items)
- **Total unique customers:** 500 | **Total line items:** 1,500

---

## Tools Used
`Power BI` `DAX` `Power Query` `Data Modelling` `CSV` `Excel`

---

## Process

1. **Data Understanding** — Explored two relational CSV files (Orders + Details); identified one-to-many relationship on Order ID
2. **Data Modelling** — Connected Orders and Details tables in Power BI via Order ID relationship
3. **Data Cleaning** — Standardized date formats using Power Query, checked for nulls, verified category consistency
4. **DAX Measures** — Created calculated measures: Total Sales, Total Profit, Total Loss, Total Qty, Profit Margin %
5. **Dashboard Page 1 (Sales)** — KPI cards, Sales by Category (donut), Sub-Category bar chart, Profit by Month (waterfall), Payment Mode donut, Top Customers, Top States
6. **Dashboard Page 2 (Loss Report)** — Loss by Month, Loss Qty by Category, Loss by Sub-Category, Loss by State with quarterly slicer
7. **Insights** — Identified 4 loss-making months, top loss sub-categories, and regional loss hotspots

---

## Dashboard Preview

### Page 1 — Sales Overview
<img width="1328" height="746" alt="Madhav Ecommerce Store Sales Dashboard" src="https://github.com/user-attachments/assets/cd278b9a-7003-472b-8a01-f14f80cfd8f2" />


### Page 2 — Loss Analysis Report
<img width="1169" height="629" alt="Madhav Ecommerce Store Sales Dashboard2" src="https://github.com/user-attachments/assets/d28c289c-099a-4243-b825-e5554f9fe227" />


---

## Key Findings

- **Electronics is the top revenue category** at ₹1.66L (38%), but also the highest loss category (₹15,488 total loss)
- **4 months recorded losses** — May (−₹3,730), July (−₹2,138), September (−₹1,399), December (−₹1,604)
- **November is the most profitable month** at ₹10,253 profit, followed by January (₹9,684) — Q1 and Q4 peaks
- **COD is the dominant payment mode** at 45.6% of all transactions — cash dependency is a fulfilment risk
- **Maharashtra is the #1 state** at ₹1.02L in sales, followed by Madhya Pradesh (₹87,463)
- **Printers and Sarees tie as top sub-categories** at ₹59K+ each in revenue
- **Phones are the biggest loss-maker** at −₹5,761, followed by Saree (−₹5,301) and Electronic Games (−₹5,275)
- **529 of 1,500 transactions (35.3%) resulted in losses** — a significant fulfilment or pricing problem

---

## Business Recommendations

1. Investigate loss-making months (May, Jul, Sep, Dec) — likely driven by discounting or return spikes
2. Review Phones, Saree, and Electronic Games pricing — these 3 sub-categories alone account for the largest losses
3. Reduce COD dependency — incentivise UPI/Credit Card payments to lower return and cancellation risk
4. Double down on Maharashtra and Madhya Pradesh — they represent 43.1% of total sales combined
5. Replicate Q1 (Jan–Mar) strategies in Q3 — Q1 averages ₹8,647 profit/month vs Q3 average loss

---

## Project Structure
```
madhav-store-ecommerce-dashboard/
├── Orders.csv               # Order-level data (500 rows)
├── Details.csv              # Line-item data (1,500 rows)
├── Madhav_Dashboard.pbix    # Power BI report file
├── dashboard_sales.png      # Sales overview screenshot
├── dashboard_loss.png       # Loss analysis screenshot
└── README.md                # This file
```

---

## Author
**Vijay Nirmalakar**
[[LinkedIn Profile](https://www.linkedin.com/in/vijaynirmalakar/)] | [[GitHub Profile](https://github.com/vijaynirmalakar)]

*Tools: Power BI | DAX | Power Query | Skills: Data Modelling, Dashboard Design, Profit & Loss Analysis*
