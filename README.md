# power-bi-financial-call-analysis-dashboard
Power BI dashboard analyzing financial call analysis dashboard performance using DAX
# 📞 Power BI Dashboard: Contact Center Performance

## 📌 Overview
This project is part of a Data Analyst internship task. It showcases how Power BI can be used to analyze a call center's performance and sales conversion using an Excel dataset.

---

## 📁 Dataset
- **File**: `financial data set.xlsx`
- **Type**: Customer service call records
- **Fields**:
  - CallID
  - AgentID, Agent_Name
  - PickedUp (1 = Answered, 0 = Missed)
  - Duration (seconds)
  - ProductSold (1 = Yes, 0 = No)

---

## 📊 KPIs (DAX Measures)
- `Total Calls = DISTINCTCOUNT(CallID)`
- `Answered Calls = CALCULATE(COUNT(CallID), PickedUp = 1)`
- `Unanswered Calls = CALCULATE(COUNT(CallID), PickedUp = 0)`
- `Products Sold = CALCULATE(COUNT(CallID), ProductSold = 1)`
- `Total Duration = SUM(Duration)`
- `Avg Call Duration = AVERAGE(Duration)`
- `Conversion Rate = Products Sold ÷ Answered Calls`

---

## 📈 Dashboard Visuals
- **KPI Cards**: Calls, Duration, Conversion Rate
- **Bar Chart**: Answered vs Unanswered by Agent
- **Column Chart**: Products Sold by Agent
- **Column Chart**: Avg Call Duration by Agent
- **Slicers**: Agent Name, ProductSold, PickedUp

---

## 🖼️ Screenshots

![Dashboard Preview](images/dashboard-full.png)

---

## 🧠 Insights
- Top agents identified by sales performance
- Conversion rate calculated per answered calls
- High volume of missed calls flagged for training

---

## 📤 Files Included
- `Dashboard.pbix`: Power BI file
- `financial data set.xlsx`: Dataset
- `PowerBI_Contact_Center_Dashboard_Summary.pptx`: Summary presentation
- `/images/`:  screenshots

---

## 🛠 Tools Used
- Power BI Desktop
- DAX

---

## 👤 Author
**Kalkotwar Akhil 
Data Analyst Intern – 25/04/2025

