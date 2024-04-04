## Home_Sales
Home Sales Key Metrics

<img width="830" alt="Screenshot 2024-04-04 at 10 07 50 AM" src="https://github.com/kaurn6538/Home_Sales/assets/98873779/48723846-c6eb-4647-8841-e46f37ddf3ec">




In this challenge, we use our knowledge of SparkSQL to determine key metrics about home sales data. Then we use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.



The required questions answered as follows:

First change the data types then sql query for the answers.

<img width="351" alt="Screenshot 2024-04-04 at 10 12 08 AM" src="https://github.com/kaurn6538/Home_Sales/assets/98873779/10b239da-56b8-45b1-901b-dce0227d03e2">

1- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places. The average prices for a four bedroom house sold by year are as follows:

<img width="194" alt="Screenshot 2024-04-04 at 10 14 08 AM" src="https://github.com/kaurn6538/Home_Sales/assets/98873779/c479c5a5-6e74-4da9-8e22-ec3eb4475f93">


2- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

<img width="189" alt="Screenshot 2024-04-04 at 10 15 52 AM" src="https://github.com/kaurn6538/Home_Sales/assets/98873779/68c2fc99-7b85-4308-80aa-06beacf62210">



3- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.



4- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

<img width="448" alt="Screenshot 2024-04-04 at 10 18 01 AM" src="https://github.com/kaurn6538/Home_Sales/assets/98873779/b46b736a-56d1-4ee2-8cba-6bc875ab0610">


Compare the run times for the various methods of running the same sql query as question # 4 above:



The highest run time was the sql query from the partitioned parquet files (1.04312419891357 seconds). It was 0.47975 seconds slower than the cached temporary table sql query (0.563373327255249 seconds) and 0.15167 seconds slower than the original temporary table view sql query (0.891453504562377 seconds). The cached temporary table sql query runs fast 0.32808 seconds faster than the original temporary table query.

## References

*    Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only. https://static.bc-edx.com/data/dl-1-2/m22/lms/starter/Starter_Code.zip
*    Home Sales Photo by Oleksandr Pidvalnyi: https://www.pexels.com/photo/person-with-keys-for-real-estate-7599735/ -https://stackoverflow.com/ for various how to questions and what-if-I...
*    Grateful to our BCS learning team for clarifying question #6
