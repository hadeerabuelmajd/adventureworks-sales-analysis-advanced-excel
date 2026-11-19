# AdventureWorks Sales Analysis | Excel Dashboard

> **Executive summary:** Analyzed AdventureWorks sales data (**$102.4M revenue, $42.6M profit, 41.6% margin, 24.4K transactions**) and built a 2-page interactive Excel dashboard. Key findings: profit is highly seasonal (Q4 = 41%), almost entirely driven by premium products (94.4%), concentrated in one product line (Mountain-200), while **78% of the catalog never sold**.

<!-- TODO: state which year/period the KPI numbers above represent (e.g. "FY2007") -->

---

## 1. Business Problem

AdventureWorks is a bicycle and accessories company selling internationally. Management needs to understand:

- When, where, and from whom does profit come?
- Which products, colors, and price segments drive profit?
- Is the business dependent on a few products or customers?
- Which parts of the catalog are not performing?

## 2. Dataset & Data Model

- **Source:** AdventureWorks sample dataset (`AdventureWorks--.xlsx`)
- **Structure:** Sales data linked to Product, Customer, Territory, and Date tables
<!-- TODO: describe how you prepared it: Excel Tables / Power Query / Data Model (Power Pivot) / lookup formulas -->

<!-- TODO: add a screenshot of the model view -->
<!-- ![Data Model](images/data_model.png) -->

## 3. Tools & Skills

Microsoft Excel · PivotTables ·  Data Modeling . Dax . Powe Query ( Transfomations , Data cleaning ) Slicers · Interactive Charts · Dashboard Design · Business Storytelling
<!-- TODO: add only what you really used: Power Query, Power Pivot/Data Model, XLOOKUP/INDEX-MATCH, SUMIFS, etc. -->

## 4. Dashboard

### Page 1: Time Analysis
KPIs (Qty, COGS, Revenue, Profit, Margin, Transactions), profit by year, month, weekday, quarter, and country filters.

<!-- ![Time Analysis](images/time_analysis.png) -->

### Page 2: Detail Dashboard
Top-5 products and customers, product colors, pricing types, catalog coverage, customer age groups, gender split, and geography.

<!-- ![Detail Dashboard](images/detail_dashboard.png) -->

## 5. Key Calculations

```
Revenue       = Quantity x Unit Price
Profit        = Revenue - COGS
Profit Margin = Profit / Revenue
```
<!-- TODO: replace with your real formulas / calculated fields (e.g. SUMIFS, calculated fields in PivotTables, Top-5 share, unsold products count) -->

## 6. Key Insights & Recommendations

| # | Insight | Why it matters | Recommendation |
|---|---------|----------------|----------------|
| 1 | **Strong seasonality:** Q4 generated $17.63M (41% of profit) vs $6.10M in Q1 (~3x). Oct-Dec alone = 41.4% of the year's profit. | Staffing, inventory, and campaigns must be ready before the peak. | Build inventory and launch campaigns in Q3; use Q1 for clearance and low-season offers. |
| 2 | **Premium products drive profit:** items priced above $150 generate 94.4% of profit ($40.2M) vs 5.6% for cheaper items. | The business depends on high-ticket sales. | Focus marketing budget on premium lines; use low-price items as add-ons. |
| 3 | **Product concentration:** the top 5 products are all Mountain-200 variants and make up 34.9% of profit. | A supply issue or competitor move on one line hits profit directly. | Secure supply for Mountain-200 and diversify with other strong lines. |
| 4 | **Bloated catalog:** only 133 of 606 products sold; **473 (78%) had no sales.** | Unsold items add storage and management cost. | Review and discontinue or bundle slow products. |
| 5 | **No customer dependency:** the top 5 customers = 0.5% of profit across 9,309 customers. | Low key-account risk. | Focus on broad acquisition and retention, not VIP accounts. |
| 6 | **Geography & age:** Australia + United States = 60.1% of profit; customers aged 50+ = 53.3% (average age 47). | Shows where and to whom marketing works best. | Prioritize these markets and tailor campaigns to the 50+ segment. |
| 7 | **Color mix:** Black leads with $16.7M (~39% of profit), then Silver $9.8M and Yellow $7.3M. | Helps decide which colors to stock deeper. | Stock more Black/Silver; review low-performing colors. |

**No meaningful pattern found in:** weekday vs weekend (72.3% weekday, about what 5 of 7 days would give) and gender (50.5% female / 49.5% male). Both look balanced, so I did not build recommendations on them.

## 7. Limitations & Assumptions

- Findings reflect the selected period/filters shown in the screenshots. <!-- TODO: specify the year -->
- The "50+" age group is open-ended, so it is not directly comparable to the 5-year bands.
- <!-- TODO: note whether 2008 data is complete or partial, since 2008 ($42M) is slightly below 2007 ($43M) -->
- This is a practice/portfolio project using a public sample dataset, so recommendations are illustrative.

## 8. Repository Structure

```
├── README.md
├── AdventureWorks--.xlsx
├── AdventureWorks_Dashboard.xlsx
└── images/
    ├── data_model.png
    ├── time_analysis.png
    └── detail_dashboard.png
```

## 9. Contact

<!-- Your name · LinkedIn · Email -->
