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

__Left Outer Join__ - guarantees that you get all the columns from table a, the left table, and if there is a match for table b, the right table, it will put those values - all values which are null will be filled in as null. In other words, it produces a complete set of records from Table A, with matching records from B where available.

__Right Outer Join__ - same as left outer join, but for the right table(table b).

You can also use __WHERE__ statements with these joins. Some possible use cases could be:
* ... join... on... WHERE tableB.attribute IS null -- This returns values only in Table A. Can be changed for tableB only.
* Full outer join on both tables, where either attribute is null, so you get only the unique values from both tables. Ex: SELECT... JOIN... ON... WHERE tableA.attribute IS null OR tableB.attribute IS null

## Union Statement

Combines result sets of two or more select statements into a single result set. All select queries must return the same number of columns and be of the same data type(ex int, float, string, etc.)

Removes all duplicate rows(Unless you use UNION ALL) and can be used with ORDER BY to sort results.

## Extract

Extracts parts from a date. We can extract many different units of time - day, day of week, day of year, etc. For the full table, go to [this page](https://www.postgresql.org/docs/9.6/static/functions-datetime.html).

You can also perform some computations, for example add/subtract, to times.

To use extract, find the date column in your table. When selecting, do extract(something from time_column_name), where something is the timestamp feature you want - for example - day, dow, doy, etc.

## Mathematical functions

You can look at the postgresql docs for more, but you can use most of these operators just like you do in other languages when querying.

You could also do
* SUM
* AVG
* round
* etc

## String functions

Look at postgresql docs (functions string postgresql) for more.

Concatenation: col1 || col2 -- returns concatenation. Can be called with multiple strings(more than 2), and you can concatenate your own strings into there too - i.e col1 || ' randomconcat ' || col2.

Char length - you can add this as a column in your select statement to add the length of the string you are returning. ex - char_length(col1)

Lower and upper - lower(col1) and upper(col1) returns lower and upper of col1 respectively.

Can also use LIKE as shown earlier.

## Subqueries

A query which is nested inside another query. We put the second query in brackets and use it in the WHERE class as an expression.

Order of execution:
* Executes subquery
* Passes result to outer query
* Outer query is then executed

## Self-Join

A special case of join where you can join a table to itself.

When you want to combine rows from the same table.

You need to use aliases when using a self-join. To further define how this code works : We create two aliases of the same table - when calling FROM, we say ' ... FROM tablename AS t1, tablename AS t2', then refer to the info from the different tables as t1 and t2. You would then use a WHERE statement to further refine your search. This allows us to treat the same table as if we are inner-joining among two different tables, and access info separately without using complicated sub-queries.

You could also do the same query using an inner join, left join, or right join, and then just calling the same table as a second table. This may not make sense for all cases.

This tactic is also more efficient than using sub-queries.

## Data Types

* Boolean
* Characters : fixed length character strings - char(n), or Variable length character strings - varchar(n)
* Number : small int, int, serial - automatically populating, float(n), real or float8, numeric(p,s) - for exact
* Temporal : date, time, timestamp, interval, timestamps

## Primary/Foreign Keys
* A Primary key is a column / group of columns that is used to uniquely identify a row in a table. They are defined through primary key constraints. A table can have only 1 primary key.
* Foreign key - a field / group of fields in one table which happens to be the primary key of another. The table that contains the foreign key is called the referencing table, and the table which the foreign key references is called the referenced table. A table can have multiple foreign keys. You need a foreign constraint to define this foreign key.

## Creating a table

CREATE TABLE table_name(column_name DATA_TYPE column_constraint, table_constraint) INHERTIS existing_table

Column Constraints - NOT NULL, UNIQUE, CHECK, PRIMARY KEY

Or, you could copy the structure(but not the data) of another table by doing:

CREATE TABLE table_copy (LIKE table);

## Inserting rows into a table

The command INSERT is used to insert rows into the table.

INSERT INTO table_name(column1, column2, ...) VALUES (value1, value2, ...);

Note : You can leave these null, but only if that column accepts null values

Toadd multiple rows, do INSERT INTO ... VALUES (value1, value2, ...), VALUES (value1, value2, ...), ... ;

To insert data that comes from another table, use the INSERT INTO SELECT statement:

INSERT INTO table_name SELECT column 1, column2, ... FROM another_table WHERE ...;

Note : The where statement can be left removed.

If, when inserting, you do not put data for columns which accept null, the table will set null as a default value for all future insertions which lack that column. You can also set the default value of a column,
