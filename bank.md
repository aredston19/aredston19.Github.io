# World Bank SQL Project #

For my latest Data Career Jumpstart project, I dive into the world of SQL. Last week I mentioned a few of the most important SQL commands, and in this project I show examples of how and when to use each of the functions and introduce several more. SQL is a crucial tool for data analysts when exploring large data sets. SQL allows you to manage and query your data in order to find important insights in a matter of no time. 

In this project I am analyzing data from the world bank about loans made by the International Development Agency (IDA) to different countries. The csv file contains 30 data points (columns) including: country name, project ID, loan amount, etc. for 1,109,994 records (rows). With that much data an excel workbook is incapable of performing even the most basic calculation tasks like sum, count, etc, much less trying to perform a more intensive task like a v-lookup or pivot table. The volume of this dataset makes it nearly impossible to analyze in excel, which is when SQL comes in to save the day.

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

When we turn our attention to SQL, it is important to know what we are looking for. In order to see the data we are working with we begin with the most basic of queries:


__SELECT *__

__FROM world_bank__

(returns full database)


__SELECT *__

__FROM world_bank__

__LIMIT 10__

(returns first 10 rows of the database)


<img src="images/WB_1.png?raw=true"/> 


The two most important commands and the only two required in every SQL query are SELECT & FROM. 

The SELECT function begins each query and FROM dictates which database you will be searching. With over 1.1 million rows of data, this database has too much data to display,which leads us to our next key phrase LIMIT, which caps the search at a specific number of rows. This is an important feature if you want to see the partial results of a larger query.

<img src="images/WB_8.png?raw=true"/> 

<img src="images/WB_7.png?raw=true"/> 

In this second query we are expanding on the original query to both filter and sort our data.

The WHERE clause allows you to filter you data on one or many different criteria. In this case we are filtering for all data related to the country Chile. Additionally, we can sort our data based on principal loan amount, the standard ORDER BY syntax will sort from smallest to largest for numerical data or alphabetically for qualitative data.You can include the phrase “DESC” to sort your queries in reverse order

__SELECT COUNT(*)__

__FROM world_bank__


<img src="images/WB_2.png?raw=true"/> 


In addition to querying the data you can also perform calculations. One of the easiest calcualtion sto perform is counting the records of your data. In this case, we see there are ~1.1 million records in our database. One thing to note is unless you tell SQL what to name your columns, it will default to a very literal/ messy title from the query. Which bring us to our next command.

<img src="images/WB_3.png?raw=true"/> 
<img src="images/WB_4.png?raw=true"/> 


In addition to just counting data there are many other calculations you can perform on the data. Let’s suppose you want to see the total amount due to the International Development Agency, you can SELECT a SUM of the entire column. 

SQL will default to naming any calculated fields exactly what is in the query, so instead of having a messy column header you can use the AS function to rename your columns. See above I have the same column twice in a row, but the second time I use AS to more conveniently rename the column. 

<img src="images/WB_5.png?raw=true"/> 
<img src="images/WB_6.png?raw=true"/>



While I wrap up this introduction to SQL article I want to introduce two more useful functions. The group by function allows you to perform calculations on multiple criteria for a column. Instead of counting all of the records in your database, you can count each record by Region. Using the GROUP BY function most closely resembles a Pivot table in Microsoft Excel. 

Two other convenient calculations you can take from your data are MIN & MAX which as you would expect return the lowest and highest values for a column. In this example, it returns the lowest and highest values for each of the 13 regions that the world bank keeps data.

### Conclusion ###
SQL is a great tool to learn and invaluable for data analysts, but it isn't easy to pick up right away. The best way to get better at it is to practice practice practice; speifically practice with a dataset you find interesting, that you are interested in uncovering insights about. 
SQL may seem overwhelming for someone who has never used it. If you are interested in learning SQL but don't know where to start, csvfiddle.io is a great place to begin. CSV Fiddle is a web browser that allows you to upload a csv file and begin practicing SQL without needing to download any applications to your computer. 

