# 🏦 Bank Customer Churn Analysis

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

An end-to-end Business Analytics project analysing 10,000 bank customers
to identify why 20.37% of them are churning — and what the bank should do about it.

The project follows a structured BA workflow: data exploration to find broad patterns,
deep segment analysis to isolate root causes, and prioritised business recommendations
for the retention team.

---

## 🎯 Business Problem

> *"The bank is losing 1 in 5 customers. We do not know who is leaving,
> why they are leaving, or where to focus our retention efforts."*

This project answers three questions:
- **Who** is leaving?
- **Why** are they leaving?
- **What** should the bank do about it?

---

## 🔑 Key Findings

| Finding | Detail |
|---|---|
| Overall churn rate | 20.37% — roughly double the industry benchmark |
| Highest churn country | Germany at 32.44% — double France and Spain |
| Highest churn age group | 51-60 at 56.21% — more than half left |
| Product sweet spot | 2 products = 7.58% churn (lowest) |
| Most dangerous segment | 3-4 products = 82-100% churn |
| Balance finding | Churned customers hold Rs. 18,363 more on average |
| Funnel 1 max risk | Germany + Inactive + 41-60 + 3-4 Products = **94.87% churn** |
| Funnel 2 max risk | Inactive + 41-60 + 3-4 Products (global) = **95.28% churn** |

---

## 🔬 Analytical Approach

### Segment Decomposition Framework

Two analytical funnels were built using a method called Segment Decomposition —
starting with a high-level finding and progressively narrowing by one variable
at a time to identify the most precise high-risk customer profile.

**Funnel 1 — Germany Deep Dive**
```
Overall (20.37%)
→ Germany (32.44%)
→ Germany + Age 41-60 (54.29%)
→ Germany + Inactive + 41-60 (64.47%)
→ Germany + Inactive + 41-60 + 3-4 Products (94.87%) ← 4.7x overall
```

**Funnel 2 — Age Group Deep Dive**
```
Overall (20.37%)
→ Age 41-60 (39.65%)
→ Inactive + Age 41-60 (51.09%)
→ Inactive + 41-60 + 3-4 Products (95.28%) ← 4.7x overall
```

Both funnels independently arrive at the same conclusion —
over-selling products to inactive older customers is the
single biggest driver of churn, regardless of geography.

---

## 📊 Project Workflow
```
Dataset → Exploration → Deep Analysis → Dashboard → Report → Recommendations
```

| Phase | Description | Tool |
|---|---|---|
| Phase 1 — Exploration | 9 business questions answered | Python · Pandas · Seaborn |
| Phase 2 — Cleaning | Verified clean — no action needed | Python |
| Phase 3 — Deep Analysis | 2 analytical funnels built | Python · Pandas |
| Phase 4 — Dashboard | 2-page interactive dashboard | Power BI |
| Phase 5 — Report | Full business analytics report | Word |

---

## 📁 Repository Structure
```
Bank-Customer-Churn-Analysis/
│
├── 📁 notebook/
│   └── Banking_churn.ipynb       ← Full Python analysis
│
├── 📁 dataset/
│   └── Bank_Churn.csv            ← Raw dataset
│
├── 📁 insights/
│   └── Bank_Churn_Report.docx    ← Business analytics report
│
├── 📁 visuals/
│   ├── Bank_Churn_Dashboard.pbix ← Power BI source file
│   └── Bank_Churn_Dashboard.pdf  ← Dashboard PDF export
│
└── 📄 README.md
```

---

## 💡 Top Recommendations

### 🔴 Immediate
1. **Audit all 3-4 product customers** — review product relevance and fee burden
2. **Launch Germany retention programme** — assign dedicated relationship managers
3. **Re-engage inactive 41-60 customers** — personalised outreach before they exit

### 🟠 Short Term
4. **Stop cross-selling beyond 2 products** without a clear customer need assessment
5. **Cross-sell one product to single-product customers** — drops churn from 27% to 7%
6. **Review female customer experience** — 8.61% higher churn than male customers

### 🟢 Strategic
7. **Build real-time inactivity monitoring** — flag customers before they formally exit
8. **Investigate Germany root cause** — competitor, service, or product gap
9. **Prioritise high-balance customers** in retention budget allocation
10. **Design age-appropriate product bundles** for the 41-60 segment

---

## 📈 Dashboard Preview

> Power BI dashboard available in the visuals/ folder
> Open .pbix file with Power BI Desktop
> or view the .pdf export directly

**Page 1 — Overview**
- Overall churn rate card
- Churn by geography, age group, products
- Active vs inactive, gender, balance segments

**Page 2 — Deep Analysis**
- Germany deep dive
- Funnel 1 and Funnel 2 risk narrowing charts

---

## 🛠 Tools Used

| Tool | Purpose |
|---|---|
| Python 3 | Data loading, exploration, analysis |
| Pandas | Data manipulation and groupby analysis |
| Seaborn / Matplotlib | Exploratory visualisations |
| Power BI Desktop | Interactive dashboard |
| Jupyter Notebook | Analysis environment |

---

## 📂 Dataset

| Detail | Value |
|---|---|
| Source | Public dataset — European bank simulation |
| File | Bank_Churn.csv |
| Records | 10,000 customers |
| Columns | 13 |
| Target Variable | Exited (1 = churned, 0 = retained) |
| Null Values | None |

---

## 👤 Author

**Rahul Panigrahi**
- LinkedIn: [linkedin.com/in/rahul-panigrahi-087235152](https://linkedin.com/in/rahul-panigrahi-087235152)
- GitHub: [github.com/rahulpanigrahi4079056-afk](https://github.com/rahulpanigrahi4079056-afk)

---

*This project was built as a complete Business Analytics case study —
from raw data to structured business recommendations.*
