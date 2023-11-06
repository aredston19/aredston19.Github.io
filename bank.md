# international monetary fund #

Data Career JumpStart week 4. In this module I’m exploring SQL, a crucial tool for data analysts when exploring large data sets. SQL allows you to query your data and find important insights in a matter or no time. 

In this module I am analyzing data from the world bank about loans made by the International Development Agency (IDA) to different countries. The csv file contains 30 data points (columns) for 1,109,994 records (rows), which would make it almost impossible to analyze in excel. With that much data an excel workbook is incapable of performing even the most basic calculation tasks like sum, count, etc. Much less trying to perform a more intensive task like a v-lookup or pivot table. 

When we turn our attention to SQL, it is important to know what we are looking for. In order to see the data we are working with we begin with the most basic of queries.

SQL is a vast landscape and there is a . Today I’ll introduce 10 of the most important commands in SQL:

1. SELECT
2. FROM
3. LIMIT
4. COUNT
5. WHERE
6. ORDER BY
7. SUM
8. AS
9. GROUP BY
10. MIN/ MAX

SELECT *
FROM world_bank

SELECT *
FROM world_bank
LIMIT 10

<img src="images/WB_1.png?raw=true"/> 
Query1

<img src="images/WB_2.png?raw=true"/> 
Query2


The two most important commands and the only two required in every SQL query are SELECT & FROM. 

The SELECT function begins each query and FROM dictates which database you will be searching. With over 1.1 million rows of data, this database has too much data to display,which leads us to our next key phrase LIMIT, which caps the search at a specific number of rows. This is an important feature if you want to see the partial results of a larger query.

SELECT *
FROM world_bank
WHERE Country = 'Chile'
ORDER BY "Original Principal Amount"

In this second query we are expanding on the original query to both filter and sort our data.

The WHERE clause allows you to filter you data on many different criteria. In this case we are filtering for all data related to the country Chile. Additionally, we can sort our data based on principal loan amount, the standard ORDER BY syntax will sort from smallest to largest for numerical data or alphabetically for qualitative data.You can include the phrase “DESC” to sort your queries in reverse order

SELECT COUNT(*)
FROM world_bank



In addition to querying the data you can also perform calculations. One of the easiest calcualtiosn to perform is counting the records of your data. In this case, we see there are ~1.1 million records in our database. One thing to note is unless you tell SQL what to rename your columns, it will default to a very literally/ messy title from the query. Which bring us to our next command.






In addition to just counting data you can also perform calculations on the data. Let’s suppose you want to see the total amount due to the International Development Agency, you can SELECT a SUM of the entire column. 

SQL will default to naming any calculated fields exactly what is in the query, so instead of having a messy column header you can use the AS function to rename your columns. See above I have the same column twice in a row, but the second time I use AS to more conveniently rename the column. 







While I wrap up this introduction to SQL article I want to introduce two more useful functions. The group by function allows you to perform calculations on multiple criteria for a column. Instead of counting all of the records in your database, you can count each record by Region. Using the GROUP BY function most closely resembles a Pivot table in Microsoft Excel. 

Two other convenient calculations you can take from your data are MIN & MAX which as you would expect return the lowest and highest values for a column. In this example, it returns the lowest and highest values for each of the 13 regions that the world bank keeps data.

Conclusion

SQL is a great took to learn and the ebay way to get better at it is to practice practice practice with a dataset. In order to pratice, I have been working on the web browser csvfiddle.io, which allows you to 

