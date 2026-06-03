[README.md](https://github.com/user-attachments/files/28539881/README.md)
# Task2-Oluwabusola-Oyenuga# 🛒 E-Commerce Sales — Exploratory Data Analysis (EDA)
**DecodeLabs Data Analytics Internship | Project 2 | Batch 2026**

---

## 📌 Project Overview

This project performs an Exploratory Data Analysis (EDA) on an e-commerce orders dataset covering January 2023 to June 2025. The goal is to uncover hidden patterns, trends, and outliers that can inform business decisions — before any dashboards or predictive models are built.

---

## 🎯 Objective

- Understand the structure and quality of the dataset
- Calculate descriptive statistics across key numeric columns
- Detect and interpret outliers using the IQR method
- Analyse product performance, order status, referral sources, and coupon impact
- Translate findings into actionable business recommendations

---

## 📁 File Structure

```
📂 DecodeLabs-Project-2/
│
├── 📊 Dataset_for_Data_Analytics.xlsx   # Raw dataset
├── 📊 EDA_Ecommerce_Analysis.xlsx       # Full EDA workbook (6 sheets)
└── 📄 README.md                         # Project documentation
```

---

## 📂 Workbook Structure

| Sheet | Description |
|---|---|
| Raw Data | Original dataset — untouched |
| Data Overview | Dataset summary, column info, and data quality check |
| Descriptive Statistics | Mean, median, min, max, Q1, Q3, std dev for numeric columns |
| Outlier Detection | IQR method applied to TotalPrice, UnitPrice, and Quantity |
| Analysis | Product performance, order status, referral source, payment method, coupon impact |
| Key Insights | Executive summary, key findings, and business recommendations |

---

## 📊 Dataset Summary

| Item | Value |
|---|---|
| Total Orders | 1,200 |
| Total Columns | 14 |
| Date Range | January 2023 – June 2025 |
| Unique Customers | 1,189 |
| Unique Products | 7 |
| Total Revenue | $1,264,761.96 |
| Missing Values | CouponCode — 309 rows (25.75%) |

---

## 🔍 Key Findings

1. **Only 19.3% of orders were successfully delivered** — cancellations (20.8%) and returns (20.6%) are the top two order statuses, representing a major fulfilment problem.
2. **Chair and Printer lead in total revenue** (~$195K each), while Phone and Desk trail behind.
3. **Laptop buyers have the highest average order value** ($1,110) — a premium customer segment.
4. **Tablet has the highest return rate (43 returns)** — suggesting a product description or quality mismatch.
5. **Chair has the most cancellations (45)** — possible stock or delivery issues.
6. **Instagram is the top acquisition channel** (259 orders), ahead of Email and Google.
7. **Coupon users spend $14 more on average** than non-coupon users — coupons attract, not discount.
8. **8 bulk-buyer outliers were detected** — all ordered maximum quantity (5 units) at high unit prices. These are premium buyers, not data errors.
9. **TotalPrice is right-skewed** — median ($824) is a more accurate measure of typical order value than the mean ($1,054).

---

## 🧮 Outlier Detection — IQR Method

Applied to **TotalPrice**:

| Metric | Value |
|---|---|
| Q1 | $410.52 |
| Q3 | $1,578.47 |
| IQR | $1,167.95 |
| Lower Bound | -$1,341.41 |
| Upper Bound | $3,330.41 |
| Outliers Found | 8 orders |
| Verdict | SIGNAL — retained as premium bulk buyers |

No outliers were found in UnitPrice or Quantity.

---

## ✅ Recommendations

1. **Investigate cancellations and returns urgently** — with only 19.3% delivery success, the fulfilment process needs immediate review.
2. **Prioritise Chair, Printer, and Laptop** in inventory and marketing — they drive the most revenue.
3. **Review Tablet product listings** — high return rate likely signals an expectation gap between listing and product.
4. **Double down on Instagram** — it's the highest-performing acquisition channel.
5. **Expand coupon campaigns** — data shows coupon users spend more, making coupons a net positive.
6. **Build a VIP programme** targeting the 8 identified bulk buyers.
7. **Use median ($824) as the benchmark** for typical order value, not the mean, due to right skew.

---

## 🛠️ Tools Used

- Microsoft Excel (Data Analysis, Formulas, Charts)

---

## 👩🏾‍💻 Analyst

**Oluwabusola Oyenuga**
Data Analyst | DecodeLabs Internship Batch 2026
[LinkedIn](https://www.linkedin.com/in/oluwabusola-oyenuga) | [GitHub](https://github.com/oluwabusola-may)
