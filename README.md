
# 📱 Mobile Sales Dashboard | Power BI

An interactive Power BI report for exploring mobile phone sales across cities, brands, models, payment methods, and time periods. The dashboard brings sales KPIs, product comparisons, transaction analysis, and customer ratings together in a single-page view.

## Project Overview

This project presents a consolidated view of mobile sales performance through an interactive dashboard. It supports exploration of geographical sales patterns, monthly sales volumes, brand performance, popular mobile models, payment preferences, and customer feedback.

### Objectives
- Monitor headline sales and transaction metrics.
- Compare sales performance across brands and mobile models.
- Explore city-level sales contributions.
- Examine quantity trends by month and sales patterns by day of the week.
- Analyze transaction shares by payment method and customer rating counts.

## Business Questions

- Which cities contribute the most to total sales?
- Which brands and mobile models perform best within the selected filters?
- How does sales quantity vary across months?
- Which days of the week generate higher sales?
- How are transactions distributed across payment methods?
- How are customer ratings distributed?

## Key Metrics

The report includes four KPI cards:

| Metric | Purpose |
| --- | --- |
| **Total Sales** | Monitor the report's sales amount measure. |
| **Total Quantity** | Track the report's quantity measure. |
| **Transactions** | Monitor the report's transaction measure. |
| **Average** | Display the existing average measure. Its business definition should be confirmed from the DAX expression before interpretation. |

> Metric names are taken from the report. Exact DAX formulas are not reproduced here; inspect the measures in Power BI Desktop for their calculation logic.

## Dashboard Features

### Visual Analysis

| Component | Analysis |
| --- | --- |
| KPI cards | Total Sales, Total Quantity, Transactions, and Average |
| City map | Total sales by city |
| Line chart | Total quantity by month, with a day level included in the date hierarchy |
| Bar chart | Total sales by mobile model, with a Top 3 model filter configured |
| Pie chart | Transactions by payment method, with percentage labels |
| Funnel chart | Count of customer ratings by rating category |
| Area chart | Total sales by day name |
| Brand summary table | Total sales, total quantity, and transactions by brand |

### Interactive Filters

The report contains slicers for:
- **Month**
- **Mobile Model**
- **Payment Method**
- **Brand**
- **Day Name**

Use these filters to explore specific segments and compare the resulting metrics.

## Data Overview

Report visuals reference a table named `Sales_Data` and the following analysis fields:

| Field | Analytical role |
| --- | --- |
| `Date` | Time-based analysis using the date hierarchy |
| `City` | Geographic sales analysis |
| `Brand` | Brand-level comparisons |
| `Mobile Model` | Product-level comparisons |
| `Payment Method` | Payment-based transaction analysis |
| `Customer Ratings` | Customer feedback analysis |
| `Day Name` | Day-of-week sales analysis |

The original source dataset is not supplied separately in this repository structure. Source provenance, date coverage, currency, and refresh requirements should be documented before extending or republishing the project.

## Tools and Skills

- **Microsoft Power BI Desktop** — report authoring and exploration.
- **DAX measures** — sales, quantity, transaction, and average KPIs.
- **Data visualization** — maps, trend charts, comparison charts, and summary tables.
- **Interactive reporting** — slicers and filtered analysis.
- **Dashboard design** — a single-page layout with a consistent blue accent, rounded panels, and KPI icons.

## Repository Structure

```text
mobile-sales-dashboard/
├── README.md
└── Mobile Sales Dashboard.pbix
```

