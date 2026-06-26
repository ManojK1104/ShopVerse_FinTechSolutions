# 📊 Shopverse Fintech – Power BI Analytics Dashboard

> **"Shop. Save. Grow."** — A comprehensive financial analytics dashboard built for Shopverse Fintech to monitor transactions, revenue, fraud patterns, and strategic business performance.

---

## 🏢 About the Project

**Project Name:** Shopverse Fintech – Business Intelligence Dashboard  
**Tool Used:** Microsoft Power BI  
**Domain:** Fintech / Financial Analytics  
**Company:** Shopverse Fintech

Shopverse Fintech is a digital-first financial platform offering payments, savings, loans, and merchant solutions — with a strong focus on financial inclusion and underserved segments. This Power BI dashboard was built to provide a **360° business performance view** across revenue, fraud, transactions, and strategic growth metrics.

---

## 🎯 Objective

To design and deliver an end-to-end interactive Power BI dashboard that:

- Tracks **revenue, profit, and net revenue** across investor types, merchant categories, and customer segments
- Monitors **fraud activity** by type, gender, and year
- Analyzes **transaction success, failure, and pending rates**
- Provides **quarter and month-wise profit & revenue trends**
- Supports strategic decision-making through **SWOT Analysis** and **Root Cause Analysis (Fishbone)**

---

## 📌 Purpose

| Purpose | Description |
|--------|-------------|
| 📈 Financial Overview | Monitor total revenue (14.96M), profit (5.98M), success rate (0.33%), and fraud rate (5.04%) |
| 🔍 Fraud Detection | Identify fraud patterns by type (Identity Theft, Card Fraud) and by gender/year |
| 💳 Transaction Monitoring | Analyze 3T active users and transaction outcomes (33% Success / 33% Pending / 33% Failed) |
| 📊 Growth Strategy | Evaluate profit performance across Acquisition, Cost Cutting, Digital Push, and Expansion strategies |
| 🧠 Strategic Insights | SWOT Analysis and Fishbone Root Cause Analysis for business improvement |

---

## 📂 Dashboard Pages

The dashboard consists of **4 tabs**:

```
📁 Shopverse Fintech Dashboard
├── 🔵 Overview
├── 🟢 Methods
├── 🟡 SWOT Analysis
└── 🔴 RCA Fishbone
```

---

## 🖼️ Dashboard Screenshots & Explanation

### 📌 Page 1 – Overview

![Overview Dashboard](screenshots/overview.png)

**Key Metrics (KPI Cards):**
| Metric | Value |
|--------|-------|
| Active Users | 3T |
| Sum of Revenue | 14.96M |
| Sum of Profit | 5.98M |
| Success Rate % | 0.33 |
| Fraud Rate % | 5.04 |
| Average Credit Score | 600.53 |

**Visuals Included:**
- **Waterfall Chart** – Revenue, processing fee, commission fee, GST amount & net revenue by `investor_type` (VC, Angel, Government, PE)
- **Area Chart** – Quarter and month-wise revenue & profit generation (Jan–Dec across Qtr1–Qtr4)
- **Donut Chart** – Transaction amount by `transaction_status` (Failed 33.47%, Success 33.41%, Pending 33.12%)
- **Bar Chart** – Sum of revenue and profit by `merchant_category` (Retail, Food, Travel, Ecommerce)
- **Decomposition Tree** – Sum of profit broken down by gender (Male: 20.2M, Female: 19.8M, Other: 19.75M) and fraud type (None: 19.4M, Identity Theft: 28.9K, Card Fraud: 27.9K)

---

### 📌 Page 2 – Methods

![Methods Dashboard](screenshots/methods.png)

**Visuals Included:**
- **Donut Chart** – Sum of net revenue by `customer_segment` (SME: 18.02M, Corporate: 17.98M, Retail: 17.95M)
- **Area Chart** – Count of fraud by Year (2020–2025), showing a dip in 2023 (99,179) and spike in 2024 (100,160)
- **Line Chart** – Profit vs. growth strategy (Acquisition: 9001K → Cost Cutting: 8998K → Digital Push: 8960K → Expansion: 8965K)
- **Bar Chart** – Sum of transaction amount by Day (1–31), consistently ~97M–100M per day with Day 31 dipping to 58M

---

### 📌 Page 3 – SWOT Analysis

![SWOT Analysis](screenshots/swot_analysis.png)

A strategic SWOT framework for **Shopverse Fintech**:

**✅ Strengths**
- Comprehensive fintech platform (payments, savings, loans, merchant solutions)
- Strong focus on financial inclusion and underserved segments
- User-friendly digital experience with simple onboarding
- Growing partner network across banking and retail ecosystem
- Agile and innovative team with deep fintech expertise
- Data-driven decision making and analytics capabilities

**⚠️ Weaknesses**
- Low brand awareness in competitive fintech market
- High transaction failure and pending rates impacting trust
- Dependence on third-party APIs and partner systems
- Limited presence in certain regions and customer segments
- Complex policies and compliance processes causing delays
- Limited feature personalization and customization

**🚀 Opportunities**
- Rising digital adoption and demand for cashless solutions
- Expansion into rural and semi-urban markets
- Partnerships with banks, NBFCs, and fintech enablers
- Growth in e-commerce, MSMEs, and gig economy
- Leveraging AI/ML for risk assessment and personalization
- Increasing government initiatives for digital payments and financial inclusion

**🔴 Threats**
- Intense competition from established banks and fintechs
- Regulatory changes and compliance requirements
- Cybersecurity risks and data privacy concerns
- Dependence on partner reliability and system uptime
- Economic downturns affecting customer spending and repayment
- Rapid technology changes and evolving customer expectations

---

### 📌 Page 4 – RCA Fishbone (Root Cause Analysis)

![RCA Fishbone](screenshots/rca_fishbone.png)

**Problem Statement:**  
> *Why are transactions resulting in 33% success, 33% pending, and 33% failed?*

**Root Cause Categories:**

| Category | Key Causes |
|----------|-----------|
| 👥 **People** | Limited customer financial literacy, Incorrect transaction details entered, Low digital adoption, Insufficient training for support team |
| ⚙️ **Process** | Complex transaction steps, Slow KYC verification, Delays in confirmation, Unclear communication of fees and status |
| 💻 **Technology** | System downtime or slow response, Payment gateway timeouts, DB/Server performance bottlenecks, Integration failures with partner systems |
| 🤝 **Partnerships** | Bank/partner service disruptions, High failure rate from banking partners, Limited partner network in certain regions, Third-party API instability |
| 📋 **Policies** | Strict compliance checks causing delays, Frequent policy or rule changes, Risk rules blocking legitimate transactions, Limited flexibility in exception handling |
| 📣 **Marketing** | Low awareness of transaction status meanings, Unclear value communication, Excessive promotional traffic spikes, Mismatch between promises and experience |

**Outcome:**
```
33% SUCCESS  |  33% PENDING  |  33% FAILED
```

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| Microsoft Power BI | Dashboard design & data visualization |
| DAX | KPI calculations and measures |
| Power Query | Data transformation and cleaning |
| Excel / CSV | Source data |

---

## 📁 Project Structure

```
shopverse-fintech-dashboard/
│
├── 📊 ShopverseFintech.pbix        # Power BI file
├── 📁 screenshots/
│   ├── overview.png
│   ├── methods.png
│   ├── swot_analysis.png
│   └── rca_fishbone.png
├── 📁 data/
│   └── shopverse_data.csv          # Source dataset
└── 📄 README.md
```



## 📊 Key Insights

- 📌 **Equal transaction split** (33-33-33%) across success, pending, and failed indicates a critical process or technology bottleneck
- 📌 **Fraud peaked in 2024** (100,160 cases) after a significant low in 2023 (99,179)
- 📌 **PE investors** contribute the highest revenue (3.71M) among investor types
- 📌 **Retail and Food** are the top-performing merchant categories with ~3.76M and 3.74M revenue respectively
- 📌 **Acquisition strategy** yields the highest profit (9001K), while Digital Push shows the lowest (8960K)
- 📌 **Day 31 transactions** drop significantly (58M vs ~97–100M average), likely due to fewer month-end transactions

---

## 👤 Author ManojKushwaha
 [GitHub](https://github.com/yourusername)

---

## 📄 License

This project is for educational and portfolio purposes.  
© 2024 Shopverse Fintech Dashboard — All rights reserved.

---

> ⭐ If you found this project useful, please consider giving it a star!
