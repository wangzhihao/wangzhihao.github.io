---
layout: post
title:  "How to export DDB to s3?"
categories: articles 
---
How to export DDB data effciently to daily snapshots?


Daily scan the whole DDB table is very ineffcient and expensive. Obsolete ways:

1. https://github.com/audienceproject/spark-dynamodb
1. https://github.com/awslabs/emr-dynamodb-connector

Publish delta and do some compactions sounds promising.

PITR sounds promising:

1. https://aws.amazon.com/blogs/aws/new-export-amazon-dynamodb-table-data-to-data-lake-amazon-s3/
1. https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/S3DataExport.HowItWorks.html


