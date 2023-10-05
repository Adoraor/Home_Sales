# Home_Sales

## Background
In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Instructions
1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
2. Import the necessary PySpark SQL functions for this assignment.
3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
4. Create a temporary table called home_sales.
5. Answer the following questions using SparkSQL:
   - What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
   - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
   - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
   - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
6. Cache your temporary table home_sales.
7. Check if your temporary table is cached.
8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
9. Partition by the "date_built" field on the formatted parquet home sales data.
10. Create a temporary table for the parquet data.
11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
12. Uncache the home_sales temporary table.
13. Verify that the home_sales temporary table is uncached using PySpark.
14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.

## Requirements
1. A Spark DataFrame is created from the dataset.

2. A temporary table of the original DataFrame is created. 

3. A query is written that returns the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year. 

4. A query is written that returns the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms. 

5. A query is written that returns the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year built rounded to two decimal places. 

6. A query is written that returns the view rating for the average price for homes that are greater than or equal to $350,000, rounded to two decimal places. (The output shows the run time for this query.) 

7. A cache of the temporary "home_sales" table is created and validated. 

8. The query from step 6 is run on the cached temporary table, and the run time is computed. 

9. A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read.

10. A temporary table of the parquet data is created. 

11. The query from step 6 is run on the parquet temporary table, and the run time is computed. 

12.The "home_sales" temporary table is uncached and verified.
