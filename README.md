# 🛒 ShopVerse Fintech — Business Intelligence Dashboard

> **Shop. Save. Grow.** — A comprehensive Power BI analytics solution for monitoring fintech performance, fraud patterns, revenue health, and strategic growth.

---

## 📌 Project Overview

**ShopVerse Fintech Dashboard** is a multi-page Power BI report designed to provide end-to-end visibility into the financial and operational health of ShopVerse — a fintech platform offering payments, savings, loans, and merchant solutions.

This dashboard transforms raw transactional data into actionable insights across four analytical layers:
- 📊 Business **Overview** (KPIs, revenue, fraud metrics)
- 🔬 **Methods** (segment analysis, fraud trends, growth strategies)
- 🧩 **SWOT Analysis** (strategic positioning)
- 🐟 **RCA Fishbone** (root cause analysis of transaction failures)

---

## 🎯 Objective

The primary objective of this dashboard is to:

1. **Monitor core business KPIs** — active users, revenue, profit, fraud rate, and credit scores in real time.
2. **Identify revenue drivers and leakages** across investor types, merchant categories, and customer segments.
3. **Analyze fraud patterns** by type, year, and demographic to strengthen risk controls.
4. **Evaluate growth strategies** and their impact on profitability.
5. **Support root cause analysis** for the critical 33% transaction failure and 33% pending rate issue.
6. **Enable strategic decision-making** through SWOT framing and fishbone diagnostics.

---

## 🎯 Purpose

| Purpose | Description |
|---|---|
| 💰 Revenue Tracking | Monitor sum of revenue (14.96M) and profit (5.98M) across quarters and months |
| 🔐 Fraud Management | Track fraud rate (5.04%) by type — Identity Theft, Card Fraud, None |
| 👥 Investor Analysis | Compare revenue across VC, Angel, Government, and PE investor types |
| 🏪 Merchant Insights | Analyse revenue and profit by Retail, Food, Travel, and Ecommerce categories |
| 📉 Transaction Health | Diagnose the 33/33/33 split of Success / Pending / Failed transactions |
| 📈 Growth Strategy | Evaluate Acquisition, Cost Cutting, Digital Push, and Expansion strategies |
| 🧠 Strategic Review | SWOT + RCA provide a structured view of risks, opportunities, and root causes |

---

## 📸 Dashboard Snapshots

### 1. 🏠 Overview Page

![Overview Dashboard](./assets/overview.png)

**What it shows:**

The Overview page is the command center of the ShopVerse dashboard. It surfaces the most critical KPIs at the top:

| KPI | Value |
|---|---|
| Active Users | 3T |
| Sum of Revenue | 14.96M |
| Sum of Profit | 5.98M |
| Success Rate % | 0.33 |
| Fraud Rate % | 5.04 |
| Avg. Credit Score | 600.53 |

**Key visuals:**
- **Revenue by Investor Type** — A bar chart breaking down revenue contributions from VC, Angel, Government, and PE investors. Total sum reaches 14.96M, with PE contributing the majority.
- **Quarter & Month Revenue vs Profit** — A dual-line chart showing consistent revenue (~1.2–1.3M/month) with profit (~0.5M/month), across all 4 quarters.
- **Transaction Status Donut** — The 33/33/33 split between Failed, Success, and Pending highlights a major operational challenge.
- **Revenue & Profit by Merchant Category** — Retail, Food, Travel, and Ecommerce each contributing ~1.5M in revenue and ~1.7–1.74M in profit.
- **Gender-wise Profit Breakdown** — Male: 20.20M | Female: 19.81M | Other: 19.75M — near-equal distribution.
- **Fraud Type Breakdown** — None: 15.4M | Identity Theft: 28,945 | Card Fraud: 27,907.

---

### 2. 🔬 Methods Page

![Methods Dashboard](./assets/methods.png)

**What it shows:**

The Methods page dives into customer segmentation, fraud trend analysis, growth strategy performance, and daily transaction patterns.

**Key visuals:**
- **Net Revenue by Customer Segment (Donut)** — Three segments: SME (~17.95M), Corporate (~18.02M), and Retail (~17.98M) — showing balanced revenue distribution across segments.
- **Count of Fraud by Year (Line Chart)** — Fraud peaked at **1,00,064 in 2020**, dipped to **98,178 in 2024**, then spiked again to **1,01,260 in 2025**, indicating an emerging fraud resurgence requiring immediate attention.
- **Profit by Growth Strategy (Bar Chart)** — Acquisition and Cost Cutting deliver the highest profits (~9001K), while Expansion shows the lowest (~8965K), suggesting early-stage investment drag.
- **Transaction Amount by Day** — Daily transaction volumes fluctuate between 68M–100M, with visible dips around days 20–25, possibly reflecting weekend or billing cycle effects.

---

### 3. 🧩 SWOT Analysis Page

![SWOT Analysis](./assets/swot.png)

**What it shows:**

A structured strategic snapshot of ShopVerse Fintech's competitive position.

| Quadrant | Highlights |
|---|---|
| ✅ **Strengths** | Comprehensive fintech platform (payments, savings, loans, merchants); strong financial inclusion focus; data-driven decision making; agile team with deep fintech expertise |
| ⚠️ **Weaknesses** | Low brand awareness; high transaction failure & pending rates; dependence on third-party APIs; limited regional presence; complex compliance processes |
| 🚀 **Opportunities** | Rising digital adoption; rural/semi-urban market expansion; partnerships with banks & NBFCs; AI/ML for personalization; government digital payment initiatives |
| 🔴 **Threats** | Intense competition from established banks; regulatory changes; cybersecurity risks; economic downturns impacting repayment; rapid tech evolution |

---

### 4. 🐟 RCA Fishbone Page

![RCA Fishbone](./assets/rca_fishbone.png)

**What it shows:**

A Root Cause Analysis (Fishbone / Ishikawa) diagram addressing the central problem:

> **"Why are transactions resulting in 33% success, 33% pending, and 33% failed?"**

Six root cause categories are mapped:

| Category | Root Causes |
|---|---|
| 👥 **People** | Limited customer financial literacy; incorrect transaction details; low digital adoption; insufficient support training |
| ⚙️ **Process** | Complex transaction steps; slow KYC verification; confirmation delays; unclear fee communication |
| 💻 **Technology** | System downtime; payment gateway timeouts; DB/server bottlenecks; partner integration failures |
| 🤝 **Partnerships** | Bank/partner disruptions; high failure rate from partners; limited regional partner network; third-party API instability |
| 📋 **Policies** | Strict compliance causing delays; frequent policy changes; risk rules blocking legitimate transactions; limited exception handling flexibility |
| 📣 **Marketing** | Low awareness of transaction status meanings; unclear value communication; excessive promotional traffic spikes; mismatch between promises and user experience |

---

## 🗂️ Repository Structure

```
shopverse-fintech-dashboard/
│
├── 📁 assets/
│   ├── overview.png
│   ├── methods.png
│   ├── swot.png
│   └── rca_fishbone.png
│
├── 📁 data/
│   └── shopverse_data.csv        # Source dataset (if shareable)
│
├── 📁 reports/
│   └── ShopVerse_Dashboard.pbix  # Power BI report file
│
├── README.md
└── LICENSE
```

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design and data visualization |
| **DAX** | Custom measures for KPIs, fraud rate, success rate |
| **Power Query (M)** | Data cleaning and transformation |
| **Excel / CSV** | Source data format |

---

## 📊 Key Metrics Summary

| Metric | Value |
|---|---|
| Active Users | 3 Trillion |
| Total Revenue | ₹14.96M |
| Total Profit | ₹5.98M |
| Success Rate | 33% |
| Fraud Rate | 5.04% |
| Avg. Credit Score | 600.53 |
| Peak Fraud Year | 2025 (1,01,260 cases) |
| Best Growth Strategy | Acquisition / Cost Cutting (~9001K profit) |

---

## 💡 Key Insights

- 🔴 **Transaction Health is Critical** — A 33% failure rate and 33% pending rate means only 1 in 3 transactions succeeds. The RCA identifies technology, process, and partnership gaps as primary causes.
- 📈 **Revenue is Consistent** — Monthly revenue holds steady at ~1.2–1.3M across all quarters, showing platform stability despite operational challenges.
- 🕵️ **Fraud is Rising Again** — After declining in 2023–2024, fraud counts are spiking in 2025. Identity theft and card fraud need targeted intervention.
- 🧩 **Segments are Balanced** — SME, Corporate, and Retail contribute nearly equally to net revenue (~18M each), suggesting no over-reliance on a single segment.
- 🚀 **Expansion Strategy Underperforms** — Compared to Cost Cutting and Acquisition, Expansion yields the lowest profit, likely due to upfront investment costs.

---



## 👤 Author

**[Manoj kushwaha]**
Data Analyst | Power BI Developer
📧 manojrkushwaha85@gmail.com
🔗 ManojK1104

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](./LICENSE) for details.

---

> *"Data is the new currency. ShopVerse turns transactions into intelligence."*
