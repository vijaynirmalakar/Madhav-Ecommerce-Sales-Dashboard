#### Project Background
I recently completed an end-to-end data analysis project on Madhav Ecommerce Store's 2018 sales data using Power BI. The dataset contained 1,500 transactions across 3 product categories, 5 payment modes, and multiple Indian states.
What started as a simple dashboard project turned into a deep investigation because the numbers told a very different story than expected.

#### Metric	Value	Interpretation
Total Sales (Revenue) --->	₹4,37,771	(Total money received from customers)

Total Profit --->	₹36,963	(Net profit after cost of goods)

Overall Profit Margin --->	8.44%	(Low — needs improvement)

Total Transactions --->	1,500	(Total orders placed)

Total Quantity Sold --->	5,615 (units	Total items sold across all orders)

Loss-Making Transactions --->	529 out of 1,500	(35% orders resulted in loss)

#### The Monthly Profit Problem
When I plotted profit by month, something immediately stood out 

5 months had negative profit:
Month	Profit	Loss Orders

May	-₹3,730 🔴	72.88%

July	-₹2,138 🔴	73.44%

September	-₹1,399 🔴	69.88%

December	-₹1,604 🔴	23.42%

#### What's Actually Working
Not everything was bad. Here's what the data showed as strengths —

Best Months: November (₹10,253 profit) and January (₹9,684 profit)

Best Category: Clothing — highest profit margin at 9.23%

Best Sub-Category: Printers — ₹8,606 total profit

Top Market: Maharashtra — ₹1,02,498 in revenue


### Key Recommendations
Based on the analysis, here are 3 actionable recommendations:

1. Fix Electronics Pricing
   
Phones and Electronic Games are bleeding money. A pricing review or reducing discounts during May–September could alone recover ₹6,000+ in annual profit.

4. Promote Credit Card Payments
   
Credit Card has 14.51% margin vs 4.79% for UPI. Offering small cashback incentives for card payments could shift behavior and significantly improve margins.

7. Double Down on Clothing + Printers
   
These two are the most profitable areas. Focused inventory and marketing here would  highest ROI.

#### Tools & Process Used
Data Pipeline followed:

Data Collection — Kaggle dataset (Orders + Details tables)
   
Data Cleaning — Fixed incorrect Sales calculation, identified anomalies
   
Data Processing — Merged tables, created calculated columns
   
EDA — Month-wise, category-wise, payment-wise breakdown
   
Visualization — Power BI dashboard with KPIs, charts, slicers
    
Insights — Root cause analysis + business recommendations

#### Biggest Learning
When I first built the dashboard, Total Sales showed ₹2 Million.

After investigation, the correct figure was ₹4.37 Lakh.

I had accidentally multiplied Amount × Quantity — but Amount was already the total order value.

This is why EDA and data validation matter before building any dashboard.
Clean data first. Visuals second. Always.
