# CodingChallenge

As part of a coding challenge we were tasked with loading data and making it available for querying using new tools.  This was accomplished using several of the AWS tools as well as SQL Work Bench.

AWS Components
- IAM Role
- S3 Bucket
	- This contains the two lookup files (BillingTerms, OrderPrimaryTeam) and the main Operative Finance file
- Redshift Cluster (dc1.large, single node)

Additional Components
- SQL Workbench/J 

I created one sql script that will perform the following
- Create tables for BillingTerms, OrderyPrimaryTeam, OperativeFinance
- Copy the data from the files in the S3 bucket to the Redshift database
- Unload Address data from Redshift to a file in S3
- Unload Items data from Redshift to a file in S3
