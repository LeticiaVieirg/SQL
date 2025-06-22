# Aggregate functions are used to perform calculations and return a single value.

The most common aggregate functions are:

- COUNT(): returns the number of rows.
- MAX(): returns the largest value in a column.
- MIN(): returns the smallest value in a column.
- SUM(): returns the total sum in a column.
- AVG(): returns the average value in a column.

``` sql
SELECT *
FROM playlist;
```

-----

## Count
COUNT() function counts the numbers of rows.

``` sql
SELECT COUNT(*)
FROM table_name;
```

## Big & Small
MIN() and MAX() return the minimum and maximum value in a columm.

Return the smallest value in the plays column.
``` sql
SELECT MIN(plays)
FROM playlist;
```

Return the most popular song in the table.
``` sql
SELECT title, artist, MAX(plays)
FROM playlist;
``` 

## Sum
The SUM() aggregate function takes a column and returns the total sum of the values in it.

Find the totak listens of the whole playlist.
``` sql
SELECT SUM(plays)
FROM playlist;
``` 

## AVG
The AVG() is used to calculate the average value od a column.
``` sql
SELECT AVG(plays)
FROM playlist;
```

## GROUP BY
The GROUP BY it's often used with aggregate functions to group the result by one or more columns.
Usinf find all the diferent artists and their average number of plays in two columns.

``` sql
SELECT AVG(plays)
FROM playlist;
```





