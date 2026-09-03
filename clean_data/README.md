# Cleaned Data

This project reuses the cleaned dataset produced in my [Olist E-Commerce BI Pipeline](https://github.com/Nkanyisogwane/olist-ecommerce-bi-pipeline) project rather than re-cleaning the raw Olist data from scratch.

## Why reuse instead of re-clean

The BI Pipeline project already performed the full cleaning process — deep cleaning on the central `orders` table, lighter cleaning on supporting tables, flagging (rather than deleting) problematic rows, and documenting each decision. Repeating that process here would be redundant and wouldn't add anything to this project's actual goal: demonstrating statistical and data science methodology on top of a dataset that's already analysis-ready.

## Where to get the data

The cleaned CSVs are available in the BI Pipeline repo:
👉 [github.com/Nkanyisogwane/olist-ecommerce-bi-pipeline](https://github.com/Nkanyisogwane/olist-ecommerce-bi-pipeline)

To reproduce this notebook, download the cleaned CSVs from that repo's data folder and place them here, in this `clean_data/` folder, before running `olist_stats_deepdive.ipynb`.

## Tables used in this project

| File | Rows | Used for |
|---|---|---|
| `orders_clean.csv` | 99,441 | All phases — delivery timing, order status |
| `order_reviews_clean.csv` | 99,224 | Phase 1, 2 — review scores |
| `customers_clean.csv` | 99,441 | Phase 3, 4 — unique customer identification (`customer_unique_id`) |
| `order_payments_clean.csv` | 103,886 | Phase 3, 5 — monetary value, revenue |

See the main [BI Pipeline README](https://github.com/Nkanyisogwane/olist-ecommerce-bi-pipeline) for full documentation of the original cleaning process, including flagged-row logic and schema design.
