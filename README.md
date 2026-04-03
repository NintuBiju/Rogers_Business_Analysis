# Rogers Canada — Subscriber Analytics 2026

**End-to-end data analytics project** covering exploratory analysis, diagnostic churn modelling, revenue growth analysis, and an interactive Tableau dashboard — built on a simulated dataset of 300,000 Rogers Canada subscribers (2020–2025).

---

## 📊 Live Tableau Dashboard

🔗 [View Interactive Dashboard](https://public.tableau.com/app/profile/nintu.biju/viz/RogersSubscriberAnalyticsDashboard2026/Dashboard1)

---

## 🗂️ Project Structure

```
rogers-subscriber-analytics/
│
├── README.md
├── notebooks/
│   └── Rogers_Data_Analysis_2026_final.ipynb   ← Full Python analysis (4 phases)
└── data/
    ├── tableau_01_kpi_summary.csv
    ├── tableau_02_churn_by_region.csv
    ├── tableau_03_churn_by_tier.csv
    ├── tableau_04_churn_by_bundle.csv
    ├── tableau_05_monthly_trend.csv
    ├── tableau_06_support_vs_churn.csv
    ├── tableau_07_billing_impact.csv
    ├── tableau_08_card_analysis.csv
    ├── tableau_09_channel_performance.csv
    └── tableau_10_revenue_risk_matrix.csv
```

---

## 🔍 Project Overview

### Dataset
- **300,000 simulated Rogers Canada subscriber records** (2020–2025)
- 16 features: Region, Loyalty Tier, Bundle Type, Sales Channel, Device Type, Billing Grievances, Support Interactions, Network Reliability Score, Credit Card Status, Monthly ARPU, Churn flag
- Overall churn rate: **4.43%** | Average ARPU: **$115.06/month**

---

## 📈 Analysis Phases

### Phase 1 — Exploratory Data Analysis (EDA)
Column-by-column analysis of all 16 features. Key findings:
- 300K subscribers across 4 regions (Ontario 45%, West 35%, Atlantic 12%, Quebec 8%)
- Classic loyalty pyramid: Silver 60% → Gold 30% → Platinum 10%
- Retail Store dominates acquisition (50%), followed by Online/App (35%)

### Phase 2 — Diagnostic Analysis (Why Are Customers Leaving?)

| Driver | Finding |
|--------|---------|
| Billing Grievances | **3.5x churn multiplier** — customers with billing issues churn at 29.6% vs 8.4% baseline |
| Support Interactions | **Tipping point at 3+ calls** — churn jumps from 4% to 7%+ and climbs to 20% at 8 calls |
| Network Reliability | Counter-intuitive: NOT a primary churn driver — scores are identical for churned vs retained |
| Device Type | BYOD customers churn slightly more — financing is not creating expected switching cost |
| Bundle Type | Churn is similar across bundles — systemic issue, not product-specific |
| Loyalty Tier | Churn is flat across Silver/Gold/Platinum — loyalty program is NOT protecting high-value customers |

### Phase 3 — Revenue Growth Analysis

| Opportunity | Finding |
|------------|---------|
| Bundle Upsell | Ultimate TV ($158 ARPU) vs App TV ($84 ARPU) — 88% ARPU gap, clear upgrade opportunity |
| Credit Card Cross-Sell | Only 25% of customers have a Rogers card — massive cross-sell headroom |
| Regional Concentration | Ontario drives the largest revenue but also the highest revenue at risk |
| CLV Optimization | Top 20% of customers by CLV are on Ultimate TV + Platinum tier + has Rogers card |

### Phase 4 — Strategic Recommendations
1. **Billing Fix First** — resolve billing grievances to cut churn by up to 3.5x for affected customers
2. **Support Trigger System** — flag customers at 3+ support interactions for proactive retention outreach
3. **Bundle Upsell Campaign** — target Internet Only and App TV customers for upgrade to Ultimate TV
4. **Credit Card Cross-Sell** — prioritize Silver-tier customers without a Rogers card (largest addressable segment)
5. **Ontario + Popular TV** — highest revenue at risk cell ($3.36M) — needs dedicated retention campaign

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Pandas, NumPy) | Data generation, EDA, diagnostic analysis |
| Matplotlib, Seaborn | Exploratory visualizations |
| Tableau Public | Interactive executive dashboard |
| Google Colab | Development environment |
| GitHub | Version control & portfolio |

---

## 📊 Dashboard Views

The Tableau dashboard includes 5 views:

1. **Churn by Region** — Geographic churn distribution (bar chart)
2. **Churn by Loyalty Tier** — Tier performance with Revenue at Risk labels
3. **Bundle Performance** — ARPU ladder colored by churn rate
4. **Support Tipping Point** — Line chart with Danger Zone reference line at 3 interactions
5. **Revenue Risk Heatmap** — Region × Bundle matrix showing revenue at risk per segment

---

## 🚀 How to Run

1. Open `notebooks/Rogers_Data_Analysis_2026_final.ipynb` in Google Colab
2. Run all cells sequentially (runtime ~3–5 minutes for 300K rows)
3. The notebook generates the master dataset and all Tableau-ready CSVs automatically
4. View the live dashboard at the link above

---

## 👤 Author

**Nintu Biju**
[Tableau Public Profile](https://public.tableau.com/app/profile/nintu.biju)

---

*This project was built as a portfolio piece demonstrating end-to-end data analytics skills: data engineering, exploratory analysis, diagnostic modelling, and business intelligence visualization.*
