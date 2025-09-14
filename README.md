# HubSpot Marketing Analytics Dashboard
![Dashboard Preview](dashboard/Hubspot%20Marketing%20Analytics%20Dashboard%20Screenshot.jpg)

## 📊 Project Overview
This project analyzes marketing and sales performance using **HubSpot data** stored in **Snowflake** and visualized with **Power BI**.  
The goal is to track the customer journey from **Leads → Deals → Closed Wins**, evaluate campaign performance, and highlight revenue opportunities.

---

## ⚙️ Technical Steps
1. **Data Integration**: HubSpot exports (`contacts.csv`, `deals.csv`, `emails.csv`) were loaded into **Snowflake** for storage and querying.  
2. **Data Modeling**: Relationships were defined between contacts, deals, and campaigns for a unified view of the marketing funnel.  
3. **DAX Measures**: Built KPIs including:  
   - `Total Revenue = SUM(Deals[Amount])`  
   - `Total Deals = COUNTROWS(Deals)`  
   - `Conversion Rate = DIVIDE([Closed Wins], [Leads], 0)`  
4. **Power BI Visuals**: Funnel chart (Leads → Deals → Wins), Campaign trend lines, Revenue by Country, and segmented deal analysis by income group.  
5. **Interactive Filters**: Slicers for Date, Country, Campaign, and Income allow dynamic exploration.

---

## 📈 Key Insights
- Lead-to-Win conversion rate: **14.7%**  
- Top revenue countries: **Spain**, **Saudi Arabia**  
- High-income customers generate **2.3x higher average deal size** compared to low-income segments  
- Campaign response trends peak during **August–October**  

---

## 💡 Features
- **Funnel Chart**: Visualizes drop-offs from Leads → Deals → Wins.  
- **Revenue by Country**: Highlights regional performance differences.  
- **Campaign Trends**: Line chart tracking open/click/conversion over time.  
- **Top 10 Customers Table**: Identifies the most valuable accounts.  
- **Dynamic Filter Panel**: Users can segment by country, campaign, or income with one slicer.  

---

## 🛠️ Tech Stack
- **Snowflake** → Data storage & transformations  
- **HubSpot** → Source CRM & marketing data  
- **Power BI** → Dashboard creation and visualization  

---

## 📂 Repo Structure
HubSpot-Marketing-Analytics-Dashboard/
│
├── data/
│ ├── contacts.csv
│ ├── deals.csv
│ └── emails.csv
│
├── dashboard/
│ ├── Marketing_Funnel_HubSpot.pbix
│ └── HubSpot_Dashboard.png
│
└── README.md
