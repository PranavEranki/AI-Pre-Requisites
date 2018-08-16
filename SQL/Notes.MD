## Some general commands

SELECT
* SELECT
* SELECT DISTINCT - unique values only
* SELECT WHERE - conditional

AGGREGATE FUNCTIONS
* COUNT - count(____) - displays # of rows
* MIN
* MAX
* SUM
* AVG

OTHER FUNCTIONS
* LIMIT - max rows displayed
* ORDER BY - column(s), asc/desc
* GROUP BY - groups rows by an aggregate function
* ROUND( ____,decimal places)
* HAVING (like where, but with group by - targets rows)
* AS - returns something as another name - think of it as renaming


## WHERE Operators
* '='	- Equal
* '<>' - Not equal. Note: In some versions of SQL this operator may be written as !=
* '>' - Greater than
* '<' - Less than
* '>=' - Greater than or equal
* '<=' - Less than or equal
* 'BETWEEN' - Between an inclusive range
* 'LIKE' - Search for a pattern
* 'IN' - To specify multiple possible values for a column

## Joins
__Inner joins__ - multiple tables, getting data from both:
Select columns in both tables from main table, join on secondary table based on some attributes. Produces only data that matches in both tables.

SELECT tablename.column, tablename2.column, etc

FROM tablename

INNER JOIN tablename2 ON tablename.column = tablename2.column;

__Full Outer Join__ - produces all the data from both tables, merging similar values and putting null for the missing side if there is no match.
Returns absolutely everything

__Left Outer Join__ - gaurantees that you get all the columns from table a, the left table, and if there is a match for table b, the right table, it will put those values - all values which are null will be filled in as null. In other words, it produces a complete set of records from Table A, with matching records from B where available.

__Right Outer Join__ - same as left outer join, but for the right table(table b).

You can also use __WHERE__ statements with these joins. Some possible use cases could be:
* ... join... on... WHERE tableB.attribute IS null -- This returns values only in Table A. Can be changed for tableB only.
* Full outer join on both tables, where either attribute is null, so you get only the unique values from both tables. Ex: SELECT... JOIN... ON... WHERE tableA.attribute IS null OR tableB.attribute IS null
