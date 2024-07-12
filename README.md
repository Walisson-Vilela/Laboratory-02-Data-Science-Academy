# Microsoft Power BI for Business Intelligence and Data Science
Lab 2
Sales, Cost, Profit Margin and KPI Dashboard

(**) 1- What was the total sales value considering each order shipping method?<br>
Using a waterfall chart, I used the shipping mode on the category and the sum of value on the y-axis. The result is that the Standard Class has the highest sales per shipping method with 8 Mi.<br>
(**) 2- Which markets had the highest average shipping cost for products sold?<br>
To calculate the average cost per shipment, I used the TreeMap graph. I used the Customer table, the Market category and calculated the average cost per shipment. It was shown that APAC had the highest average number of product shipments followed by the US.<br>
(**) 3- The company aims (goal) to maintain an average of 350 for the sales value every month. Show an indicator (KPI – Key Performance Indicator) with the average sales value. Was the company below or above the target in April/2014?<br>
According to the indicator, the company was below the target of 350.00. To calculate the target, I used the Meter Axis filter with a target of 350, and to find out whether the month of April was above or below, I used data tracking selecting the month of April of 2014.<br>
(**) 4- Consider that the profit is equivalent to: sales value - shipping cost. Which product category showed the highest average profit?<br>
To calculate the average profit per category, I had to create a calculated profit column, calculating the sales value minus the shipping cost using DAX language (profit = sales[Sales Value] - Sales[Shipping Cost]).
To display the data, I used the Pie chart, as there are few categories. The category that presented the highest average profit was Technology.<br>
(**) 5- What was the behavior of the profit margin over time? Consider the profit margin as the profit divided by the sales value.<br>
Creating a new Profit Margin column, I used the expression DAX Profit Margin = ROUND(DIVIDE(Sales[Profit],Sales[Sales Value]) * 100, 2), thus calculating the division of the profit by the sales value, thus being the The sum of the profit margin until July 2014 was 194 million.<br>

![Dashboard](./Lab02.png)
