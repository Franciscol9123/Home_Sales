# Home_Sales
Use of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/d5283ac2-1105-4108-9234-4f770f17921b)

### Findings
1. What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/9a8c70f1-9ed2-4960-98ad-f16ac4fb457d)


2. What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/bfb02b2a-a650-4593-af63-f1603fc9cbb4)


3. What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/3916e6e1-bde4-462c-a07a-cf79088c76de)


4. What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
- Original data

![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/2cf3bdee-80e6-4b6c-b78a-bd5ac1a2fd7a)

5. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
Partition by the "date_built" field on the formatted parquet home sales data.

- Cached data
  
![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/56076394-ff03-4b77-b445-b1b61b614e52)

- Parquet formatted data

![image](https://github.com/Annbelbella/Home_Sales/assets/124645643/82c9af2e-17cb-4f41-89a2-31af8bb80656)

 Both the cached data and the Parquet formatted data have faster runtimes compared to the original data . 

In conclusion, Parquet formatted data demonstrates the best runtime among the three options (Run time for original data, cached data and parquet formatted data).
