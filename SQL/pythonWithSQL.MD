First, you want to import.

*import psycopg2 as pg2*

Now, connect to your database. This assumes you use default settings

*conn = pg2.connect(database = 'database_name', user = 'postgres')*

We now need to retrieve the cursor, which allows for SQL data retrieval.

*cur = conn.cursor*

Now, we can execute SQL queries as wanted - replace 'Query' with a string which contains your query in SQL.

*cur.execute('Query')*

Now, if your query worked, you can do these commands to fetch some of the returned data:

*cur.fetchall()*

*cur.fetchone()*

*cur.fetchmany(n)* # How many values we want to fetch

When you are all done, do:

*conn.close()*

to terminate the connection to the database.

Now, you could assign these values to variables, and then use indexes to access certain data points and such as values.

Think of this as the pandas for SQL - this allows us to get and use .tar files in python code. We can even convert this data into a pandas dataframe if wanted, which would make applications such as machine learning quite easy.

Also note that you could easily destroy your data with commands such as Drop Table if you are not careful.
