![Screenshot 2024-06-20 021736](https://github.com/huycuuvan/PowerBi/assets/116445067/2dbe34dd-4ead-45a9-8405-875ab0f89e67)

1.	Power BI Dashboard Explanation
•  Slicers: These allow users to filter data based on Region, State, Store, and Date. This enables focused analysis on specific subsets of the data.
•  Cards: Display key metrics such as Sum of Revenue, Sum of Profit, and Profit Percentage, providing at-a-glance insights into overall performance.
•  Map: Shows profit by state with bubble sizes indicating the level of profit—larger bubbles represent higher profits.
•  Pie Charts: Display the distribution of revenue and profit by region.
•  Line Chart: Tracks Revenue and Cost over time, enabling trend analysis.
•  Bar Chart: Summarizes the total revenue.
2.	Answer the following questions using Dashboard:
•	Use the slicers at the top of the dashboard to filter by Region, State, StoreID, and Date range. Selecting an option from these slicers will dynamically update the visualizations to reflect the filtered data.
•	The Cards on the dashboard update automatically based on the slicers. When you select specific criteria (e.g., a particular state or date range), the Sum of Revenue, Sum of Profit, and Profit Percentage cards will display the values corresponding to the filtered data.
•	The Pie Chart titled "Sum of Revenue by RegionName" displays the revenue distribution among different regions. Each segment represents a region, with the size of the segment proportional to the revenue.
•	To calculate the topN and bottomN Revenue, you can create a new visualization or table in Power BI using the following steps:
o	Use the TOPN function in a DAX formula to create measures for the topN and bottomN stores based on revenue.
o	Apply these measures in a table or bar chart visualization to display the results.
•	The Map visualization displays store locations with bubbles. The size of each bubble represents the sum of profit for that store. Larger bubbles indicate higher profits, and smaller bubbles indicate lower profits. This is set by mapping the profit measure to the bubble size property in the map visualization.
•	You need to create a measure for profit calculation:
o	Use a DAX formula such as Profit = SUM(Sales[Revenue]) - SUM(Sales[Cost]) to calculate the profit for each product.
o	Apply this measure in a table or any relevant visualization to display the profit for each product.
•	The Area Chart on the dashboard tracks the Revenue and Cost over time. Each area represents either the sum of revenue or the sum of cost, allowing for visual comparison of these metrics over the selected date range.
•	Similar to calculating topN and bottomN revenue, you can create a measure for topN profits:
o	Use the TOPN function in a DAX formula to rank products based on profit.
o	Display the topN products using a table, bar chart, or any suitable visualization.
