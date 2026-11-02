# RFM Feature Distributions & Customer Behavior Analysis

**To:** Head of Marketing  
**From:** Data Analytics  
**Subject:** Recency, Frequency, and Monetary (RFM) Distribution Findings  

## 1. Overview
To systematically identify our best customers, we engineered three core behavioral metrics across our **8,800 active buyers** using transaction data from March 16, 2026, to June 14, 2026 (with a reference date of June 15, 2026):
* **Recency ($R$):** Days elapsed since the customer's last order.
* **Frequency ($F$):** Total count of completed orders per customer.
* **Monetary ($M$):** Total spend per customer across all orders.

---

## 2. Feature Distribution Breakdown

### Recency Dynamics ($R$)
* **Data Summary:** Mean = **38.84 days** | Median = **34.00 days** | Range = **1 to 91 days** (25th percentile: 16 days; 75th percentile: 63 days).
* **Distribution Shape:** Multi-modal with strong engagement clusters. A significant peak appears under 30 days (400+ customers per bucket), followed by a secondary plateau around 65–75 days.
* **Business Takeaway:** Over 50% of active buyers purchased within the last 34 days. The visible drop-off past 60 days marks a distinct drop in engagement, defining a key threshold to trigger automated re-engagement and win-back campaigns.

### Frequency Behavior ($F$)
* **Data Summary:** Mean = **4.55 orders** | Median = **1.00 order** | Range = **1 to 178 orders** (75th percentile: 5.00 orders).
* **Distribution Shape:** Extremely right-skewed. Over 7,000 customers have placed only 1 order, while a tiny elite long-tail scales up to 178 orders.
* **Business Takeaway:** The store relies heavily on single-purchase acquisition. Shifting single-order customers into repeat buyers (orders 2–5) represents our single highest-leverage retention opportunity.

### Monetary Value ($M$)
* **Data Summary:** Mean = **₹33,949.33** | Median = **₹11,678.46** | Range = **₹175.82 to ₹1,459,762.00** (25th percentile: ₹3,773.64; 75th percentile: ₹38,243.18).
* **Distribution Shape:** Severely positive-skewed. The top 25% of customers spend above ₹38,243, while extreme outliers spend up to ₹1.46M.
* **Business Takeaway:** The mean spend (₹33,949) is triple the median spend (₹11,678) due to power spenders. Traditional average revenue metrics obscure true customer tiers, making percentile-based segment scoring necessary for upcoming clustering.

---

## 3. Executive Recommendations
1. **Automate 2nd-Purchase Onboarding:** Deploy targeted post-purchase retention sequences within 14 days of an initial order to move buyers past the 1-order hurdle.
2. **Launch a Dedicated VIP Program:** Establish an exclusive VIP tier for top-decile monetary spenders (spending > ₹38,000) to protect core revenue drivers.
3. **Set a 60-Day Win-Back Trigger:** Implement automated re-engagement offers before customers cross the 60-day recency threshold.