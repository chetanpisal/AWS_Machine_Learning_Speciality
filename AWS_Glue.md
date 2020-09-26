## AWS Glue• Creates catalogues of data (schemas).• Performs ETL.• Some limited ML capabilities.


AWS Glue is a fully managed extract, transform, and load (ETL) service that makes it easy to prepare and load your data for analytics. You can create and run an ETL job with a few clicks in the AWS Glue visual editor. You simply point AWS Glue to your data stored on AWS or a JDBC-compatible source and AWS Glue discovers your data and stores the associated metadata (e.g. table definition and schema) in the AWS Glue Data Catalog. Once cataloged, your data is immediately searchable, queryable, and available for ETL.

**AWS Glue requires the least amount of setup and maintenance since it is serverless, and it does not require management of the infrastructure**


Benefits

### Less hassle

AWS Glue is integrated across a wide range of AWS services, meaning less hassle for you when onboarding. AWS Glue natively supports data stored in Amazon Aurora and all other Amazon RDS engines, Amazon Redshift, and Amazon S3, as well as common database engines and databases in your Virtual Private Cloud (Amazon VPC) running on Amazon EC2.

### Cost effective

AWS Glue is serverless. There is no infrastructure to provision or manage. AWS Glue handles provisioning, configuration, and scaling of the resources required to run your ETL jobs on a fully managed, scale-out Apache Spark environment. You pay only for the resources used while your jobs are running.

### More power

AWS Glue automates much of the effort in building, maintaining, and running ETL jobs. AWS Glue crawls your data sources, identifies data formats, and suggests schemas and transformations. AWS Glue automatically generates the code to execute your data transformations and loading processes.




## Using Python Libraries with AWS Glue


You can use Python extension modules and libraries with your AWS Glue ETL scripts as long as they are written in pure Python. C libraries such as pandas are not supported at the present time, nor are extensions written in other languages.

### Zipping Libraries for Inclusion

Unless a library is contained in a single .py file, it should be packaged in a .zip archive. The package directory should be at the root of the archive, and must contain an __init__.py file for the package. Python will then be able to import the package in the normal way.

If your library only consists of a single Python module in one .py file, you do not need to place it in a .zip file.

### Loading Python Libraries in a Development Endpoint

If you are using different library sets for different ETL scripts, you can either set up a separate development endpoint for each set, or you can overwrite the library .zip file(s) that your development endpoint loads every time you switch scripts.

You can use the console to specify one or more library .zip files for a development endpoint when you create it. After assigning a name and an IAM role, choose Script Libraries and job parameters (optional) and enter the full Amazon S3 path to your library .zip file in the Python library path box.
