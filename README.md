# DecodeLabs Internship – Project 4: Data Visualization (Power BI)

## 📌 Project Overview
This project transforms the insights from **Exploratory Data Analysis (Project 2)** into a polished, interactive Power BI dashboard. The goal is to communicate key business findings clearly, following best practices for data visualization – action titles, high data‑ink ratio, direct labelling, and a single narrative per page.

## 🧹 Recap: Project 1 – Data Cleaning & Preparation
Before any analysis or visualisation, the raw sales dataset was cleaned using Excel Power Query:
- Removed duplicate `OrderID` values (zero duplicates remain).
- Standardised `Date` to ISO format (YYYY-MM-DD).
- Rounded `UnitPrice` and `TotalPrice` to 2 decimal places.
- Trimmed whitespace from all text columns.
- Applied **Proper Case** to `Product`, `ShippingAddress`, `PaymentMethod`, `OrderStatus`, `ReferralSource`.
- Preserved nulls in `CouponCode` (meaningful – indicates no coupon used).



## 📊 Recap: Project 2 – Exploratory Data Analysis (EDA)
Using the cleaned dataset, the following analyses were performed (in Excel):
- Descriptive statistics (mean, median, quartiles, IQR) for Quantity, UnitPrice, TotalPrice, ItemsInCart.
- Histogram of TotalPrice (right‑skewed, most orders <$1000).
- Outlier detection using the IQR method – orders above $3,330 flagged.
- Correlation analysis: UnitPrice vs TotalPrice (r=0.72), Quantity vs TotalPrice (r=0.62), ItemsInCart vs TotalPrice (r=0.39).
- PivotTables for revenue by product, order status, payment method, and average order value by referral source.
- Monthly sales trend line chart (peaks in May‑June, dips in January).

Key insight: **Only 19% of orders are delivered** – over 41% are cancelled or returned.

## 🎯 Project 4 – Data Visualization (Power BI)
All EDA insights were converted into an interactive Power BI dashboard. The visualisations follow the **SCR framework** (Situation → Complication → Resolution) and adhere to the principles from the project brief:

### Visualisations Created

| Business Question | Visual Type | Key Finding |
|------------------|-------------|--------------|
| What are the overall KPIs? | Card visuals | Total revenue, total orders, average order value, outlier count |
| Which product generates the most revenue? | Bar chart | Chair leads (15.5% of normal revenue), Phone lowest (12.3%) |
| What is the order status breakdown? | Donut Chart | Only 19% Delivered; 21% Cancelled, 21% Returned – critical issue |
| How does revenue trend over time? | Line chart | Highest month: June 2024 ($68k); seasonal peaks in May‑June |
| Which payment method is most used? | Bar chart | Credit Card highest, but Cash & Online are very close |
| Which referral source has highest average order value? | Bar chart | Facebook & Instagram (~$1055) slightly outperform others |



## 📁 Files in this Repository
| File Name | Description |
|-----------|-------------|
| `Dataset for Data Analytics (Project 2) - Cleaned.xlsx` | The cleaned dataset used as source for Power BI. |
| `Project4_Dashboard.pbix` | Power BI file containing all visuals and measures. |
| `README.md` | This file – project documentation. |

## 🚀 How to Reproduce
1. Open `Project4_Dashboard.pbix` in Power BI Desktop.
2. Refresh data if needed (the Excel source is included).
3. Explore the dashboard – use slicers to filter by date and product.

## 📈 Key Business Recommendations (from the dashboard)
- **Fix order fulfilment** – only 19% of orders are delivered. Investigate cancellation and return causes.
- **Boost Phone sales** – lowest revenue product (12.3%). Consider bundling or promotions.
- **Leverage seasonal peaks** – plan major campaigns around May‑June.
- **Maintain all payment methods** – revenue is balanced, but Debit Card lags slightly.
- **Encourage high‑value referrals** – Facebook & Instagram drive the highest AOV.


---

*Intern: Shaima Morgan*  
*Batch: 2026*  
