# 🛒 Superstore Sales Analysis — Power BI

An interactive Power BI report for analysing sales, profit, quantity and discounts using the Sample Superstore dataset.

## 📊 Dashboard Preview

![Superstore Sales Dashboard](./DASHBOARD.png)

## 📌 Project Overview

This project demonstrates data preparation, KPI reporting, visual analysis and interactive filtering in Power BI.

The report contains two pages:
- **Sales Overview:** Interactive sales dashboard.
- **Order Details:** Detailed order information in a table.

## 🛠️ Tools Used

- Power BI Desktop
- Power Query
- Sample Superstore CSV dataset
- GitHub for project documentation

## 🧹 Data Preparation

The original dataset contains **9,994 rows and 21 columns**.

Transformations applied in Power Query:
- Corrected column data types.
- Renamed customer, customer segment and shipping mode columns.
- Kept Consumer and Corporate customer segments.
- Removed Row ID, Country and Postal Code.
- Duplicated Order ID.
- Split the duplicated Order ID into order code and order reference.
- Renamed the split columns and set their data types to Text.

The query contains **eight transformation steps**, excluding Source and Promoted Headers.

Column Quality, Column Distribution and Column Profile were used to inspect the data.

## 🎯 Key Performance Indicators

| KPI | Calculation |
|---|---|
| Total Sales | Sum of Sales |
| Total Profit | Sum of Profit |
| Total Quantity | Sum of Quantity |
| Average Discount | Average of Discount |

Average Discount is displayed as a decimal: **0.16 represents approximately 16%**.

## 📈 Dashboard Charts

- **Sales by Category:** Category sales sorted in descending order.
- **Profit by Region:** Regional profit sorted in descending order.
- **Top 5 Sub-Categories by Sales:** Highest-selling sub-categories within the current filter context.

Data labels make the values easy to compare.

## 🎛️ Slicers and Filters

- **Region slicer:** Explore regional performance.
- **Category slicer:** Explore product categories.
- **Page filter:** Standard Class and Second Class shipping.
- **Top N filter:** Top 5 Sub-Categories by Sum of Sales.

The shipping filter applies only to Sales Overview. Totals on Order Details can therefore differ.

## 🔄 Visual Interactions

The following chart interactions were tested:
- Category selection filters Profit by Region.
- Region selection filters Top 5 Sub-Categories.
- Sub-Category selection filters Sales by Category.

Slicers and chart selections also update the KPI cards.

## 💡 Dashboard Insights

With all regions and categories selected and the shipping filter applied:

| Metric | Value |
|---|---:|
| Total Sales | 1,496,802.59 |
| Total Profit | 178,567.48 |
| Total Quantity | 24,936 |
| Average Discount | Approximately 0.16 |

- **Technology** has the highest category sales.
- **West** has the highest regional profit.
- **Chairs** leads the Top 5 Sub-Categories by Sales.

Results change when slicers or chart selections are applied.

## 🎨 Report Design

- Dark charcoal canvas
- White cards and chart panels
- Red chart accents and visual titles
- Charcoal KPI values
- Left-side slicers
- Aligned visuals in a 16:9 layout

The dark background is a design variation from the assignment's specified light-grey background.

## 📂 Repository Contents

- Power BI report — `.pbix`
- Original Superstore dataset — `.csv`
- Dashboard preview — `DASHBOARD.png`
- Order Details screenshots
- Project documentation — `README.md`

## 🚀 How to Use

1. Download the Power BI report and CSV dataset.
2. Open the PBIX file in Power BI Desktop.
3. Use Region and Category slicers to explore the dashboard.
4. Click a chart bar to filter related charts and KPI cards.
5. Click the selected bar again to clear the selection.
6. Open Order Details to view detailed records.

For data refresh, update the CSV source path in Power Query to the file's location on your computer.
