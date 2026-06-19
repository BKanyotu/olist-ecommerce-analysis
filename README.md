# Olist Brazilian E-Commerce Analysis

An end to end data analytics project on the Olist Brazilian E-Commerce public dataset, covering the full path from raw database to business recommendations across two phases.

## Project Structure

**Phase 1 — SQL** (`Olist_Brazilian_Ecommerce_Data_Project_SQL.ipynb`)
Data extraction, preparation and exploratory analysis in PostgreSQL via SQLAlchemy. Covers revenue and order trends, product and category performance, delivery logistics, customer satisfaction, payment behaviour and seller performance.

**Phase 2 — Python** (`olist_brazilian_ecommerce_project_python.ipynb`)
Deeper analysis and modelling, pulling prepared data directly from the clean views built in Phase 1. Covers geospatial analysis, customer value and purchase affinity, and demand trend forecasting.

## Key Findings

- **Volume driven growth, then a plateau.** Olist grew rapidly through 2017 then levelled off across 2018 at roughly 6,000 to 7,000 orders a month, with flat average order value. Growth came from more orders, not higher spend or repeat custom.
- **A one and done platform.** 97% of customers bought only once and 96.7% of orders contained a single product. This reframed the customer analysis away from loyalty and retention toward single order value.
- **Value comes from item price, not basket size.** Even the largest orders averaged close to one product, so high value orders are single high ticket items rather than large baskets.
- **Delivery is the key weakness.** A late delivery against the promised date collapses the review score from about 4.3 to 2.3, and the harm is triggered the moment an order slips past its estimate. Lateness concentrates in the North and Northeast and rises with seller to customer distance.
- **Concentrated sellers.** The top 20% of sellers generate over 80% of platform sales.

## Important Note on Revenue

All revenue figures are gross merchandise value, the total value of sales flowing through the platform, not Olist's own earnings. Olist operates on an undisclosed commission and subscription model, so its actual income is a share of these totals that the data does not disclose.

## Tools and Methods

- **Database:** PostgreSQL
- **Languages and libraries:** SQL, Python (pandas, numpy, matplotlib, seaborn, geopandas, statsmodels, SQLAlchemy)
- **Methods:** exploratory data analysis, geospatial choropleth mapping, haversine distance analysis, RFM exploration, cohort and basket viability testing, Holt's linear trend forecasting

## Dataset

Olist Brazilian E-Commerce Public Dataset (Kaggle):
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

The dataset is anonymised to zip code prefix level, so geographic findings are regional rather than precise.


