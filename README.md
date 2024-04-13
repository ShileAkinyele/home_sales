# home_sales
This contains analysis on home sales data using pyspark sql. the spark sql query is used to find the following metrics.

What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.


For further optimization while shuffling to better optimize the speed at which data is being processed the following techniques are applied, 

Creating a temporary view 
Caching the temporary view data and partitioning the parquetformated data. Using just the temporary view of the table gives a run time of 1.2160 seconds while that of Caching the temporary view data gives 0.5159 secs and the parquet dataframe gives 
a run time of 0.9066 seconds.

