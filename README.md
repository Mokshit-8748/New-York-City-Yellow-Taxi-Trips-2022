# NYC Yellow Taxi Trips 2022 – Tableau Dashboard

This repository contains a comprehensive Tableau dashboard analyzing the New York City Yellow Taxi trip data for 2022, as well as the datasets, SQL queries, and essential source files used in the project.

## Overview

This project provides actionable insights into NYC’s yellow taxi ecosystem for 2022. By leveraging detailed trip data, we identify passenger trends, payment methods, tipping behavior, and key performance indicators. Visualizations and datasets are designed for urban mobility stakeholders such as city planners and transportation policymakers.

## Repository Contents

- **/data/**
  - `Unified_dataset.csv` – Summary KPIs by passenger bucket (trips, fares, tips).
  - `detailed-dataset.csv`– Full trip segmentation (by hour, payment, tipping bucket, etc.).
  - `top-10-trips.csv`– Top 10 longest trip records with all features.
- **/assets/**
  - `dashboard_snapshot.jpg`-<img width="1590" height="795" alt="Screenshot 2025-08-03 214134" src="https://github.com/user-attachments/assets/982b6def-19ec-413a-aba9-b8d8626b4946" />

- **/tableau/**
  - `NYC_Yellow_Taxi_2022.twb` – Tableau workbook file with all visualizations.
- **/queries/**
  - `unified_dataset_query.sql` – SQL used for KPIs.
  - `detailed_dataset_query.sql` – SQL for breakdowns (segmentation; time, payment, tip).
  - `top_10_trips_query.sql` – SQL for longest trip analysis.

## How to Use

1. **Explore the Dashboard**  
   Open the `.twb` file in Tableau Desktop or Tableau Public. You’ll find dashboard covering multiple KPIs, passenger and trip segmentation, payment methods, tipping analysis, and top trips.

2. **Review & Reproduce Analyses**  
   - Each chart/metric is powered by the included CSV datasets.  
   - To ensure transparency, all SQL queries used to extract and shape these datasets are provided in `/queries/`.  
   - Data source slides and visual footnotes in the dashboard indicate which dataset/query powers each analytic section.

3. **Dashboard Features**  
   - **Core KPIs**: Aggregated by passenger bucket.  
   - **Segmentation by hour and payment**: Detailed breakdowns for trip distribution and fare/tip analysis.  
   - **Tipping Patterns**: Distribution across defined percentage buckets.  
   - **Top 10 Trips**: Outlier and long-distance trip inspection.

## Key Insights & Takeaways

- **Solo riding is dominant**: Single-passenger trips account for most rides and revenue.  
- **Credit cards rule**: The vast majority of fares are paid with cards, especially for higher-value and higher-tip rides.  
- **Tips skew low**: Most tips fall into the 0–5% range, with only a small subset exceeding 20%.  
- **Peak travel hours**: Demand is highest during evening rush (5–8 PM); early morning hours are lowest.  
- **Long trips are rare, but impactful**: Most rides are short or moderate; the top 10 longest trips are significant outliers and contribute disproportionately to revenue.  
- **Segmented insights**: Both fare and tipping percentages are higher for solo and two-passenger trips compared to larger groups.

## Prerequisites

- [Tableau Desktop](https://www.tableau.com/products/desktop) or [Tableau Public](https://public.tableau.com/)  
- BigQuery or another SQL platform for custom data extraction

## Recreating / Extending the Analysis

1. **SQL Extraction:** Use the provided queries in `/queries/` to re-extract the most recent data from BigQuery or your data warehouse.  
2. **Data Update:** Replace or append to the CSVs in `/data/` as needed.  
3. **Dashboard Customization:** Open the Tableau workbook and refresh data sources or customize visuals.

## Attribution

- Data source: NYC TLC Yellow Taxi Trips (BigQuery Public Dataset)  
- Dashboard and analysis by: Mokshit-8748

## License

This project is licensed under the MIT License.


## Acknowledgements

- NYC Taxi & Limousine Commission – original data provider.  
- Tableau Public and community support for dashboard best practices.

---

**Questions or feedback?**  
Your feedback is always welcome! Please open an issue or reach out to the maintainer with any questions or suggestions.

> *For maximum transparency, this repository includes raw data, all transformation queries, and the exact dashboard snapshot as used in analysis. You are encouraged to fork, adapt, or extend with your own NYC taxi data explorations!*
