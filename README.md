# Power-BI-Workshop-Project
End to End Power BI Project

Data Preparation in Power BI (cleaning, transforming & shaping data).
Session-1:
Steps followed:
1.Loaded the dataset "FactCmpySales_2017" into Power Query Editor,clicking on "Transform" Button.
2.Removed Top (Two) rows using Remove rows option from Top Ribbon,since we don't need them.
3.Made 1st row as header using the option available from the menu.
4.Renamed order id,Removed dupliactes since order id should be unique,Changed the datatype to Whole number from Text,Excluded rows with "NA,Blanks" using filtering.
5.Removed Column3,promo bin2,Promo discount2.
5.Changed datatype of order_date to date,handled error(50% errorrate) using replaced errors with "null" option.
7.Sales column: replaced sales word with empty space from each row,changed datatype to whole number since we cannot calculate total sales with text datatype format.
8. Promobin1: replaced blank cells with null and then use "fill up" option, to fill the values.
9.Removed errors from sales,price colum since they are lessthan 1%. 
"Click on Close and Apply"
10. Created 4 KPI's,1 pie chart,1 line chart,1 clustered column chart.
