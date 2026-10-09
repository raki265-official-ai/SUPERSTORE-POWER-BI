# Superstore Sales Analysis — Power BI

An interactive sales report created with Power BI and the Sample Superstore dataset to explore sales, profit, quantity and discounts.

## Dashboard Preview

![Superstore Sales Dashboard](DASHBOARD.png)

## Project Overview

This project covers data preparation in Power Query, KPI cards, sales charts, slicers, filters and visual interactions.

The report contains two pages:
- **Sales Overview:** Interactive dashboard.
- **Order Details:** A table for exploring order-level information.

## Tools Used

- Power BI Desktop
- Power Query
- Sample Superstore CSV dataset

## Data Preparation

The original dataset contains 9,994 rows and 21 columns.

The following transformations were applied:
- Corrected column data types.
- Renamed customer, customer segment and shipping mode columns.
- Filtered customer segments to Consumer and Corporate.
- Removed Row ID, Country and Postal Code.
- Duplicated Order ID and split it into order code and order reference.
- Set the split columns to Text.

Column Quality, Column Distribution and Column Profile were used to inspect the data.

The query contains eight transformation steps, excluding Source and Promoted Headers.

## Key Performance Indicators

| KPI | Calculation |
|---|---|
| Total Sales | Sum of Sales |
| Total Profit | Sum of Profit |
| Total Quantity | Sum of Quantity |
| Average Discount | Average of Discount |

Discount is displayed as a decimal: 0.16 represents approximately 16%.

## Dashboard Charts

- **Sales by Category:** Compares category sales in descending order.
- **Profit by Region:** Compares regional profit in descending order.
- **Top 5 Sub-Categories by Sales:** Displays the five highest-selling sub-categories within the current filter context.

## Slicers and Filters

- Region slicer
- Category slicer
- Sales Overview page filter: Standard Class and Second Class shipping
- Top N visual filter: Top 5 Sub-Categories by Sum of Sales

The shipping filter applies only to Sales Overview. Order Details can therefore show different totals.

## Visual Interactions

The following interactions were tested:
- Selecting a category bar filters Profit by Region.
- Selecting a region bar filters Top 5 Sub-Categories.
- Selecting a sub-category bar filters Sales by Category.

Chart selections and slicers also update the KPI cards.

## Dashboard Insights

With all regions and categories selected and the shipping filter applied:
- Total Sales: **1,496,802.59**
- Total Profit: **178,567.48**
- Total Quantity: **24,936**
- Average Discount: **approximately 0.16**
- Technology has the highest category sales.
- West has the highest regional profit.
- Chairs leads the Top 5 Sub-Categories by Sales.

These results change when slicers or chart selections are applied.

## Design

The report uses a dark charcoal background, white visual panels, red chart accents and charcoal KPI values.

The dark background is a design variation from the assignment's specified light-grey background.

## Repository Contents

- superstore-sales overview.pbix
- sample-superstore.csv
- outputs
- Project documentation (README.md)


 ## author⭐
 
  # rakesh

## How to Use

1. Download the PBIX file and CSV dataset.
2. Open the PBIX in Power BI Desktop.
3. Explore the report using Region and Category slicers.
4. Click chart bars to filter related visuals.
5. Click the selected bar again to clear the selection.

To refresh the data, update the CSV source path in Power Query to its location on your computer.
