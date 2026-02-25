# E-Commerce Funnel & KPI Analytics

End-to-end e-commerce analytics project using GA4 BigQuery sample data.  
This project covers SQL data modeling, Tableau dashboard visualization, and advanced Python analysis including revenue decomposition and conversion impact modeling.

---

## 📊 Executive Summary

This project analyzes user behavior across an e-commerce funnel to understand:

- What drives revenue?
- Where does the funnel leak?
- How did post-holiday performance change?
- Which device segment offers the highest optimization ROI?

Key results:

- **Total Revenue:** $362,165  
- **Overall Conversion Rate:** 7.21%  
- **Funnel Entry Users (Viewed):** 61,252  
- **Average Order Value (AOV):** ~$82  

Revenue peaked during early–mid December (holiday period), followed by a 72% decline post-holiday, primarily driven by conversion rate deterioration.

---

## 🧱 Project Architecture

**Data Source:** GA4 BigQuery public sample dataset  

**Workflow:**
1. SQL modeling in BigQuery (funnel stages + KPI tables)
2. Tableau dashboard for executive visualization
3. Python deep-dive analysis for:
   - Trend smoothing (7-day rolling averages)
   - Funnel stage drop-off analysis
   - Revenue decomposition modeling
   - Device conversion impact simulation

---

## 📈 Dashboard Preview

![Dashboard](dashboard/ecommerce_dashboard.png)

The dashboard highlights:
- Revenue & Conversion trends
- Funnel stage distribution
- Device conversion comparison
- Executive KPI summary

---

## 🔍 Key Analytical Findings

### 1️⃣ Revenue Drivers

Correlation analysis shows revenue is most sensitive to:

- Conversion Rate (0.83)
- Traffic Volume (0.73)
- AOV (0.60)

Conversion rate is the strongest revenue lever.

---

### 2️⃣ Holiday vs Post-Holiday Decline

Post-holiday performance change:

- Revenue: -72.6%
- Conversion Rate: -47%
- Users: -34%
- AOV: -25%

The primary driver of revenue decline was conversion rate deterioration.

---

### 3️⃣ Funnel Drop-Off Analysis

Stage Conversion Rates:

- View → Cart: 20.48%
- Cart → Checkout: 77.44%
- Checkout → Purchase: 45.49%
- Overall Funnel: 7.21%

Largest leakage occurs at **View → Cart**, indicating potential issues in:
- Product page engagement
- Pricing perception
- Traffic quality

---

### 4️⃣ Device Optimization Impact Model

Simulation: +1% absolute improvement in mobile conversion

- Current Revenue: $362,165
- Projected Revenue: $382,210
- Estimated Revenue Lift: **+$20,045**

Mobile conversion improvement represents a high-ROI optimization opportunity.

---

## 🧪 Python Deep-Dive Analysis Includes

- 7-day rolling revenue & conversion smoothing
- Correlation heatmap
- Revenue decomposition modeling
- Peak vs Post-period performance comparison
- Funnel stage efficiency metrics
- Device-level weighted conversion modeling

Notebook available here:

📓 `notebook/01_funnel_deep_dive.ipynb`

---

## 📁 Project Structure

```text
ecommerce-funnel-analytics/
│
├── dashboard/
│   └── ecommerce_dashboard.png
│
├── data/
│   ├── daily_kpis.csv
│   ├── funnel_summary.csv
│   └── device_conversion.csv
│
├── figures/
│
├── notebook/
│   └── 01_funnel_deep_dive.ipynb
│
├── README.md
└── LICENSE
```

---

## 🚀 Strategic Recommendations

1. Improve View → Cart conversion via product page optimization.
2. Prioritize mobile UX improvements (high revenue elasticity).
3. Run post-holiday re-engagement campaigns to stabilize conversion.
4. Monitor conversion deterioration more aggressively than traffic changes.

---

## 🛠 Tech Stack

- Google BigQuery (SQL modeling)
- Tableau Public (Dashboard Visualization)
- Python (Pandas, NumPy, Matplotlib)
- Jupyter Notebook

---

## 👤 Author

Kaustubh Gaikwad  
M.S. Business Analytics & Artificial Intelligence  
University of Texas at Dallas  
 
