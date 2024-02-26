# Introduction 
This repo contains ADF pipelines to perform migration of data from on-prem sql server to azure sql server.
Pipeline:
1) pl-onprem-sqlserver-bulkload.json - This pipeline is used to bulk-load data from on-prem to cloud.
2) pl-onprem-sqlserver-incremental.json - This pipeline is used to incrementally load update data from on-prem to cloud. To insure upsert, I've used watermark table which gets updated with the maximum created_at time at time of every load.
