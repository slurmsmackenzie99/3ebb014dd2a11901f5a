> Ogólne

*.lock files in the package manager (NPM/Yarn/Composer) are used to make sure that all people working on the project are *locked* with the same versions of the packages installed for the project. This makes sure that there's no bugs caused by different package versions used between the team members.

> Backend

Indexes, in short, are a form of mapping/structuring the data in the database which vastly increases the speed in which it can be looked up/retrieved. The basis of their work is that they store a primary key (usually, although the indexed field can also be a non-primary key, or there can be a second indexed field, then it'd be called a compound index) and a pointer to the row. During a query this index table (consisting of indexed field and a pointer) is used to scan through the records and retrieve data faster.

> Key / Index

Key and index in the table and synonymous but it's possible to create a table where the indexed field is not a primary key (although it's not usually the case).

> Types of indexes

The types of indexes that I'm aware of are: 
 - clustered
 If you add a primary key to a table it becomes a clustered index. Clustered index means the data is indexed and sorted in a sequential order.

 - non-clustered
 (never used those so had to look up) Whereas the clustered index stores a primary key and a pointer to the block, the non-clustered index stores a field value and a pointer to the actual row. It results in it taking more memory on disk. It's also slower than using a clustered index.

> When to use non-clustered indexes

 Non-clustered index would be used when there's more than one field that's indexed, because there can only be one clustered index per table.