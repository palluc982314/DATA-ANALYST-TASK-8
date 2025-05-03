# DATA-ANALYST-TASK-8
Develop an elementary interactive dashboard that displays sales performance for product, region, and month
# ???? Simple Sales Dashboard Design (Task 8)

## ???? Objective
Design a simple interactive dashboard in Power BI that displays sales performance by product category, region, and month.

---

## ???? Tools Used
- **Primary Tool:** Power BI
- **Optional:** Python + Pandas (for preprocessing)
- **Dataset:** Superstore_Sales.csv  
  *(Columns: Order Date, Region, Category, Sales, Profit)*

---

## ???? Recreating the Dashboard Steps

### 1. Load the Dataset
- Launch Power BI Desktop.
- Navigate to `Home > Get Data > Text/CSV`.
- Load the data by selecting the `Superstore_Sales.csv` file.

### 2. Format Order Date as "Month-Year"
**Option A: Power Query Editor**
- Launch Power Query Editor (`Transform Data`).
- Choose the `Order Date` column.
- Apply `Add Column > Column from Examples` to get Month-Year (e.g., `Jan-2016`).
-.Rename to `MonthYear`, then press `Close & Apply`.

**Option B: Using DAX (Recommended)**
-.Go to `Modeling > New Column` and type:
  ```DAX
  MonthYear = FORMAT('Superstore_Sales'[Order Date], "MMM-yyyy")
3. Create Visuals
???? Line Chart - Sales over Months
Axis: MonthYear

Values: Sales

???? Bar Chart - Sales by Region
Axis: Region

Values: Sales

???? Donut Chart - Sales by Category
Legend: Category

Values: Sales

4. Add a Slicer (Filter)
Add a Slicer visual.

Drag Region or Category in for dynamic filtering.

5. Format and Highlight
Apply the Format pane (paint roller icon) to:

Highlight top values with colors

Add chart titles

Change axis labels, fonts, and backgrounds

???? Deliverables
Dashboard Screenshot or PDF Export

Export via: File > Export > PDF
or screenshot using Snipping Tool.

Insights (see below)

???? Insights from the Dashboard
???? West region consistently registered the largest total sales, particularly in Q3 and Q4.

???? Technology category produced most of the revenue, followed by Furniture.

???? Sales experienced a seasonal trough in February of several years.

????️ November and December were the best months for sales, presumably due to year-end promotions.

✅ Outcome
By doing this task, you will:

Learn to use Power BI for visual analytics

Know how to reshape and filter time-series data

Practice summarizing data into concise business insights

