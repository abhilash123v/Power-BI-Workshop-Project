# Power-BI-Workshop-Project
This is beginner friendly Project. One can learn complete power BI.

### 1
##### What is Power BI?
Power bi is a magic tool which turns boring data into cool,interactive visuals like graphs,charts and dashboards. Simply story telling whith data,helps your team make smarter decisions.
_One can easily answers questions like_
- In which market/region furniture category is doing well?
- Tell me from which category we are getting highest profits?
##### Things covered in this project:
1. Data prep and cleaning
2. Data modelling
3. Visuals
4. DAX
5. Power BI service
#### Creating Visuals.
1. Import file named "Orders" which contains two sheets.
2. connect both sheets "List of Orders" and "orders breakdown" by clicking on Data modelling icon which have orderid as common column(just drag orderid  onto id column)(_cardinality is 1:many_). This also called __data modelling(where we are making connection between 2 sheets, so that we are able to get answers).__ why? becuase numerical values are present in order breakdown sheet.
3. __Interactivity__: By clicking on 1 graph all others visuals data gets changed in dashboard.
4. Format visuals -> callout value ->two decimal places.
5. Created KPI's ->OrderID,Total Profit,Total Sales,Total Cost(derived column -> Cost=sales-profit using table view option-> create new column).
6. clustered column charts -> sum of sales by region, sub-category wise sum of sales,
7. Table Visual -> customer name wise count of orders,sum of profits.
8. Pie chart -> Sum of quantity(in values) by region(in legend).
9. Line chart -> Count of orders by year,quarter.
10. Slicers : Drag order date to Field-> you can adjust the time filter.
11. Bubble map/Map chart ->Country(in location),orderid(in bubble size).
12. __Drill Down__: Also called Time intellegence-> means (DAX -> time and year functions + line plot year,quarter,month,day wise): Clustered column chart you get options on top(arrows)-> click on ⬇️,now click on any year _bars_ to further drill down to month,day.

### 2
#### Data Preparation in Power BI (cleaning, transforming & shaping data).
##### Session-1:
Steps followed:
1. Loaded the dataset "FactCmpySales_2017" into Power Query Editor,clicking on "Transform" Button.
2. Removed Top (Two) rows using Remove rows option from Top Ribbon,since we don't need them.
3. Made 1st row as header using the option available from the menu.
4. Renamed order id,Removed dupliactes since order id should be unique,Changed the datatype to Whole number from Text,Excluded rows with "NA,Blanks" using filtering.
5. Removed Column3,promo bin2,Promo discount2.
5. Changed datatype of order_date to date,handled error(50% errorrate) using _replaced errors with "null" option_ or simply keep it as itis..
7. Sales column: replaced sales word with empty space from each row,changed datatype to whole number since we cannot calculate total sales with text datatype format.
8. Promobin1: replaced blank cells with null and then use "fill up" option, to fill the values.
9. Removed errors from sales,price colum since they are lessthan 1%. 
__"Click on Close and Apply"__
10. Created 4 KPI's,1 pie chart,1 line chart,1 clustered column chart.
##### Session-2:
1. Append data using power query: Appending 2 tables 1 after the other(both must have same number of columns.
2. Merge: Merge two tables using a common column just like joins in sql.
3. Pivot and unpivot:_
  Use Unpivot to turn columns into rows (ideal for time-series, creating attribute-value pairs), and Pivot to turn row values into column headers (aggregating data).
  Both are found in the Transform tab. 
4. Getting data into PowerBI from multiple sources.
### 3
#### Import and Work with data from multiple sources like:
* CSV Files
* Excel
* SQL Databases
* Web Sources
* Cloud Platforms
