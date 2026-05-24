# Financial Audit Dashboard — Power BI

I built this dashboard to explore financial performance data across 6 countries and 5 customer segments over FY2013–2014. I wanted to go beyond just numbers and find patterns that would actually mean something — things like where margins were quietly eroding or which markets were punching above their weight.

---

## Screenshots

![Executive Summary](screenshots/executive_summary.png)
![Regional Analysis](screenshots/regional_analysis.png)
![Product Analysis](screenshots/product_analysis.png)

---

## What I built

The dashboard has 3 pages, each answering a different question:

- **Executive Summary** — where does the business stand overall? KPIs, trends, and a segment breakdown at a glance
- **Regional Analysis** — which countries are actually profitable, not just high-revenue?
- **Product Deep-Dive** — which products are worth pushing, and where is discounting hurting us?

---

## What I found

A few things stood out once the data was cleaned up and visualised properly. Australia led in revenue but the margins told a different story at the country level. The Government segment was consistently the most profitable. And high-discount transactions were quietly compressing margins by 12–18 percentage points — something that's easy to miss without looking at it visually.

---

## Tools used

Power BI Desktop for the dashboard, Python (pandas) to clean and prep the data, and Excel as the source file.

---

## How to open it

Download `Financial_Dashboard.pbix` and open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop). If it asks for the data source, just point it to `Financial_Sample_Cleaned.xlsx` in the same folder.
