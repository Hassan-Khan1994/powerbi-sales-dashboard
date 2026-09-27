# 📊 Power BI Sales Dashboard

An interactive **Power BI** dashboard analyzing sales performance across regions, product categories, customer segments, and sales representatives — built to turn raw transactional data into decisions.

> **Author:** Hassan Khan · Technical Project Manager & BI/Business Analyst
> **Tools:** Power BI Desktop, DAX, Power Query

---

## 🎯 Business Questions Answered

- What are our **total sales, profit, and profit margin**, and how are they trending over time?
- Which **regions and segments** drive the most revenue?
- What are the **top-performing products and categories**?
- Who are the **top sales representatives**?
- Where are we **losing margin to discounts**?

---

## 🖼️ Dashboard Preview

> 📌 _Add your dashboard screenshots to the `images/` folder and link them here._

<!-- Example:
![Sales Overview](images/dashboard-overview.png)
![Regional Breakdown](images/regional-breakdown.png)
-->

*(Screenshots coming soon — dashboard in progress.)*

---

## 📁 Dataset

The sample dataset is in [`data/sample_sales_data.csv`](data/sample_sales_data.csv) — **600 orders (2023–2024)** with the following fields:

| Column | Description |
|--------|-------------|
| `OrderID` | Unique order identifier |
| `OrderDate` | Date of the order |
| `Region` | Sales region (North, South, East, West, Central) |
| `Segment` | Customer segment (Consumer, Corporate, SME) |
| `SalesRep` | Sales representative |
| `Category` | Product category |
| `Product` | Product name |
| `Quantity` | Units sold |
| `UnitPrice` | Price per unit |
| `Discount` | Discount applied (0–0.20) |
| `Sales` | Net sales amount |
| `Profit` | Profit for the order |

---

## 📈 Key Insights

> _Fill this in once your dashboard is built — this section is what recruiters read first._

- 📌 _Insight 1 — e.g. "The West region generated 28% of total revenue."_
- 📌 _Insight 2 — e.g. "Electronics had the highest sales but Furniture had the best margin."_
- 📌 _Insight 3 — e.g. "Discounts above 15% erased most of the profit on Office Supplies."_

---

## 🧮 Sample DAX Measures

```dax
Total Sales   = SUM ( Sales[Sales] )
Total Profit  = SUM ( Sales[Profit] )
Profit Margin = DIVIDE ( [Total Profit], [Total Sales] )
Total Orders  = DISTINCTCOUNT ( Sales[OrderID] )
Avg Order Value = DIVIDE ( [Total Sales], [Total Orders] )
```

---

## 🚀 How to Open

1. Download / clone this repository.
2. Open **Power BI Desktop**.
3. Get Data → **Text/CSV** → select `data/sample_sales_data.csv`.
4. Build your visuals, or open the `.pbix` file in the `dashboard/` folder (once added).

---

## 🗂️ Repository Structure

```
powerbi-sales-dashboard/
├── data/        # Source dataset (CSV)
├── dashboard/   # Power BI file (.pbix)
├── images/      # Dashboard screenshots
└── README.md
```

---

## 🛠️ Skills Demonstrated

`Power BI` · `DAX` · `Power Query` · `Data Modeling` · `Data Visualization` · `Business Analysis`

---

<sub>⭐ Part of my data analytics portfolio. Feedback and opportunities welcome — khanhassan718@yahoo.com</sub>
