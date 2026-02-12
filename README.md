📊 Digital Marketing Analytics — Power BI
I built this project to understand why a D2C brand was losing money despite having "cheap" ads.
Spoiler: The cheapest platform had a 31% return rate. The expensive one was actually more profitable.

The Business Problem
A D2C e-commerce brand was running ads on Meta, Google Ads & LinkedIn.
On paper, Meta looked great — lowest cost per customer (₹355).
But 1 in 3 Meta orders was being returned (RTO).
After digging into 28,000+ orders across 90 days, the real picture was very different.

What I Found
Meta — The Trap

CAC looks cheap at ₹355
But 31.66% RTO means massive hidden losses
True cost is ~40% higher than it appears

Google Ads — The Winner

CAC of ₹106, RTO of only 5.91%
18x ROAS, drives 70% of total orders
Expensive to acquire, but customers actually keep the product

LinkedIn — Pause It

ROAS of 0.68 (losing ₹0.32 on every ₹1 spent)
Net loss of ₹2.42L across 3 campaigns
Pausing LinkedIn + moving budget to Google = ~₹1.15 Cr saved annually


What I Built
Data Model: Star schema with 2 fact tables (FactSales + FactMarketing) and 4 dimensions (Campaign, Date, City)
ETL: Raw data was intentionally messy — 3 different date formats, currency symbols in number columns, 7 variations of "Delivered", duplicate rows. Cleaned everything in Power Query (18 transformation steps).
DAX Measures: CAC, ROAS, RTO%, Net Profit, Effective CAC, Platform Efficiency Score
Dashboards:

Executive Overview
Finance & Time Analysis
Campaign Performance
Key Insights page (the one I'm most proud of)


Data Issues I Fixed
The raw data had real-world messiness built in:
ProblemFixDates in 3 formatsPower Query locale conversion"₹3293.17" stored as textRemove symbol → convert to Decimal"delivered", "DELIVERED", "Dlvrd"Standardize to "Delivered"RTO reason filled on delivered ordersConditional null replacement35 duplicate rowsRemove DuplicatesPlatform: "meta", "Facebook Ads", "META"Replace Values → "Meta"



screenshots/
  01_executive_dashboard.png
  02_finance_analysis.png
  03_campaign_performance.png
  04_key_insights.png

digital_marketing_analytics.pbix

Tools
Power BI · Power Query (M) · DAX · Star Schema

The Biggest Takeaway
Low acquisition cost doesn't mean profitable customer.
You have to track what happens after the click —
RTO rate, payment method, day of week, city tier.
That's where the real story is.

Built as part of a self-directed Power BI learning project.
Actively looking for Data Analyst roles — open to connect!
LinkedIn: [https://www.linkedin.com/in/rohit-joshi-100a97394/]
Email: [workwithrj07@gmail.com]
