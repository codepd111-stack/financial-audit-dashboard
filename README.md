# 📊 Financial Audit Dashboard — Power BI

An interactive financial KPI dashboard built in Power BI, analysing **$276M+ in revenue** across **1,080 transactions**, **6 countries**, and **5 customer segments** over FY2013–2014.

> Built as part of a Data Analytics portfolio targeting consulting & audit roles.

---

## 🖼️ Dashboard Preview

<!-- Replace the path below with your actual screenshot filenames -->
![Executive Summary](screenshots/executive_summary.png)
![Regional Analysis](screenshots/regional_analysis.png)
![Product Analysis](screenshots/product_analysis.png)

---

## 📁 Project Structure

```
financial-audit-dashboard/
├── Financial_Dashboard.pbix        # Power BI dashboard file
├── Financial_Sample_Cleaned.xlsx   # Cleaned dataset (1,080 rows, 19 columns)
├── screenshots/
│   ├── executive_summary.png
│   ├── regional_analysis.png
│   └── product_analysis.png
└── README.md
```

---

## 🔍 Key Insights

| Insight | Finding |
|---|---|
| 💰 Total Revenue | $276M across FY2013–2014 |
| 📈 Profit Margin | 36% overall |
| 🌏 Top Market | Australia ($51.8M) |
| 🏆 Top Segment | Government (34.1% margin) |
| ⚠️ Risk Identified | High-discount band reduces margin by 12–18 pts |
| 📦 Top Product | Amarilla ($22.1M profit) |

---

## 📐 Dashboard Pages

### Page 1 — Executive Summary
- 4 KPI cards: Total Revenue, Profit, Margin %, YoY Growth
- Monthly revenue trend (2013 vs 2014 overlay)
- Sales by segment (bar chart)
- Sales by product (donut chart)
- Interactive slicers: Year, Segment, Country

### Page 2 — Regional Analysis
- Sales by country by quarter
- Profit margin % by country
- Revenue vs COGS by month
- Country KPI summary table with conditional formatting

### Page 3 — Product Deep-Dive
- Profit by product
- Units sold vs profit margin (scatter)
- Discount band impact by product (stacked bar)
- Discount rate KPI cards

---

## 🛠️ Tools & Skills

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

- **Power BI Desktop** — Dashboard design, DAX measures, drill-through
- **DAX** — Custom KPIs: YoY Growth %, Profit Margin %, Discount Rate %
- **Python (pandas)** — Data cleaning, null handling, feature engineering
- **Excel** — Source data format

---

## 📊 DAX Measures Used

```dax
Profit Margin % = DIVIDE([Total Profit], [Total Sales]) * 100

YoY Sales Growth % =
DIVIDE([Sales 2014] - [Sales 2013], [Sales 2013]) * 100

Discount Rate % =
DIVIDE([Total Discounts], SUM('Data'[Gross Sales])) * 100
```

---

## 💡 Business Recommendations

1. **Review discount approval thresholds** — High-discount transactions compress margins significantly, especially in the Channel Partners segment
2. **Expand in India & France** — Both markets show strong growth momentum with room to scale
3. **Audit Montana product pricing** — Lowest margin efficiency across all products
4. **Reduce geographic concentration** — Top 3 countries (Australia, Germany, USA) account for 52% of revenue

---

## 🚀 How to Open

1. Download `Financial_Dashboard.pbix`
2. Open with [Power BI Desktop](https://powerbi.microsoft.com/desktop) (free)
3. If prompted for data source, point to `Financial_Sample_Cleaned.xlsx` in the same folder

---

## 👤 Author

**[Your Name]**
[LinkedIn Profile URL] | [Your Email]

---

*This project is part of a 3-project Data Analytics portfolio built for consulting roles.*
