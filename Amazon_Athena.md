## Amazon Athena


Amazon Athena is an interactive query service that makes it easy to analyze data in Amazon S3 using standard SQL. Athena is serverless, so there is no infrastructure to setup or manage, and you can start analyzing data immediately. You don’t even need to load your data into Athena, it works directly with data stored in S3. To get started, just log into the Athena Management Console, define your schema, and start querying. Amazon Athena uses Presto with full standard SQL support and works with a variety of standard data formats, including CSV, JSON, ORC, Apache Parquet and Avro. While Amazon Athena is ideal for quick, ad-hoc querying and integrates with Amazon QuickSight for easy visualization, it can also handle complex analysis, including large joins, window functions, and arrays.


Q: What can I do with Amazon Athena?
Amazon Athena helps you analyze data stored in Amazon S3. You can use Athena to run ad-hoc queries using ANSI SQL, without the need to aggregate or load the data into Athena. Amazon Athena can process unstructured, semi-structured, and structured data sets. Examples include CSV, JSON, Avro or columnar data formats such as Apache Parquet and Apache ORC. Amazon Athena integrates with Amazon QuickSight for easy visualization. You can also use Amazon Athena to generate reports or to explore data with business intelligence tools or SQL clients, connected via an ODBC or JDBC driver.
 
Q: How do I get started with Amazon Athena?
To get started with Amazon Athena, simply log into the AWS Management Console for Athena and create your schema by writing DDL statements on the console or by using a create table wizard. You can then start querying data using a built-in query editor. Athena queries data directly from Amazon S3 so there’s no loading required.
 
Q: How do you access Amazon Athena?
Amazon Athena can be accessed via the AWS Management Console, an API, or an ODBC or JDBC driver. You can programmatically run queries, add tables or partitions using the ODBC or JDBC driver.
 
Q: What are the service limits associated with Amazon Athena?
Please click here to learn more about service limits.

 
Q: What is the underlying technology behind Amazon Athena?
Amazon Athena uses Presto with full standard SQL support and works with a variety of standard data formats, including CSV, JSON, ORC, Avro, and Parquet. Athena can handle complex analysis, including large joins, window functions, and arrays. Because Amazon Athena uses Amazon S3 as the underlying data store, it is highly available and durable with data redundantly stored across multiple facilities and multiple devices in each facility. Learn more about Presto here.
 
Q: How does Amazon Athena store table definitions and schema?
Amazon Athena uses a managed Data Catalog to store information and schemas about the databases and tables that you create for your data stored in Amazon S3. In regions where AWS Glue is available, you can upgrade to using the AWS Glue Data Catalog with Amazon Athena. In regions where AWS Glue is not available, Athena uses an internal Catalog.
You can modify the catalog using DDL statements or via the AWS Management Console. Any schemas you define are automatically saved unless you explicitly delete them. Athena uses schema-on-read technology, which means that your table definitions applied to your data in S3 when queries are being executed. There’s no data loading or transformation required. You can delete table definitions and schema without impacting the underlying data stored on Amazon S3.

Q. How Amazon Athena is priced?

With Amazon Athena, customers pay only for the queries they run ($5 per terabyte scanned). Customers can save 30–90% on per-query costs and get better performance by compressing, partitioning, and converting your data into columnar formats.
 
 