
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
