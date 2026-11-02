# Executive Summary: E-Commerce RFM Customer Segmentation

**Target Audience:** Marketing Leadership & Executive Stakeholders  
**Scope:** Analysis of 8,800 active customers across 90 days of order activity (March 16 – June 14, 2026).

---

## Business Context
To optimize marketing spend and drive customer retention, we performed an end-to-end Recency, Frequency, and Monetary (RFM) segmentation on PostgreSQL database records using Python and Pandas. This project evaluates spending distributions, quantifies customer lifecycle stages, and outlines four targeted quarterly campaign strategies.

---

## Three Key Takeaways

1. **Extreme Revenue Concentration:** 
   **22.5% of our customer base (VIP Champions) generates 65.8% of total marketplace revenue**, averaging over ₹99,300 in spend and 13+ lifetime orders. Protecting and retaining this core segment represents our highest financial leverage point.
2. **Heavy Single-Purchase Dependency:** 
   **26.9% of customers belong to the Casual & One-Timers segment**, accounting for only **2.5% of total revenue**. Converting these single-order buyers into repeat customers represents our highest-leverage acquisition-to-retention opportunity.
3. **Significant Revenue at Churn Risk:** 
   **25.2% of our base (At-Risk Spenders)** drives **14.3% of overall revenue** but has remained inactive for over 66 days. Immediate automated win-back triggers are required to prevent active revenue decay.

---

## Strategic Recommendations
* **Allocate 70% of Lifecycle Budget** toward high-ROI channels:
  * **VIP Champions:** Maintain exclusivity with early product drops and priority support rather than deep discounts.
  * **At-Risk Spenders:** Deploy time-sensitive win-back vouchers to reactivate slipping high-value customers.
* **Allocate 30% of Lifecycle Budget** to automated post-purchase onboarding sequences, driving 2nd-purchase conversion within 14 days of acquisition.

---

## Detailed Reports & Deliverables
* [01: Customer Overview One-Pager](./01_customer_overview.md)
* [02: RFM Feature Distributions](./02_rfm_distributions.md)
* [03: Segment Definitions & Campaign Brief](./03_segment_definitions.md)