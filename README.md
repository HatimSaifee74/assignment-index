Provide the answers with proper examples: 
1. You have primary key (Oracle creates default index on a primary key) as well as user created index 
on the same table then which index will fire?
Ans: Ok, so basically if we try to create index on primary key it will not allow us and it will say “such 
column list already indexed” because primary key is already implicitly indexed.
If the other column is indexed .Than the index fired will depend on the data the query and the 
statistics.
2. Is it possible to create an index on views? 
Ans: Oracle SQL standards do not support creating indexes on views. But we can use unique 
clustered index which can be created on a view, it is stored in the database just like a table with a 
clustered index.
3. Is it possible to create an index on updatable views? 
Ans: No, index can’t be created on updatable views.
4. Index makes searching fast explain how? 
Ans: what index does is create a sorted list based on attribute indexed without creating a new 
table . So instead of doing a linear search for required search it applies binary search which 
complets the search in O(logn).It creates a binary tree and performs the search much faster.
5. When to use Function-based index? 
Ans: we use function based index when we need to improve the performance of a particular query 
which uses that function in it.
6. How does a database know when to use an index? 
Ans: Indexes are used to quickly locate data without having to search every row in a database table 
every time a database table is accessed. It cut down the number of rows/records that need to be 
examined when a select query with a where clause is executed.
7. How many clustered indexes can be created on a table? 
Ans: There can be only one clustered index per table, because the data rows themselves 
can be stored in only one order.
8.If we create separate index on each column of a table, what are the advantages or disadvantages of 
the same? 
Ans: Disadvantage of creating index on each attributes are that 
• Additional Disk Space: clustered index does not require any additional 
disk space, but non-clustered index requires additional space for each 
indexed column because of which amount of storage complexity 
increases.
• DML Becomes Slow: Another drawbacks is that data modification
becomes slow as database needs to perform the command all the 
indexes along with table .
Advantages of creating on index is that it can query and retrieve data very fast.
9.Can we create clustered index on a column containing duplicate values? 
Ans: Yes, we can create clustered index on column containing duplicate values.
10.Can we create a Primary Key on a table on which a clustered index is already defined? 
Ans: There is no clustered index in oracle ,But there is index organized table (IOT) which has almost 
same functionalities as clusterd index. We can create clustered index on the columns on which primary 
key is not defined in sql.
