# SQL_Project1_Instacart

Project: Instacart SQL + DA/FA/BA practice
Purpose: reproducible SQL pipeline that produces business & financial proxies (KPIs, cohort/retention, RFM, basket analysis) and a simple prediction prototype (user*product next-order label).

## Overview & Primary Goal
Build a repeatable, SQL-first data-product pipeline from the Instacart dataset that delivers:
- Descriptive business insights (product / category / user KPIs, basket behavior)
- Actionable BA outputs (RFM segments, cohort retention, cross-sell candidates)
- FA-style proxies (CLTV / ARPU proxies via price assumptions or mapping)
- A simple DA model prototype: predict whether a user will buy a product in their next order (classification)

All outputs are exportable CSVs and ready for light Python modeling & visualization.

## Quantifiable Sub-goals (deliverables & success criteria)
- ETL completeness — Import tables + create indexes. Success: row counts match CSVs.
- Product / Category KPIs — product_kpis.csv, aisle_kpis.csv, department_kpis.csv. Success: top-20 products exported, reorder_rate computed.
- User RFM & segments — user_rfm.csv and summary rfm_summary.csv. Success: segmented groups show distinct avg_orders.
- Cohort retention — cohort_retention.csv (0..12 periods) + heatmap-ready CSV. Success: retention matrix generated and validated.
- Basket co-occurrence — product_pairs_topN.csv (support, lift). Success: top 50 pairs exported.
- ML dataset + baseline model — ml_dataset.csv and model report (AUC, Precision@K). Success: model beats popularity baseline.
- FA proxies / CLTV — cltv_proxy.csv under two price-assumption scenarios. Success: cohort-level CLTV table exported.
