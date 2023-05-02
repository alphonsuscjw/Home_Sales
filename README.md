# Home_Sales

This challenge ustilises SparkSQL to determine key metrics about home sales data. This data comes in the form of big data in a CSV file which contains the metadata for each house sold, such as price, date sold, date built and number of bedrooms and bathrooms.

The following steps were involved in the analysis:
1. Read the CSV file into a Spark Dataframe.
2. Created a temporary view/table called "home_sales" of the DataFrame.
3. Made 4 SQL queries to answer 4 questions relevant to the analysis of the data.
4. Cached the temporary table and validated the cache.
5. Using the cached data, ran one of the same queries above. Determined the runtime and compared it to uncached runtime.
6. Formatted the home sales data into parquet format and partitioned by the "date_built" field on it.
7. Read the parquet formatted and partitioned data.
8. Created a temporary table for the parquet data.
9. Ran the same query above with the parquet DataFrame. Determined the runtime and compared it to the cached version.
10. Uncached the home_sales temporary table and verified that it was uncached.
