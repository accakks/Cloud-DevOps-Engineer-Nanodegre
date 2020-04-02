# Lesson 3: Storage and Content Delivery

#### Why cloud storage services?
- Durability
- Availability
- Scalibility (Vertical, Horizontal, Diagonal)

###### Storage & Database Services
- Amazon Simple Storage Service (Amazon S3)
- Amazon Simple Storage Service (Amazon S3) Glacier
- DynamoDB
- Relational Database Service (RDS)
- Redshift
- ElastiCache
- Neptune
- Amazon DocumentDB	

#### [S3](https://aws.amazon.com/s3/) and [Glacier](https://docs.aws.amazon.com/amazonglacier/latest/dev/introduction.html) 
- Amazon Simple Storage Service (or S3) is an object storage system in the cloud.
- Under storage section
- When you upload a file to S3, it gives a unique URL for that file which can be used to access that file. 
- All objects & files are stored in bucket. S3 buckets name should be globally unique, even though they live in a region.
- A single object can be up to 5 terabytes in size
- Excellent durability & availability 
- Use cases: hosting static website, content delivery, backup and recovery, archiving & big data, application data, hybrid cloud storage.
- S3 offers several [storage classes](https://aws.amazon.com/s3/storage-classes/), which are basically different access levels for your data at certain price point. 
- S3 Glacier storage class :
	- For data archiving purposes, for data you don't need to access frequently. 
	- Cheaper than S3 standard class. 
	- Data retrival slow (upto few hours) 
	- Use case: Monthly log files for audit purposes 
- S3 Acceleration can be used to enable fast, easy, and secure transfers of files over long distances between your data source and your S3 bucket.

#### [DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html)
- NoSQL database (schema-less). DynamoDB supports key-value and document data models.
- found under the Database section
- fits well with modern day applications that need to quickly scale & handle large amounts of data. 
- can handle more than 10 trillion requests per day.
- supports GET/PUT operations using a primary key.
- Fully managed , serverless (AWS manages servers, patches and upgrades)
- synchronously replicates data across three AZs in an AWS Region.

- Use cases: Lyft, Airbnb, Netflix etc. 

*_Create a NoSQL database in cloud_*

#### [Relational Database Service(RDS)](https://aws.amazon.com/rds/)
- Aids in database administration. Sits on top of database to help manage database, automating time consuming 
administrative tasks like include upgrades, patching, installs, backups, monitoring, performance checks, security, etc.
- Can manage Oracle, PostgreSQL, MySQL, MariaDB, SQL Server, Aurora.
- Features: 
	- Failover 
	- Backups
	- Restore 
	- Encryption
	- Security 
	- Monitoring
	- Data Replication
	- Ability to scale

#### [Redshift](https://docs.aws.amazon.com/redshift/latest/mgmt/welcome.html)
- Data warehousing service, help companies manage big data
- Managed service that allows you torun fast queries against your data using SQL, ETL, and BI tools. 
- It is not for transaction processing. Usually contains historical data from transactional systems.More recent transactions maybe placed in relational database.
- Redshift stores data in a column format to aid in fast querying.
- Delivers great performance by using ML
- Redshift Spectrum is a feature that enables you to run queries against data in Amazon S3.
- Redshift encrypts and keeps your data secure in transit and at rest.
- Redshift clusters can be isolated using Amazon Virtual Private Cloud (VPC).

*_create a MySQL database instance using RDS._*


