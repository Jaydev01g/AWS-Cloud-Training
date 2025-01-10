# AWS ANALYTICS SERVICES

The are several AWS Analytics services and these include:
• Amazon Athena
• Amazon EMR
• Amazon CloudSearch
• Amazon Elasticsearch Service
• Amazon Kinesis
• Amazon QuickSight
• Amazon Data Pipeline
• AWS Glue
• AWS Lake Formation
• Amazon MSK
In this article we will focus on Athena, EMR, Glue and Kinesis as these are the services that 
are most likely to come up on the AWS Certified Cloud Practitioner exam. You may also 
want to follow the links to the other services and read up to understand what they are at a 
high-level.

## AMAZON ELASTIC MAP REDUCE
Amazon EMR is a web service that enables businesses, researchers, data analysts, and 
developers to easily and cost-effectively process vast amounts of data.
EMR utilizes a hosted Hadoop framework running on Amazon EC2 and Amazon S3.
Managed Hadoop framework for processing huge amounts of data.
Also support Apache Spark, HBase, Presto and Flink.
Most commonly used for log analysis, financial analysis, or extract, translate and loading 
(ETL) activities.
A Step is a programmatic task for performing some process on the data (e.g. count words).
A cluster is a collection of EC2 instances provisioned by EMR to run your Steps.
EMR uses Apache Hadoop as its distributed data processing engine, which is an open 
source, Java software framework that supports data-intensive distributed applications 
running on large clusters of commodity hardware.
EMR is a good place to deploy Apache Spark, an open-source distributed processing used 
for big data workloads which utilizes in-memory caching and optimized query execution.
You can also launch Presto clusters. Presto is an open-source distributed SQL query engine 
designed for fast analytic queries against large datasets.
EMR launches all nodes for a given cluster in the same Amazon EC2 Availability Zone.
You can access Amazon EMR by using the AWS Management Console, Command Line 
Tools, SDKS, or the EMR API.
With EMR you have access to the underlying operating system (you can SSH in).

## AMAZON ATHENA
Amazon Athena is an interactive query service that makes it easy to analyze data in 
Amazon S3 using standard SQL.
Athena is serverless, so there is no infrastructure to manage, and you pay only for the 
queries that you run.
Athena is easy to use – simply point to your data in Amazon S3, define the schema, and 
start querying using standard SQL.
Amazon Athena uses Presto with full standard SQL support and works with a variety of 
standard data formats, including CSV, JSON, ORC, Apache Parquet and Avro.
While Amazon Athena is ideal for quick, ad-hoc querying and integrates with Amazon 
QuickSight for easy visualization, it can also handle complex analysis, including large joins, 
window functions, and arrays.
Amazon Athena uses a managed Data Catalog to store information and schemas about the 
databases and tables that you create for your data stored in Amazon S3.

## AWS GLUE
AWS Glue is a fully managed, pay-as-you-go, extract, transform, and load (ETL) service that 
automates the time-consuming steps of data preparation for analytics.
AWS Glue automatically discovers and profiles data via the Glue Data Catalog, 
recommends and generates ETL code to transform your source data into target schemas.
AWS Glue runs the ETL jobs on a fully managed, scale-out Apache Spark environment to 
load your data into its destination.
AWS Glue also allows you to setup, orchestrate, and monitor complex data flows.
You can create and run an ETL job with a few clicks in the AWS Management Console.
Use AWS Glue to discover properties of data, transform it, and prepare it for analytics.
Glue can automatically discover both structured and semi-structured data stored in data 
lakes on Amazon S3, data warehouses in Amazon Redshift, and various databases running 
on AWS.
It provides a unified view of data via the Glue Data Catalog that is available for ETL, 
querying and reporting using services like Amazon Athena, Amazon EMR, and Amazon 
Redshift Spectrum.
Glue automatically generates Scala or Python code for ETL jobs that you can further 
customize using tools you are already familiar with.
AWS Glue is serverless, so there are no compute resources to configure and manage.
DATA ANALYSIS AND QUERY USE CASES
Query services like Amazon Athena, data warehouses like Amazon Redshift, and 
sophisticated data processing frameworks like Amazon EMR, all address different needs 
and use cases.
Amazon Redshift provides the fastest query performance for enterprise reporting and 
business intelligence workloads, particularly those involving extremely complex SQL with 
multiple joins and sub-queries.
Amazon EMR makes it simple and cost effective to run highly distributed processing 
frameworks such as Hadoop, Spark, and Presto when compared to on-premises 
deployments. Amazon EMR is flexible – you can run custom applications and code, and 
define specific compute, memory, storage, and application parameters to optimize your 
analytic requirements.
Amazon Athena provides the easiest way to run ad-hoc queries for data in S3 without the 
need to setup or manage any servers.
The table below shows the primary use case and situations for using a few AWS query and 
analytics services:![image](https://github.com/user-attachments/assets/b7552fb3-3ddf-49fe-9377-1c6641abe516)

## AMAZON KINESIS
Amazon Kinesis makes it easy to collect, process, and analyze real-time, streaming data so 
you can get timely insights and react quickly to new information.
Collection of services for processing streams of various data.
Data is processed in “shards”.
ThereKINESIS VIDEO STREAMS
Kinesis Video Streams makes it easy to securely stream video from connected devices to 
AWS for analytics, machine learning (ML), and other processing.
Durably stores, encrypts, and indexes video data streams, and allows access to data 
through easy-to-use APIs.
Producers provide data streams.
Stores data for 24 hours by default, up to 7 days.
Consumers receive and process data.
Can have multiple shards in a stream.
Supports encryption at rest with server-side encryption (KMS) with a customer master key.

### KINESIS DATA STREAMS
Kinesis Data Streams enables you to build custom applications that process or analyze 
streaming data for specialized needs.
Kinesis Data Streams enables real-time processing of streaming big data.
Kinesis Data Streams is useful for rapidly moving data off data producers and then 
continuously processing the data.
Kinesis Data Streams stores data for later processing by applications (key difference with 
Firehose which delivers data directly to AWS services).
Common use cases include:
• Accelerated log and data feed intake.
• Real-time metrics and reporting.
• Real-time data analytics.
• Complex stream processing.

### KINESIS DATA FIREHOSE
Kinesis Data Firehose is the easiest way to load streaming data into data stores and 
analytics tools.
Captures, transforms, and loads streaming data.
Enables near real-time analytics with existing business intelligence tools and dashboards.
Kinesis Data Streams can be used as the source(s) to Kinesis Data Firehose.
You can configure Kinesis Data Firehose to transform your data before delivering it.
With Kinesis Data Firehose you don’t need to write an application or manage resources.
Firehose can batch, compress, and encrypt data before loading it.
Firehose synchronously replicates data across three AZs as it is transported to destinations.
Each delivery stream stores data records for up to 24 hours.
 are four types of Kinesis service, and these are detailed below.

### KINESIS DATA ANALYTICS
Amazon Kinesis Data Analytics is the easiest way to process and analyze real-time, 
streaming data.
Can use standard SQL queries to process Kinesis data streams.
Provides real-time analysis.
Use cases:
• Generate time-series analytics.
• Feed real-time dashboards.
• Create real-time alerts and notifications.
Quickly author and run powerful SQL code against streaming sources.
Can ingest data from Kinesis Streams and Kinesis Firehose.
Output to S3, RedShift, Elasticsearch and Kinesis Data Streams.
Sits over Kinesis Data Streams and Kinesis Data Firehose.

## AWS ANALYTICS SERVICES QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: Which service can be used to analyze data on Amazon S3 using serverless 
SQL queries?
1. Amazon Kinesis
2. Amazon Athena
3. AWS Glue
4. AWS Lambda

Question 2: A company has many manufacturing facilities with sensors that send 
environmental information. Which service can ingest and process the data?
1. Amazon Kinesis
2. AWS Glue
3. AWS Data Pipeline

Question 3: A company needs an interactive dashboard for business intelligence. What 
should they use?
1. Amazon CloudWatch
2. AWS CloudTrail
3. Amazon QuickSight



# APPLICATION INTEGRATION SERVICES
The AWS application integration services are a family of services that enable decoupled 
communication between applications.
These services provide decoupling for microservices, distributed systems, and serverless 
applications. 
AWS application integration services allow you to connect apps, without needing to write 
custom code to enable interoperability.
Decoupled applications can interoperate whilst being resilient to the failure or overload of 
any individual component.
The following services are involved with application integration:
Service What it does Example use cases
Simple Queue 
Service (SQS)
Messaging queue; store and 
forward patterns
Building distributed / decoupled 
applications
Simple 
Notification 
Service (SNS)
Set up, operate, and send 
notifications from the cloud
Send email notification when 
CloudWatch alarm is triggered
Step Functions Out-of-the-box coordination 
of AWS service components 
with visual workflow
Order processing workflow
Simple 
Workflow 
Service (SWF)
Need to support external 
processes or specialized 
execution logic
Human-enabled workflows like an 
order fulfilment system or for 
procedural requests
Amazon MQ Message broker service for 
Apache Active MQ and 
RabbitMQ
Need a message queue that 
supports industry standard APIs and 
protocols; migrate queues to AWS

## AMAZON SIMPLE NOTIFICATION SERVICE
Amazon Simple Notification Service (Amazon SNS) is a web service that makes it easy to set 
up, operate, and send notifications from the cloud.
Amazon SNS is used for building and integrating loosely-coupled, distributed applications.
SNS provides instantaneous, push-based delivery (no polling).
SNS concepts:
• Topics – how you label and group different endpoints that you send messages to.
• Subscriptions – the endpoints that a topic sends messages to.
• Publishers – the person/alarm/event that gives SNS the message that needs to be 
sent.
SNS usage:
• Send automated or manual notifications.
• Send notification to email, mobile (SMS), SQS, and HTTP endpoints.
• Closely integrated with other AWS services such as CloudWatch so that alarms, 
events, and actions in your AWS account can trigger notifications.
Uses simple APIs and easy integration with applications.
Flexible message delivery is provided over multiple transport protocols.
Offered under an inexpensive, pay-as-you-go model with no up-front costs.
The web-based AWS Management Console offers the simplicity of a point-and-click 
interface.
Data type is JSON.
SNS supports a wide variety of needs including event notification, monitoring applications, 
workflow systems, time-sensitive information updates, mobile applications, and any other 
application that generates or consumes notifications.
SNS Subscribers:
• HTTP.
• HTTPS.
• Email.
• Email-JSON.
• SQS.
• Application.
• Lambda.
SNS supports notifications over multiple transport protocols:
• HTTP/HTTPS – subscribers specify a URL as part of the subscription registration.
• Email/Email-JSON – messages are sent to registered addresses as email (text-based 
or JSON-object).
• SQS – users can specify an SQS standard queue as the endpoint.
• SMS – messages are sent to registered phone numbers as SMS text messages.
Topic names are limited to 256 characters.
SNS supports CloudTrail auditing for authenticated calls.
SNS provides durable storage of all messages that it receives (across multiple AZs).

## AMAZON SIMPLE QUEUE SERVICE (AMAZON SQS)
Amazon Simple Queue Service (SQS) is a distributed queue system.
Amazon SQS enables you to send, store, and receive messages between software 
components.
An Amazon SQS queue is a temporary repository for messages that are awaiting 
processing.
The SQS queue acts as a buffer between the component producing and saving data, and 
the component receiving the data for processing.
![image](https://github.com/user-attachments/assets/063b0039-c774-4a90-a149-b5fe5ce98cff)
This is known as decoupling / loose coupling and helps to enable elasticity for your 
application.
Amazon SQS is pull-based, not push-based (like Amazon SNS).

## AMAZON SIMPLE WORKFLOW SERVICE 
(AMAZON SWF)
Amazon Simple Workflow Service (SWF) is a web service that makes it easy to coordinate 
work across distributed application components.
Amazon SWF is used for processing background jobs that have parallel or sequential steps. 
You can think of Amazon SWF as a fully managed state tracker and task coordinator.
Use Amazon SWF if your app’s steps take more than 500 milliseconds to complete, you 
need to track the state of processing, or you need to recover or retry if a task fails.
With SWF you can create distributed asynchronous systems as workflows.
Tracks the state of your workflow which you interact and update via API.
Best suited for human-enabled workflows like an order fulfilment system or for procedural 
requests.
AWS recommends that for new applications customers consider AWS Step Functions 
instead of SWF.

### AMAZON MQ
Amazon MQ is a managed message broker service for ActiveMQ.
Amazon MQ supports industry-standard APIs and protocols so you can migrate messaging 
and applications without rewriting code.
Amazon MQ provides cost-efficient and flexible messaging capacity.
Amazon MQ manages the administration and maintenance of ActiveMQ brokers and 
automatically provisions infrastructure for high availability.

### AWS STEP FUNCTIONS
AWS Step Functions can be used to coordinate the components of distributed applications 
as a series of steps in a visual workflow.
You can quickly build and run state machines to execute the steps of your application in a 
reliable and scalable fashion.
How it works:
1. Define the steps of your workflow in the JSON-based Amazon States Language. The 
visual console automatically graphs each step in the order of execution.
2. Start an execution to visualize and verify the steps of your application are 
operating as intended. The console highlights the real-time status of each step and 
provides a detailed history of every execution.
3. AWS Step Functions operates and scales the steps of your application and 
underlying compute for you to help ensure your application executes reliably 
under increasing demand.
It is a managed workflow and orchestration platform.

### APPLICATION INTEGRATION SERVICES QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: An application needs to send SMS text messages to customers to notify them 
of product updates. Which service can be used?
1. AWS Step Functions
2. Amazon Simple Queue Service
3. Amazon Simple Notification Service
4. AWS Lambda

Question 2: A company needs to orchestrate several batch processes on AWS. Which 
serverless service can assist?
1. Amazon Simple Workflow Service
2. Amazon Simple Queue Service
3. Amazon EventBridge
4. AWS Step Functions

Question 3: How can a company decouple an application which uses a message-oriented 
API to communicate data between application components?
1. Create an Amazon SQS queue
2. Create an Amazon SNS topic
3. Create an AWS Step Functions state machine
4. Create an Amazon VPC route table

Question 4: How can an application be configured to send a notification to multiple 
Amazon SQS queues?
1. Use a FIFO queue
2. Use an Amazon SNS topic
3. Create an AWS Step Functions state machine





# AWS CLOUD MANAGEMENT

The AWS Cloud Management services can be used for account management, configuration 
compliance, application delivery, and systems management.

## AWS ORGANIZATIONS
AWS organizations allows you to consolidate multiple AWS accounts into an organization 
that you create and centrally manage.
Available in two feature sets:
• Consolidated Billing.
• All features.
Includes root accounts and organizational units.
Policies are applied to root accounts or OUs.
Consolidated billing includes:
• Paying Account – independent and cannot access resources of other accounts.
• Linked Accounts – all linked accounts are independent.
### AWS CONTROL TOWER
Simplifies the process of creating multi-account environments.
Sets up governance, compliance, and security guardrails for you.
Integrates with other services and features to setup the environment for you including:
• AWS Organizations, SCPs, OUs, AWS Config, AWS CloudTrail, Amazon S3, Amazon 
SNS, AWS CloudFormation, AWS Service Catalog, AWS Single Sign-On (SSO).
Examples of guardrails AWS Control Tower can configure for you include:
• Disallowing public write access to Amazon Simple Storage Service (Amazon S3) 
buckets.
• Disallowing access as a root user without multi-factor authentication.
• Enabling encryption for Amazon EBS volumes attached to Amazon EC2 instances.

## AWS Config
AWS Config is a fully managed service that provides you with an AWS resource inventory, 
configuration history, and configuration change notifications to enable security and 
regulatory compliance.
With AWS Config, you can discover existing and deleted AWS resources, determine your 
overall compliance against rules, and dive into configuration details of a resource at any 
point in time. AWS Config enables compliance auditing, security analysis, resource change 
tracking, and troubleshooting.

## AWS SERVICE CATALOG
AWS Service Catalog allows organizations to create and manage catalogs of IT services that 
are approved for use on AWS.
AWS Service Catalog allows you to centrally manage commonly deployed IT services.
IT services can include virtual machine images, servers, software, and databases and multitier application architectures.
Enables users to quickly deploy only the approved IT services they need.

## AWS SYSTEMS MANAGER
Manages many AWS resources including Amazon EC2, Amazon S3, Amazon RDS etc.
Systems Manager Components:
• Automation.
• Run Command.
• Inventory.
• Patch Manager.
• Session Manager.
• Parameter Store.

## AWS PERSONAL HEALTH DASHBOARD
AWS Personal Health Dashboard provides alerts and remediation guidance when AWS is 
experiencing events that may impact you.
Personal Health Dashboard gives you a personalized view into the performance and 
availability of the AWS services underlying your AWS resources.
The dashboard displays relevant and timely information to help you manage events in 
progress.
Also provides proactive notification to help you plan for scheduled activities.
Alerts are triggered by changes in the health of AWS resources, giving you event visibility, 
and guidance to help quickly diagnose and resolve issues.
You get a personalized view of the status of the AWS services that power your applications, 
enabling you to quickly see when AWS is experiencing issues that may impact you.
Also provides forward looking notifications, and you can set up alerts across multiple 
channels, including email and mobile notifications, so you receive timely and relevant 
information to help plan for scheduled changes that may affect you.
Alerts include remediation details and specific guidance to enable you to take immediate 
action to address AWS events impacting your resources.
Can integrate with Amazon CloudWatch Events, enabling you to build custom rules and 
select targets such as AWS Lambda functions to define automated remediation actions.
The AWS Health API allows you to integrate health data and notifications with your existing 
in-house or third-party IT Management tools.

## SERVICE HEALTH DASHBOARD
AWS publishes up-to-the-minute information on service availability.
This information is not personalized to you (unlike Personal Health Dashboard).

### AWS OPSWORKS
AWS OpsWorks is a configuration management service that provides managed instances of 
Chef and Puppet.
Updates include patching, updating, backup, configuration, and compliance management.

### AWS TRUSTED ADVISOR
AWS Trusted Advisor is an online tool that provides you real time guidance to help you 
provision your resources following AWS best practices.
Trusted Advisor checks help optimize your AWS infrastructure, improve security and 
performance, reduce your overall costs, and monitor service limits.
AWS Basic Support and AWS Developer Support customers get access to 6 security checks 
(S3 Bucket Permissions, Security Groups – Specific Ports Unrestricted, IAM Use, MFA on 
Root Account, EBS Public Snapshots, RDS Public Snapshots) and 50 service limit checks.
AWS Business Support and AWS Enterprise Support customers get access to all 115 Trusted 
Advisor checks (14 cost optimization, 17 security, 24 fault tolerance, 10 performance, and 
50 service limits) and recommendations.

### AWS CLOUDFORMATION
AWS CloudFormation provides a common language for you to describe and provision all 
the infrastructure resources in your cloud environment.
CloudFormation allows you to use a simple text file to model and provision, in an 
automated and secure manner, all the resources needed for your applications across all 
regions and accounts.
This file serves as the single source of truth for your cloud environment.
You can use JSON or YAML to describe what AWS resources you want to create and 
configure.

## AWS CLOUD MANAGEMENT QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.

Question 1: An organization is looking for a way to deploy infrastructure on AWS in 
different regions whilst ensuring consistent configuration. Which service should the 
organization use?
1. AWS Elastic Beanstalk
2. AWS Config
3. AWS CloudFormation
4. AWS Launch Configuration

Question 2: Which service uses JSON or YAML template files to deploy infrastructure as 
code?
1. AWS CloudFormation
2. AWS Elastic Beanstalk

Question 3: Which service can be used to automatically create an Amazon VPC and thenlaunch an EC2 instance, Auto Scaling Group and Elastic Load balancer?
1. AWS Elastic Beanstalk
2. AWS Management Console
3. AWS API
4. AWS CloudFormation

Question 4: AWS Trusted advisor does NOT provide advice on which of the following?
1. Cost optimization
2. Performance
3. Total Cost of Ownership (TCO)
4. Security
5. Fault Tolerance

Question 5: A company wishes to determine if there will be any AWS maintenance that 
could affect their systems over the next few days. Which service should they check?
1. AWS Service Health Dashboard
2. AWS Personal Health Dashboard
3. AWS Trusted Advisor

Question 6: A company wishes to restrict the applications users can launch to an 
approved list. Which service should they use?
1. AWS Service Catalog
2. AWS Systems Manager
3. AWS OpsWorks

Question 7: AWS Systems Manager includes management of all the following 
components, except:
1. Automation
2. Patch Manager
3. Session Manager
4. Service Catalog


