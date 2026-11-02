# E-Commerce Customer Segmentation & Revenue Analysis

An end-to-end data analytics project establishing customer behavioral baselines, feature engineering Recency, Frequency, and Monetary (RFM) metrics, and profiling actionable target segments for marketing campaign optimization.

![RFM Segment Revenue Concentration](./rfm_revenue_concentration.png)

---

## Executive Overview
Analyzing 8,800 active e-commerce customers across a 90-day operational window revealed significant revenue skewness. Using quantile-based RFM scoring and rule-based segmentation, we categorized the customer base into four strategic cohorts:
* **VIP Champions (22.5% base | 65.9% revenue):** High-touch, frequent buyers averaging ₹99,315 in spend.
* **Loyal Regulars (25.4% base | 17.4% revenue):** Steady repeat shoppers averaging 3.07 orders.
* **At-Risk Spenders (25.2% base | 14.3% revenue):** High-value historical spenders inactive for >66 days.
* **Casual & One-Timers (26.9% base | 2.5% revenue):** Single-purchase buyers with minimal monetary contribution.

For the full executive write-up and strategic campaign breakdown, see the [Executive Summary](./findings/00_executive_summary.md).

---

## Project Structure
```text
├── findings/
│   ├── 00_executive_summary.md     # Executive synthesis & core takeaways
│   ├── 01_customer_overview.md      # Milestone 2: Baseline customer overview
│   ├── 02_rfm_distributions.md     # Milestone 3: RFM feature distribution analysis
│   └── 03_segment_definitions.md   # Milestone 4: Segment profiling & campaign brief
├── notebooks/
│   ├── 01_exploration.ipynb        # Data ingestion & initial EDA
│   ├── 02_rfm_features.ipynb       # RFM feature extraction & distribution checks
│   └── 03_segment_segments.ipynb   # Quantile scoring & customer segmentation
├── rfm_revenue_concentration.png   # Embedded visualization
├── requirements.txt                # Python dependencies
└── README.md                       # Project overview & documentation

Tech Stack & Data Architecture
Database: Cloud PostgreSQL (Neon)

Data Processing & Analytics: Python 3.10+, Pandas, NumPy

Visualization: Seaborn, Matplotlib

Database Driver: pg8000 (Pure-Python SSL database connection)