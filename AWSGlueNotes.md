#AWS Glue

http://aws-glue-beta-documentation.s3-website-us-west-2.amazonaws.com/glue-dg.pdf

https://console.aws.amazon.com/glue


## Notes:
- Initial setup based on the DG done
	- and it created and ran a job!
- crawler created table with the 
	- PREFIX
	- Bucket Name
	ex: src_gluedata
- job created output file
	- did *not* register the table in catalog
	- default name
		run-1499485602698-part-r-00000

## To Understand
[ ] Transforms!
	[ ] Spigot - for debugging
		- how to easily query the JSON file?
		- where should these sampled files go?
	[ ] SplitRows?
		- for QA?  you could move questionable rows out?
[ ] Logs
	- all in Cloudwatch!
	- separate Glue project that just deals with Cloudwatch logs? SelfReferencing?
[ ] ## Script annotations
	- to create good diagrams
[ ] How to export out job diagrams
[ ] Set up a Development Endpoint and Notebook to Interactively Author ETL Scripts
[ ] Job filter data based on S3 Tags?
[ ] Code in S3 Bucket - S3 versioning? or GitHub?
[ ] Data "libraries" management
	- S3 Data Events?
[ ] Glue and Cloudwatch logs


## Questions:
[ ] Is the catalog queryable ?
	- is the hive metastore in an accessible MySQL db?
[ ] Is there a way to customize the crawler table names other than just "prefix" ?
[ ] How to review the "lineage of your data"?
[ ] How to use S3 properly
	- code tables?
	- simple data tables?
	- large, partitioned tables?
[ ] How to set up VPC and S3 Endpoint
	- would want to do this
[ ] Is there only 1 Glue project?  Don't remember creating one.
[ ] How to schedule Enterprise - cron?


## Feedback:
1. latest change date on the developer guide
	- reply
2. Default Target Table
3. Organization of jobs


## Team
- GitHub? - each our own

## To Diagram
[ ] Security and structure
	- IAM roles and accounts
	- including VPC, S3, Roles
[ ] Framework
	- structure of S3 in relation to sources and final targets
	- a structure for jobs



## S3 Structure
Rules:
	Never update; write new key and delete old as required
	MetData;	
		S3EMPER - Netflix OSS (or dynamo)
		MetaCat - Netflix OSS (
	Parquet format;
	

CODE:
	- main
	- Python libary path
	- Referenced files path


TEMP:

SOURCE DATA:


LOAD DATA





