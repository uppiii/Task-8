Power BI Dashboard Assignment Guide
Step 1: Load Your Data

Open Power BI Desktop.

Click Home → Get Data → Excel (or CSV).

Select your file data.xlsx (or data.csv) → Click Load.

Your table will appear in the Fields pane.

Note the table name (e.g., data) and column names (Sales, Profit, Category, Order Date).

Step 2: Create Measures (KPIs)

Go to Modeling → New Measure and create:

Total Sales

Total Sales = SUM('data'[Sales])


Total Profit

Total Profit = SUM('data'[Profit])


Profit Margin (optional)

Profit Margin = DIVIDE([Total Profit],[Total Sales],0)


💡 DIVIDE() avoids errors if total sales = 0.

Step 3: Add KPI Cards

Go to Report view → Visualizations → Card.

Drag Total Sales → Card shows total sales.

Drag Total Profit → Card shows total profit.

Drag Profit Margin → Optional card showing percentage.

Formatting Tips:

Click Card → Format → Data label → Display units → Millions (M).

Add colors: Green for Profit, Blue for Sales.

Step 4: Visualize Profit by Category

Select Bar Chart from Visualizations.

Drag Category → Axis.

Drag Profit measure → Values.

Format:

Colors → Palette (e.g., Viridis)

Add data labels → On

Insight: Quickly see which product category contributes most to profit.

Step 5: Monthly Sales Trend

Select Line Chart from Visualizations.

Drag Order Date → X-axis.

Click the dropdown → Select Month or Month-Year.

Drag Sales → Y-axis.

Optional: Drag Profit → Y-axis → Dual axis if needed.

Insight: Shows trends and seasonal peaks in sales.

Step 6: Add Insights Text Box

Click Text Box → Type:

- Total Sales: $2,297,201 approx.
- Total Profit: $286,397 approx.
- Profit Margin: ~12.5%
- High sales don’t always mean high profit. Some categories may need cost optimization.


Format text for clarity and alignment.

Step 7: Dashboard Layout

Place Cards at top for KPIs.

Bar chart: Profit by Category → left side.

Line chart: Monthly Sales Trend → right side.

Text box: Insights → bottom or side panel.

Add colors, borders, and icons to make it visually appealing.

Step 8: Optional Features

Filters / Slicers:

Category, Region, or Segment to interactively filter the visuals.

Conditional Formatting:

Highlight negative profit values in red.

Drill-downs:

Click on Category → see Sub-Category profit.

✅ Result:
You’ll have a complete Power BI dashboard showing:

Total Sales, Total Profit, Profit Margin

Profit by Category

Monthly Sales Trend

Key insights summarized
