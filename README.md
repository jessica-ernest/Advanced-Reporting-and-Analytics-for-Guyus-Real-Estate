#  🏠 Advanced-Reporting-and-Analytics-for-Guyus-Real-Estate — Power BI

---

## 1. Business Context & Objectives

### The Company
Guyus Real Estate is a large real estate company managing 
residential, commercial and land sales across multiple 
US states. They handle thousands of transactions monthly 
across a wide network of agents and locations.

### The Problem
The company relied entirely on Excel for monthly sales 
reporting. This created serious business challenges:
- Reports took days to compile manually
- Data errors and inconsistencies were common
- Executives couldn't access real-time insights
- Strategic decisions were delayed waiting for reports
- No way to drill down by agent, state or property type

### The Objective
Design and deliver a fully automated Power BI dashboard 
that gives executives real-time visibility into:
- Total sales, transactions, average and max sales price
- Agent performance rankings
- Sales trends by month
- Performance by property type
- Geographic breakdown by state

---

## 2. Data Sources & Data Preparation

### Data Source
- Monthly Excel files stored in a shared folder
- Data covered: transactions, agents, property types, 
  states, cities and sale amounts
- Volume: 6,000+ transaction records

### Data Preparation Steps
1. Connected Power BI directly to the Excel folder 
   (folder connector — auto-updates when new files added)
2. Opened Power Query to clean and transform data:
   - Removed duplicate transaction records
   - Handled null/missing values in sales columns
   - Standardized agent name formatting
   - Corrected data types (dates, currencies, numbers)
   - Split location fields into State and City columns
3. Built a star schema data model with:
   - Fact table: Transactions
   - Dimension tables: Agents, Properties, Locations, Dates
4. Created table relationships in Model View

---

## 3. Analytical Methodology & Approach

### Data Modelling
Built a star schema to enable fast, flexible querying 
across all dimensions of the business.

### DAX Measures Created
- Total Sales = SUM(Transactions[SaleAmount])
- Total Transactions = COUNTROWS(Transactions)
- Average Sales = AVERAGE(Transactions[SaleAmount])
- Max Sales Price = MAX(Transactions[SaleAmount])
- MoM Sales Change = (This Month - Last Month) / 
  Last Month × 100

### Dashboard Design Decisions
- KPI cards at top for executive-level summary
- Line chart for monthly sales trends 
  (spot seasonal patterns instantly)
- Horizontal bar chart for agent rankings 
  (easy top performer identification)
- US Map visual for geographic performance
- Donut chart for property type split
- Slicers: Quarter, Month, Property Type, 
  City, Agent Name
- Drill-through page for granular state + 
  agent + property analysis

---

## 4. Results & Key Insights

### KPI Summary
| Metric | Value | Change vs Last Month |
|--------|-------|----------------------|
| Total Sales | $3bn | ▲ 16.8% |
| Total Transactions | 6,000 | ▲ 16.7% |
| Max Sales Price | $1,000K | 0.0% |
| Average Sales | $553K | ▲ 0.1% |

### Key Findings

**Agent Performance:**
- Top agent Robert Davis closed 287 transactions
- Top 5 agents (Davis, Miller, Garcia ×2, Williams) 
  were closely competitive — healthy team balance
- Opportunity: bottom-performing agents need support 
  or retraining

**Monthly Trends:**
- February was the lowest month at $422M 
  — classic Q1 seasonal dip in real estate
- May peaked at $472M before slight July decline
- Recommendation: run promotions in Feb/March 
  to counter seasonal slowdown

**Property Type Split:**
- Land: 35.46% — highest seller
- Commercial: 32.32%
- Residential: 32.22%
- Insight: Land sales dominating is unusual — 
  suggests development market opportunity

**Geographic Performance:**
- Texas and California were top performing states
- Opportunity: underperforming states identified 
  for targeted agent deployment

---

## 5. Implementation, Monitoring & Next Steps

### What Was Delivered
- Fully automated Power BI dashboard live in 
  Power BI Service
- Replaced 100% of manual Excel reporting
- Folder connector means dashboard refreshes 
  automatically when new monthly data is added
- Two pages: Executive Overview + Drill-through 
  Detail View

### Business Impact
- Estimated 15+ hours per month saved on 
  manual reporting
- Zero manual data entry errors going forward
- Executives now access insights in real time 
  instead of waiting days for reports
- Sales team can self-serve their own performance data

### Next Steps & Recommendations
1. Add a YoY (Year over Year) comparison page
2. Build an agent target vs actual tracker
3. Add customer demographics data for deeper 
   buyer behaviour analysis
4. Set up automatic email report subscription 
   for executives
5. Expand to include profit margin data 
   not just revenue

---

## 🛠️ Tools Used
Power BI · DAX · Power Query · Excel · Data Modelling · 
Star Schema Design

---

## 🔗 Live Dashboard
[👉 Click Here to View Live Dashboard] https://app.powerbi.com/links/adeA0dHqAC?ctid=455dfcec-e922-4d88-92d8-50622c950c2f&pbi_source=linkShare

---

## 📸 Screenshots
![Executive Overview](https://raw.githubusercontent.com/jessica-ernest/Advanced-Reporting-and-Analytics-for-Guyus-Real-Estate/main/Real%20Estate%20Dashboard%201..png)
