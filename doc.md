# COLUMN-ORIENTED DATABASE

Traditional relational databases are row-oriented, with each row having a row-id and each field within the row stored together in a table. 
Every time you look something up in a row-oriented database, every row is scanned, regardless of which columns you require. 

# Time-series data
Time series data is a set of values that is organized by hours. Examples of time series data include sensor data, stock quotes, click sequence data, and application telemetry data. Time series data can be analyzed to search for historical trends, real-time alerts, or for predictive modeling.

Time series data represents how a resource or process changes over time. Data is time-stamped, but more importantly, time is the most significant axis for viewing or analyzing data. Typically, time series data arrives in chronological order and is usually treated as an insert rather than an update to the database. For this reason, change is measured over time, allowing you to look back and predict future changes. Therefore, time series data is best viewed with scatter or line charts.




### Situations to use it
Choose a time series solution when you need to ingest data whose strategic value focuses on changes over a period of time, and you're mostly inserting new ones and updating them only on rare occasions, if they ever update. You can use this information to detect anomalies, visualize trends, and compare current data with historical data, among other things. This type of architecture is also ideal for predictive modeling and forecasting results, since it has the historical record of changes over time, which can be applied to any number of forecasting models.
The use of time series offers the following advantages:
They clearly represent how a resource or process changes over time.
They help to quickly detect changes in a number of related sources, making it easy to highlight anomalies and emerging trends clearly.
Best suited for predictive modeling and forecasting.


### DataBases:
OpenTSDB is a distributed and scalable time series database. This database introduces concepts such as metrics and labels, and designs a set of data models for time series scenarios. It uses HBase as storage in the underlying layer and adopts the special row key design based on characteristics of time series scenarios to improve the ability to aggregate and query time series data.

TimescaleDB is a time series SQL database that presents a specific schema and manages table fragments by time. The underlying TimescaleDB layer is based on PostgreSQL.

Microsoft Time Series Insight (preview) provides a fully managed end-to-end storage and query solution for highly contextualized IoT scale data optimized for time series. Its powerful visualization enables interactive ad-hoc data analysis and asset-based data reporting.
In addition, this service supports warm data analysis and raw data analysis by data types. Users are billed separately for storage and queries used.

Timestream is applicable in scenarios like IoT and application operations.
Provides an adaptive query processing engine to quickly analyze data, automatically summarize, retain, layer, and compress data. Timestream users are billed separately for writes, stored data, and scanned query data and can achieve efficient administration with this serverless service.

|  |column-oriented databases  |
|--|--|
| Benefits | High performance on aggregation queries (like COUNT, SUM, AVG, MIN, MAX) <br> Highly efficient data compression and/or partitioning<br>True scalability and fast data loading for Big Data<br>Accessible by many 3rd  party BI analytic tools <br> Fairly simple systems administration
| advantages for certain types of systems|Data Warehouses and Business Intelligence<br>Customer Relationship Management (CRM)<br>Library Card Catalogs<br>Ad hoc query systems
|Disadvantages|Transactions are to be avoided or just not supported<br>Queries with table joins can reduce high performance<br> Record updates and deletes reduce storage efficiency<br> Effective partitioning/indexing schemes can be difficult to design
|DB|[SAP Sybase IQ](https://www.sap.com/index.html)<br>[Infobright](http://www.ignitetech.com/solutions/information-technology/infobrightdb)<br>[Vertica (HP)](https://www.vertica.com/)<br>[ParAccel](https://www.actian.com/)<br>[Microsoft SQL Server](https://www.microsoft.com/)

**References**
- [dzone](https://dzone.com/articles/nosql-database-types-1#:~:text=There%20are%20four%20big%20NoSQL,are%20often%20combinations%20of%20these.)
- [dbbest](https://www.dbbest.com/blog/column-oriented-database-technologies/)
- [Microsoft](https://docs.microsoft.com/es-es/azure/architecture/data-guide/scenarios/time-series)
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDMzOTY3MDY2LC0yMDcxNjU4ODQsLTE4MT
A3MDQ2NTUsLTUzNTg2ODk4M119
-->
