https://dzone.com/articles/nosql-database-types-1#:~:text=There%20are%20four%20big%20NoSQL,are%20often%20combinations%20of%20these.

COLUMN-ORIENTED DATABASE

Traditional relational databases are row-oriented, with each row having a row-id and each field within the row stored together in a table. Let’s say, for example’s  sake, that no extra data about hobbies is stored and you have only a single table to  describe people, as shown in figure 6.8. Notice how in this scenario you have slight denormalization because hobbies could be repeated. If the hobby information is a nice extra but not essential to your use case, adding it as a list within the Hobbies column is an acceptable approach. But if the information isn’t important enough for a separate table, should it be stored at all?

Every time you look something up in a row-oriented database, every row is scanned, regardless of which columns you require. 
|  |column-oriented databases  |
|--|--|
| Benefits | High performance on aggregation queries (like COUNT, SUM, AVG, MIN, MAX) <br> Highly efficient data compression and/or partitioning<br>True scalability and fast data loading for Big Data<br>Accessible by many 3rd  party BI analytic tools <br> Fairly simple systems administration
| advantages for certain types of systems|Data Warehouses and Business Intelligence<br>Customer Relationship Management (CRM)<br>Library Card Catalogs<br>Ad hoc query systems
||
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MTA3MDQ2NTUsLTUzNTg2ODk4M119
-->