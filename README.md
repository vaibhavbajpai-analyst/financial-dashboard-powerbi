📊 Financial Dashboard – Power BI Project

This repository contains a Financial Dashboard built using Power BI for analyzing company performance across revenue, profitability, receivables, and cash flows.

The project demonstrates how to transform raw financial data into an interactive dashboard with KPIs, charts, and drilldowns.

🚀 Project Files
shobhit.pbix → Power BI file (Dashboard & Data Model)
Data Analyst - TAG Case Study Data.xlsx → Raw dataset (Revenue, Expenses, Cash Flow, Aging, Budgets, etc.)
Financial Dashboard.JPG → Screenshot of the dashboard
📌 Dashboard Features

Key KPIs

Net Cash
EBITDA %
Revenue
Gross Margin %

Visuals & Analysis

Product/Service Revenue Share (Donut chart)
Receivables Aging (Buckets: <30, 30–60, >60 days)
Revenue & Profit Trend (Monthly trend)
Budget vs Actual Revenue (Comparison by Product/Service)
Cash Flow Analysis (Inflows, Outflows, Net Cash)

Filters / Slicers

Date Range
Product/Service
Period
Region
📂 Data Source

The dataset is provided in Excel (Data Analyst - TAG Case Study Data.xlsx), containing the following fields:

Time → Month
Dimensions → Region, Product/Service
Financials → Revenue, COGS, Gross Profit, Opex, EBITDA
Cash Flow → Inflows, Outflows
Working Capital → Receivables Aging (Days), Payables Aging (Days)
Budget Data → Revenue Budget, Budget Variance %
🧮 DAX Measures

Key calculated measures in Power BI:

Gross Profit = SUM(Revenue) - SUM(COGS)
Gross Margin % = DIVIDE([Gross Profit], SUM(Revenue), 0)
EBITDA = SUM(Gross Profit) - SUM(Opex)
EBITDA % = DIVIDE([EBITDA], SUM(Revenue), 0)
Net Cash = SUM(Cash Inflows) - SUM(Cash Outflows)
Receivables Aging = Bucketed into <30 Days, 30–60 Days, >60 Days
Budget Variance % = DIVIDE((SUM(Revenue) - SUM(Revenue Budget)), SUM(Revenue Budget), 0)
🏗️ Data Model
Fact Table → Financial transactions (Revenue, COGS, Cash Flows, etc.)
Dimensions → Date, Region, Product/Service
Relationships built for drill-downs and filtering.
📸 Dashboard Preview

⚙️ How to Use
Download the repository.
Open shobhit.pbix in Power BI Desktop.
Load the dataset from Data Analyst - TAG Case Study Data.xlsx (already connected in the PBIX).
Explore KPIs & use slicers for interactive analysis.
🎯 Insights
Product A & Service X contribute the largest revenue share.
Receivables of $14.8M are overdue (30–60 days), requiring working capital management.
EBITDA Margin at 18.6%, indicating healthy profitability.
Net Cash Position: $0.69M, showing moderate liquidity.
🛠️ Tools & Skills
Power BI (Dashboarding, DAX, Data Modeling)
Excel (Raw Data Preparation)
Data Analysis (Financial KPIs, Variance Analysis, Cash Flow Analysis)
