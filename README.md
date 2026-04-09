# E-commerce-Revenue-Leakage-Pipeline
An end-to-end Python pipeline to identify financial loss in e-commerce. Unifies 6 data silos to isolate 'Revenue Killer' products and operational failures.


# E-commerce Revenue Leakage & Return Optimization Pipeline

## 📌 Project Overview
This project addresses a critical business struggle: **Revenue Leakage**. By analyzing 100k+ records from the Olist Brazilian E-commerce dataset, I built an end-to-end pipeline to identify why orders are being canceled and which products are "Revenue Killers."

## 🚀 How to Run
1. Clone this repository.
2. Download the Olist Dataset from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?resource=download).
3. Ensure you have `pandas` installed: `pip install pandas`.
4. Run `returns_analysis_pipeline.py`.

## 🛠️ The Data Pipeline (CRUD Logic)
I unified 6 fragmented data silos into a single analytical engine:
- **Orders & Items:** Linked transaction status to financial value.
- **Products & Translations:** Categorized "problem areas" into English for stakeholder reporting.
- **Reviews:** Connected 1-star sentiments to canceled orders to find the "Smoking Gun."

## 🔍 Key Business Insights
- **Financial Leakage:** Quantified revenue lost to 'Canceled' vs 'Unavailable' orders.
- **The "Hit List":** Discovered specific products with a **100% cancellation rate** and a **1.0 average review score**.
- **Root Cause:** Identified that "Unavailable" items (Operational Failure) drive the lowest customer satisfaction (1.5/5.0 stars).
