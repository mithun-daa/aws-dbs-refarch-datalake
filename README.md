---
description: >-
  This page provides an overview of what is a data lake and provides a high
  level blueprint of a data lake on AWS.
---

# Overview of a Data Lake on AWS

## Data lake Overview

A [**data lake**](https://en.wikipedia.org/wiki/Data_lake) is a data repository that stores data in its raw format until it is used for analytics. It is designed to store massive amount of data at scale. A schema to the dataset in data lake is given as part of transformation while reading it. Below is a pictorial representation of a typical datalake on AWS cloud.

![A datalake blueprint on AWS](.gitbook/assets/image%20%281%29.png)

Data lakes are ideally designed with the following characteristics:

* [**Secure**](https://en.wikipedia.org/wiki/Data_security) – Datalakes must implement strong security to enable broad adoption across your business. data lakes must implement strong [Identity](https://aws.amazon.com/iam) controls, enable Fine Grained Access to data, and support encrypting your data. 
* **Centralized:**  Data lakes are designed to logically access all data using a single service that enables  sharing of data across your Orgainsations or Business Units. Those business units may also have their own private data lakes. However,  any consumer with right permissions should be able to consume data across one or more such data lake in a consistent manner. 
* **Flexible:** Data lakes will capture data from any source system, including Relational and NoSQL databases, audio/video files, log files, free-form text, or any other type of data managed by your applications. They store structured, semi-structured and unstructured data in the same format as it is generated in the source systems, and provide a way to access data where the format and structure of the data are not defined until the data is queried: “just in time” or “**schema on read**”
* **Cost Effective:** Data lakes store a virtually unlimited amount of data in any format inexpensively, and provide you looking to manage the data lifecycle for cost optimisation, as well as offering cost transparency.
* **An Analytics Ecosystem Foundation:** Data lakes are foundations of enterprise analytics architecture. It is designed to be the one stop data repository for all analytic systems as well as users to  discover and consume  datasets to drive business outcomes.
* **Decoupled from Compute:** – In traditional big data and data warehouse solutions, storage and compute are tightly coupled in a way that can limit scalability. With a datalake, you store, secure, and index your data to enable data exploration by a virtually unlimited number of clients. These customers may run Big Data Ecosystem Tools on multiple [Amazon EMR](https://aws.amazon.com/emr/) clusters, run serverless queries with [Amazon Athena](https://aws.amazon.com/athena), [Amazon Redshift](https://aws.amazon.com/redshift) or [AWS Glue](https://aws.amazon.com/glue), or use legacy analytics tools on [Amazon Elastic Compute Cloud \(EC2\)](https://aws.amazon.com/ec2).
* **Integrated:** – Your datalake should enable exploration by virtually any analytical tool, and support access using common an open data formats and API's

### Is centralized data lake built using a single AWS account?

The direct answer is "NO". Centralized data lake doesn't mean a single S3 bucket, single data catalog within a single AWS account. What it exactly means is, even though  your data lakes are physically decentralized across many accounts, storage services and catalogs, you still have a centralized governance process that can be configured to support different analytics tools, data access controls and lifecycle policies.Your primary goal is to have a single threaded ownership for governance of each dataset and friction-less data access for data consumers across multiple business domains within the organization. 

## Have suggestions? Join our [Slack channel](https://join.slack.com/t/cat-cwp4274/shared_invite/zt-e2ztjpgw-Bugw46iXsLbZ~V54AljWsA) to  share feedback.

