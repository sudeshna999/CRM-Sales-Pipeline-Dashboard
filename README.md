
#  CRM Sales Pipeline Dashboard – Power BI Project

> **“Track and optimize your sales funnel using a dynamic, visual CRM dashboard built for performance, insights, and growth.”**

---

##  Project Overview

This Power BI dashboard presents a comprehensive view of the **CRM Sales Pipeline**, designed to help businesses monitor lead status, analyze sales team performance, identify bottlenecks, and improve conversion rates.

By transforming raw CRM data into actionable insights, this dashboard supports strategic decision-making and enhances the visibility of the entire sales journey — from initial contact to deal closure.

> **Link** https://app.powerbi.com/view?r=eyJrIjoiYTU5ODg2ZDEtMThlYS00YTg3LWI0MzMtOWFkNTI3YTEzNDVjIiwidCI6ImZjNTIzNTI4LTNkMzgtNGNhMy05NGRkLTU5NjIzMDJkMzBlOCJ9


---
>  **Use Case**: B2B or B2C CRM analytics  
>  **Target Users**: Sales managers, marketing teams, and business analysts  
>  **Outcome**: Data-driven strategies to boost revenue and sales efficiency  

---

##  Tech Stack

- **Power BI Desktop** – Dashboard creation and interactivity  
- **Power Query** – Data transformation and cleansing  
- **DAX** – Calculated fields, KPIs, and dynamic measures  
- **Excel / SQL** – Source of CRM data (e.g., leads, deals, revenue)

---

##  Dashboard Features

-  **Sales Pipeline Overview**: Track leads across stages (New, Qualified, Proposal, Closed)  
-  **Sales Rep Performance**: Revenue by rep, win/loss ratio, deal size insights  
-  **Time to Close**: Average days from lead to closure by stage  
-  **Conversion Rates**: Funnel metrics across lead journey  
-  **Deal Type & Segment Analysis**: Filter by product type, customer segment, industry  
- **Risk & Opportunity Indicators**: Identify stuck or at-risk deals  

---

##  Business Objectives

- Gain full visibility into the sales funnel and performance trends  
- Identify high-performing reps and underperforming segments  
- Highlight stages with drop-offs or excessive time lags  
- Enable focused strategy and performance coaching based on data  
- Drive accountability with clear KPIs and conversion insights  

---

##  Key Insights Unlocked

| Metric | Insight Example |
|--------|-----------------|
|  Win Rate | Rep A closes 70% of qualified leads, highest in the team |
|  Stage Drop-off | 35% of leads drop between "Qualified" and "Proposal Sent" |
|  Time to Close | Enterprise deals take 2x longer to close than SMB deals |
|  Revenue Trends | Deals in the Software segment increased by 45% |
|  Lost Deal Reasons | Price sensitivity and delayed decision-making dominate losses |

---

##  Folder Structure

```plaintext
 crm_sales.pbix           # Power BI dashboard file
 README.md                # Project documentation
 assets/                  # Dataset and Icons
```

## Sample DAX Measures

```Win Rate % = 
DIVIDE(
    CALCULATE(COUNTROWS(Deals), Deals[Status] = "Won"),
    CALCULATE(COUNTROWS(Deals), Deals[Status] IN {"Won", "Lost"}),
    0
)

Avg Deal Size = AVERAGE(Deals[Revenue])

Conversion Rate = 
DIVIDE(
    COUNTROWS(FILTER(Deals, Deals[Stage] = "Closed")),
    COUNTROWS(FILTER(Deals, Deals[Stage] = "Lead")),
    0
)
```

---

## Dashboard Pages

![image](https://github.com/user-attachments/assets/68cf9e84-3504-41f3-8a1b-8cd7a9d0f53e)

![image](https://github.com/user-attachments/assets/af153342-edc7-40d6-a0d1-2f21564a03b3)

![image](https://github.com/user-attachments/assets/7044ab1f-6e0d-4141-bc65-a9a7fd21b1a0)

![image](https://github.com/user-attachments/assets/6ee159ab-bd57-4da8-99b1-629f469decbb)

---




---


## Author
### — Sudeshna Dey
###  — Contact & Contributions

####  Email: sudeshnadey1000@gmail.com
####  LinkedIn: https://www.linkedin.com/in/sudeshna-dey-724a811a0/
Have feedback or suggestions? I'm always open to improving and collaborating!
 
If you find this project helpful:
Give it a star
Thanks for visiting — and happy data analyzing!


