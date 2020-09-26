## The Kinesis Family

** Kinesis Data Streams

It partition data into Shards (1 - 500 shards default limit)

• Each shard consists of a sequence of data records. These can be ingested at 1000 records per second.• Default limit of 500 shards, but you can request increase to unlimited shards.• A data record is the unit of data captured.• sequence number• partition key• data blob (your payload, up to 1 MB)• Transient Data Store - retention period for the data records are 24 hours to 7 days.

Interacting With Kinesis Data Streams1. _Kinesis Producer Library (KPL)_. Easy to use library that allows you to write to a Kinesis Data Stream.  Java Wrapper2. _Kinesis Client Library (KCL_ Integrated directly with KPL for consumer applications to consume and process data from Kinesis DataStream.3. _Kinesis API (AWS SDK)_ Used for low level API operations to send records to a Kinesis Data Stream.  Any AWS SDK


Data Consumers would be _EC2, Lambda, Kinesis Data Analytics, EMR Apache Spark_

Storage and Analyzation - _S3, DynamoDB, RedShift, BI tools_


When should you useKinesis Data Streams?
• Needs to be processed by consumers.• Real time analytics.• Feed into other services in real time.• Some action needs to occur on your data.• Storing data is optional.• Data retention is important.

Kinesis Data Streams - Use Cases• Process and evaluate logs immediatelyExample: Analyze system and application logs continuously and process within seconds.• Real-time data analyticsExample: Run real-time analytics on click stream data and process it within seconds.



** Kinesis Data Firehose

Processing Tools (Optional) - Lambda

Storage - S3 event to DynamoDB, RedShift


When should you use Kinesis Data Firehose?• Easily collect streaming data.• Processing is optional.• Final destination is S3 (or other data store).• Data retention is not important.


Kinesis Data Firehose - use cases

• Stream and store data from devicesExample: Capturing important data from IoT devices, embedded systems, consumer applications and storing it into a data lake.• Create ETL jobs on streaming dataExample: Running ETL jobs on streaming data before data is stored into a data warehousing solution.



** Kinesis Video Streams

When should you use Kinesis Video Streams?• Needs to process real-time streaming video data (audio, images, radar).• Batch-process and store streaming video.• Feed streaming data Kinesis into other AWS services

** Kinesis Data Analytics

When should you use Kinesis Data Analytics?• Run SQL queries on streaming data.• Construct applications that provide insight on your data.• Create metrics, dashboards, monitoring, notifications, and alarms.• Output query results into S3 (other AWS datasources)

Kinesis Data Analytics - Use Cases• Responsive real-time analyticsExample: Send real-time alarms or notifications when certain metrics reach predefined threshold.• Stream ETL jobsExample: Stream raw sensor data then, clean, enrich, organize, and transform it before it lands into data warehouse or data lake.



_Kinesis Data Streams and Kinesis Data Analytics cannot write data directly to S3. Kinesis Data Firehose is used as the main delivery mechanism for outputting data into S3. You can also use Lambda to write data into S3_



