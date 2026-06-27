# 🛒 eCommerce Customer Segmentation — RFM Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

A full end-to-end customer segmentation project on an eCommerce transaction dataset, using **RFM Modelling**, **Decile Analysis**, and data-driven **Marketing Strategy** recommendations.

---

## 📌 Project Overview

Most eCommerce businesses generate vast transactional data but struggle to translate it into actionable segments. This project addresses that gap by:

- Scoring every customer on **Recency**, **Frequency**, and **Monetary** value
- Grouping customers into 5 named segments (Champions → Dormant)
- Ranking all customers into **10 revenue-based deciles**
- Producing a **budget allocation framework** and per-tier marketing strategies

> **Key finding:** The top 10% of customers (Decile 1) drive **28.4% of total revenue**. The top 3 deciles together account for over **53%** — a classic Pareto distribution.

---

## 📊 Dashboards Generated

| Dashboard | Description |
|-----------|-------------|
| `rfm_dashboard_1.png` | Overview — KPIs, segment donut, sales distribution, decile bar chart, cumulative revenue curve |
| `rfm_dashboard_2.png` | Deep Dive — RFM heatmap (R × F → £), avg frequency per segment, avg monetary per segment |
| `rfm_dashboard_3.png` | Strategy View — full decile table, top countries by avg sale, budget allocation pie, RFM score histogram, actionable strategies |
| `rfm_dashboard_4.png` | Scatter plot — Frequency vs Monetary coloured by segment |

---

## 🧠 RFM Methodology

Each customer is scored **1–5** on three dimensions:

| Dimension | Definition | High Score = |
|-----------|-----------|--------------|
| **Recency (R)** | Days since last purchase | Bought very recently |
| **Frequency (F)** | Number of transactions | Buys often |
| **Monetary (M)** | Total spend (£) | High lifetime value |

Scores are summed into a composite **RFM Score (3–15)** and mapped to segments:

| RFM Score | Segment |
|-----------|---------|
| 13–15 | 🏆 Champions |
| 10–12 | ⭐ Loyal Customers |
| 8–9 | 🌱 Potential Loyalists |
| 6–7 | ⚠️ At-Risk Customers |
| 3–5 | 💤 Dormant / Lost |

---

## 📈 Key Results

| Metric | Value |
|--------|-------|
| Active Customers | 300 |
| Total Revenue | £146,843 |
| Avg Transaction Frequency | 35.4 |
| Avg Customer Spend | £489 |
| Champions avg spend | £2,150 |
| Dormant avg spend | £210 |
| D1 revenue contribution | 28.4% |
| Top 3 deciles combined | 53.7% |

---

## 💡 Recommendations Summary

| Tier | Strategy |
|------|----------|
| **Champions (D1–D2)** | VIP loyalty programme, early access, referral incentives |
| **Loyal (D3–D4)** | Tiered membership upsell, cross-sell, personalised emails |
| **Potential (D5–D6)** | Limited-time bundles, frequency rewards, gamified points |
| **At-Risk / Dormant (D7–D10)** | Win-back campaigns, "we miss you" coupons, reactivation surveys |

### Recommended Marketing Budget Split

```
Champions   ████████████████  40%
Loyal       ██████████        25%
Potential   ████████          20%
Re-engage   ██████            15%
```

---

## 🗂️ Repository Structure

```
ecommerce-rfm-segmentation/
│
├── Ecommerce_Project.ipynb     ← Main analysis notebook
├── requirements.txt            ← Python dependencies
├── .gitignore                  ← Files excluded from git
├── README.md                   ← This file
│
└── outputs/                    ← Generated charts & reports
    ├── rfm_dashboard_1.png
    ├── rfm_dashboard_2.png
    ├── rfm_dashboard_3.png
    ├── rfm_dashboard_4.png
    └── RFM_Analysis_Report.xlsx
```

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/YOUR_USERNAME/ecommerce-rfm-segmentation.git
cd ecommerce-rfm-segmentation
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

```bash
jupyter notebook Ecommerce_Project.ipynb
```

All four dashboards and the Excel report will be saved automatically to the `outputs/` folder.

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **Pandas** — data wrangling, RFM calculation, decile grouping
- **NumPy** — numerical operations
- **Matplotlib** — all visualisations (no Seaborn dependency)
- **OpenPyXL** — Excel export
- **Jupyter Notebook** — interactive analysis environment

---

## 👩‍💻 About

**Lisha Bhowmik** — BBA Graduate & Data Analyst  
Passionate about turning raw transactional data into marketing intelligence.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin)](https://linkedin.com/in/YOUR_PROFILE)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?logo=github)](https://github.com/YOUR_USERNAME)

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
