# Voltmetrics — Sales & CRM Analytics Platform

A Business Intelligence and CRM solution built for **Volt Metrics**, a growing consumer electronics retailer, to support its expansion into the Irish market and its shift toward a customer-centric, data-driven business model.

This project combines **Power BI** dashboards with **Salesforce CRM** reporting to unify sales performance, product analytics, and customer relationship management into a single closed-loop system.

---

## 📌 Project Overview

Volt Metrics operates physical stores across the US, UK, Germany, Canada, France, the Netherlands, and Australia, generating over **$11M in revenue** across **9,000+ orders** and **~6,500 customers**. Despite steady growth, the business lacked:

- A unified view of sales performance across regions and channels
- Customer segmentation and CRM integration
- Real-time inventory and demand insight
- A tracked, personalised marketing strategy

This project addresses those gaps through an integrated **Power BI + Salesforce CRM** solution built on a synthetic dataset (~60,000 transactions, 7,000 customers, 100 products, 50 stores) designed to mirror real-world retail operations.

---

## 🎯 Business Goals

- Support strategic **market expansion into Ireland**
- Grow **online sales share** beyond the current 13.9%
- Build a **customer-centric CRM** with segmentation and loyalty tracking
- Improve **product and inventory planning**
- Enable **faster, data-driven decision-making** across the business

---

## 🧱 Data Model

A star schema built around a central **Sales fact table**, linked to four dimension tables:

| Table | Purpose |
|---|---|
| **Sales** | Central fact table — orders, revenue, quantity, dates, channel |
| **Products** | Product metadata — brand, category, subcategory, pricing |
| **Customers** | Demographics — country, gender, segment |
| **Stores** | Store-level attributes — location, size, purchase type |
| **Date** | Time intelligence — day, month, quarter, year |
| **Measures** | Centralised DAX measures for KPIs |

Relationships follow standard one-to-many foreign key joins (`ProductKey`, `CustomerKey`, `StoreKey`, `Date`) enabling multi-dimensional slicing across time, geography, product, and customer attributes.

---

## 📊 Power BI Dashboards

**1. In-Store Sales Performance** — Revenue, orders, top brands/products, quarterly trends, channel split, and revenue by country.

**2. Online Sales Performance** — Same KPI structure filtered to the online channel, enabling direct online vs. in-store comparison.

**3. Category Performance** — Revenue and order volume by product category, subcategory, and colour, with a drill-through subcategory matrix.

**4. Customer Details Overview** — Demographic and behavioural analysis: spend trends by year, gender and age-group splits, and customer-level revenue tables, filterable by country and quarter.

---

## 🤝 Salesforce CRM

- **Customer Segmentation & Lifetime Value Dashboard** — segments 32+ customers into High-Value, Medium-Value, Repeat, and One-Time buyer groups, with average spend and top-10 LTV rankings.
- **Marketing Campaigns** — three targeted campaigns (Q3 Promo for High-Value customers, Loyalty Booster for Repeat buyers, Come Back Offer for One-Time buyers), each with tracked contact reach and status.
- **Case Management** — support case tracking for issues like delayed shipping and unprocessed refunds, including priority flagging and cross-sell linkage.

---

## 🛠️ Tools & Technologies

`Power BI` · `DAX` · `Power Query` · `Salesforce CRM` · `Mockaroo` (synthetic data generation) · `Star Schema Data Modelling`

---

## 📁 Repository Contents

```
├── VoltMetricsDashboardfinal.pbix     # Power BI dashboard file
├── BIBA_CA2_Report.pdf                # Full specification & implementation report
├── Presentation_2.pptx                # Project presentation deck
└── README.md
```

---

## 🔍 Key Insights

- **Computers** and **Cell Phones** are the top-performing categories by both revenue and order volume
- **Adventure Works** and **Contoso** are the strongest-performing brands across channels
- Revenue shows a **seasonal dip in Q2**, recovering in Q3/Q4
- **High-Value customers** average €111K in spend vs. €12K for One-Time buyers — a strong case for loyalty investment
- Ireland shows early but promising customer activity, supporting the case for targeted regional expansion

## 📷 Dashboard Preview
Below is a screenshot of the final interactive Power BI dashboard built for this project.
<img width="586" height="329" alt="image" src="https://github.com/user-attachments/assets/69232421-c026-400f-966f-1a9b19891d5a" />
<img width="632" height="356" alt="image" src="https://github.com/user-attachments/assets/f9e6475e-a693-4d08-8a39-508e7e2918c2" />

<img width="660" height="374" alt="image" src="https://github.com/user-attachments/assets/a2388716-8844-4db0-848a-d0cd1c5f8b07" />

## 🤝 Salesforce CRM


Customer Segmentation & Lifetime Value Dashboard — segments 32+ customers into High-Value, Medium-Value, Repeat, and One-Time buyer groups, with average spend and top-10 LTV rankings.
Marketing Campaigns — three targeted campaigns (Q3 Promo for High-Value customers, Loyalty Booster for Repeat buyers, Come Back Offer for One-Time buyers), each with tracked contact reach and status.
Case Management — support case tracking for issues like delayed shipping and unprocessed refunds, including priority flagging and cross-sell linkage.

<img width="453" height="174" alt="image" src="https://github.com/user-attachments/assets/c6df6dae-3745-404d-a3db-4bd4dc1c7a7b" />

<img width="432" height="295" alt="image" src="https://github.com/user-attachments/assets/5fd64a96-6f0f-4b17-9657-a1a5ff34189d" />

<img width="839" height="296" alt="image" src="https://github.com/user-attachments/assets/27e94960-8d7d-4406-8fb0-ec3f87dd33d2" />





---

## 🚀 Future Enhancements

- Predictive analytics for sales forecasting and churn risk
- Automated, dynamic Customer Lifetime Value scoring
- Real-time campaign performance tracking (opens, click-throughs)
- AI-assisted case routing and resolution recommendations
