# AWS MACHINE LEARNING SERVICES

This article discusses AWS Machine Learning Services in the context of the AWS Certified 
Cloud Practitioner Exam. Services in this category come up regularly in questions and are 
usually high level.

## AWS REKOGNITION
Add image and video analysis to your applications.
Identify objects, people, text, scenes, and activities in images and videos.
Processes videos stored in an Amazon S3 bucket.
Publish completion status to Amazon SNS Topic.

## AMAZON TRANSCRIBE
Add speech to text capabilities to applications.
Recorded speech can be converted to text before it can be used in applications.
Uses a deep learning process called automatic speech recognition (ASR) to convert speech 
to text quickly and accurately.

## AMAZON TRANSLATE
Neural machine translation service that delivers fast, high-quality, and affordable language 
translation.
Uses deep learning models to deliver more accurate and more natural sounding 
translation.
Localize content such as websites and applications for your diverse users.


# AMAZON TEXTRACT
Automatically extract printed text, handwriting, and data from any document.
Features:
• Optical character recognition (OCR).
• Identifies relationships, structure, and text.
• Uses AI to extract text and structured data.
• Recognizes handwriting as well as printed text.
• Can extract from documents such as PDFs, images, forms, and tables.
• Understands context. For example, know what data to extract from a receipt or 
invoice.

# AMAZON SAGEMAKER

Helps data scientists and developers to prepare, build, train, and deploy high-quality 
machine learning (ML) models.
ML development activities including:
• Data preparation.
• Feature engineering.
• Statistical bias detection.
• Auto-ML.
• Training and tuning.
• Hosting.
• Monitoring.
• Workflows.

# AMAZON COMPREHEND

Natural-language processing (NLP) service.
Uses machine learning to uncover information in unstructured data.
Can identify critical elements in data, including references to language, people, and places, 
and the text files can be categorized by relevant topics.
In real time, you can automatically and accurately detect customer sentiment in your 
content.

# AMAZON LEX

Conversational AI for Chatbots.
Build conversational interfaces into any application using voice and text.
Build bots to increase contact center productivity, automate simple tasks, and drive 
operational efficiencies across the enterprise.

# AMAZON POLLY

Turns text into lifelike speech.
Create applications that talk and build entirely new categories of speech-enabled products.
Text-to-Speech (TTS) service uses advanced deep learning technologies to synthesize 
natural sounding human speech.

# AMAZON FORECAST

Time-series forecasting service.
Uses ML and is built for business metrics analysis

# AMAZON DEVOPS GURU

Cloud operations service for improving application operational performance and 
availability.
Detect behaviors that deviate from normal operating patterns.
Benefits:
• Automatically detect operational issues.
• Resolve issues with ML-powered insights.
• Elastically scale operational analytics.
• Uses ML to reduce alarm noise.

## AWS MACHINE LEARNING SERVICES QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: A company recorded some support call conversations in mp4 files. How can 
the company extract the audio into a text document?
1. Use Amazon Translate
2. Use Amazon Polly
3. Use Amazon Transcribe

Question 2: An application is being built that needs to identify faces in images. Which 
service can be used?
1. AWS Polly
2. AWS Lambda
3. AWS Rekognition



# ADDITIONAL AWS SERVICES
There are Additional AWS Services & Tools that may feature on the exam. Often you do not 
need to know these at a deep level but do need to understand what they are and what 
they are used for.
On this page, you’ll find some high-level details and links for more information on some of 
these services and tools.
Exam tip: Before sitting the exam, it would be wise to go through the AWS console and pick 
out any services you’re not familiar with and do a bit of reading up on them using the AWS 
documentation.
Note: If a service starts appearing regularly on the exam it may be moved to the main 
cheat sheet for the AWS service category.

# COMPUTE AMAZON ELASTIC CONTAINER SERVICE FOR KUBERNETES (EKS)

• Amazon Elastic Container Service for Kubernetes (EKS) is a 
managed Kubernetes service that makes it easy for you to run Kubernetes on AWS 
without needing to install, operate, and maintain your own Kubernetes control 
plane.
• EKS is certified Kubernetes conformant, so existing applications running on 
upstream Kubernetes are compatible with Amazon EKS.
• EKS automatically manages the availability and scalability of the Kubernetes 
control plane nodes that are responsible for starting and stopping containers, 
scheduling containers on virtual machines, storing cluster data, and other tasks.
• EKS automatically detects and replaces unhealthy control plane nodes for each 
cluster.
• Generally available but only in limited regions currently.
• https://aws.amazon.com/eks/features/

# DATABASE AMAZON NEPTUNE

• Amazon Neptune is a fast, reliable, fully managed graph database service that 
makes it easy to build and run applications that work with highly connected 
datasets.
• With Amazon Neptune, you can create sophisticated, interactive graph 
applications that can query billions of relationships in milliseconds.
• SQL queries for highly connected data are complex and hard to tune for 
performance. Instead, Amazon Neptune allows you to use the popular graph query 
languages Apache TinkerPop Gremlin and W3C’s SPARQL to execute powerful 
queries that are easy to write and perform well on connected data.
• https://aws.amazon.com/neptune/features/


# MIGRATION

## AWS MIGRATION HUB
• AWS Migration Hub provides a single location to track the progress of application 
migrations across multiple AWS and partner solutions.
• Using Migration Hub allows you to choose the AWS and partner migration tools 
that best fit your needs, while providing visibility into the status of migrations 
across your portfolio of applications.
• For example, you might use AWS Database Migration Service, AWS Server 
Migration Service, and partner migration tools such as ATADATA ATAmotion, 
CloudEndure Live Migration, or RiverMeadow Server Migration SaaS to migrate an 
application comprised of a database, virtualized web servers, and a bare metal 
server.
• Using Migration Hub, you can view the migration progress of all the resources in 
the application.
• https://aws.amazon.com/migration-hub/features/

## AWS DATABASE MIGRATION SERVICE
• AWS Database Migration Service helps you migrate databases to AWS quickly and 
securely.
• The source database remains fully operational during the migration, minimizing 
downtime to applications that rely on the database.
• The AWS Database Migration Service can migrate your data to and from most 
widely used commercial and open-source databases.
• AWS Database Migration Service supports homogenous migrations such as Oracle 
to Oracle, as well as heterogeneous migrations between different database 
platforms, such as Oracle or Microsoft SQL Server to Amazon Aurora.
• With AWS Database Migration Service, you can continuously replicate your data 
with high availability and consolidate databases into a petabyte-scale data 
warehouse by streaming data to Amazon Redshift and Amazon S3.
• https://aws.amazon.com/dms/

## AWS SERVER MIGRATION SERVICE
• AWS Server Migration Service (SMS) is an agentless service which makes it easier 
and faster for you to migrate thousands of on-premises workloads to AWS
• AWS SMS allows you to automate, schedule, and track incremental replications of 
live server volumes, making it easier for you to coordinate large-scale server 
migrations
• https://aws.amazon.com/server-migration-service

# NETWORKING & CONTENT DELIVERY

## AMAZON API GATEWAY
• Amazon API Gateway is a fully managed service that makes it easy for developers 
to create, publish, maintain, monitor, and secure APIs at any scale.
• With a few clicks in the AWS Management Console, you can create an API that acts 
as a “front door” for applications to access data, business logic, or functionality 
from your back-end services.
• Back-end services may include Amazon Elastic Compute Cloud (Amazon EC2), code 
running on AWS Lambda, or any web application.
• https://aws.amazon.com/api-gateway/features/

# DEVELOPER TOOLS 
## AWS CODESTAR
• AWS CodeStar enables you to quickly develop, build, and deploy applications on 
AWS. AWS CodeStar provides a unified user interface, enabling you to easily 
manage your software development activities in one place.
• With AWS CodeStar, you can set up your entire continuous delivery toolchain in 
minutes, allowing you to start releasing code faster. AWS CodeStar makes it easy 
for your whole team to work together securely, allowing you to easily manage 
access and add owners, contributors, and viewers to your projects.
• With AWS CodeStar, you can use a variety of project templates to start developing 
applications on Amazon EC2, AWS Lambda, and AWS Elastic Beanstalk.
• AWS CodeStar projects support many popular programming languages including 
Java, JavaScript, PHP, Ruby, and Python.
• https://aws.amazon.com/codestar/features/
## AWS CODECOMMIT
• AWS CodeCommit is a fully managed source control service that hosts secure Gitbased repositories.
• It makes it easy for teams to collaborate on code in a secure and highly scalable 
ecosystem.
• CodeCommit eliminates the need to operate your own source control system or 
worry about scaling its infrastructure.
• You can use CodeCommit to securely store anything from source code to binaries, 
and it works seamlessly with your existing Git tools.
• https://aws.amazon.com/codecommit/features/

## AWS CODEBUILD
• AWS CodeBuild is a fully managed continuous integration service that compiles 
source code, runs tests, and produces software packages that are ready to deploy.
• With CodeBuild, you don’t need to provision, manage, and scale your own build 
servers. CodeBuild scales continuously and processes multiple builds concurrently, so your builds are not left waiting in a queue.
• You can get started quickly by using prepackaged build environments, or you can 
create custom build environments that use your own build tools.
• With CodeBuild, you are charged by the minute for the compute resources you 
use.
• https://aws.amazon.com/codebuild/features/

## AWS CODEDEPLOY
• AWS CodeDeploy is a fully managed deployment service that automates software 
deployments to a variety of computer services such as Amazon EC2, AWS Lambda, 
and your on-premises servers.
• AWS CodeDeploy makes it easier for you to rapidly release new features, helps you 
avoid downtime during application deployment, and handles the complexity of 
updating your applications.
• You can use AWS CodeDeploy to automate software deployments, eliminating the 
need for error-prone manual operations. The service scales to match your 
deployment needs, from a single Lambda function to thousands of EC2 instances.
• https://aws.amazon.com/codedeploy/features/

## AWS CODEPIPELINE
• AWS CodePipeline is a fully managed continuous delivery service that helps you 
automate your release pipelines for fast and reliable application and infrastructure 
updates.
• CodePipeline automates the build, test, and deploy phases of your release process 
every time there is a code change, based on the release model you define.
• This enables you to deliver features and updates rapidly and reliably.
• You can easily integrate AWS CodePipeline with third-party services such as GitHub 
or with your own custom plugin.
• https://aws.amazon.com/codepipeline/features/

## AWS X-RAY
• AWS X-Ray helps developers analyze and debug production, distributed 
applications, such as those built using a microservices architecture.
• With X-Ray, you can understand how your application and its underlying services 
are performing to identify and troubleshoot the root cause of performance issues 
and errors.
• X-Ray provides an end-to-end view of requests as they travel through your 
application and shows a map of your application’s underlying components.
• You can use X-Ray to analyze both applications in development and in production, 
from simple three-tier applications to complex microservices applications 
consisting of thousands of services.
• https://aws.amazon.com/xray/features/
• https://aws.amazon.com/servicecatalog/features/

# AWS MANAGED SERVICES
• AWS Managed Services provides ongoing management of your AWS infrastructure 
so you can focus on your applications.
• By implementing best practices to maintain your infrastructure, AWS Managed 
Services helps to reduce your operational overhead and risk.
• AWS Managed Services automates common activities such as change requests, 
monitoring, patch management, security, and backup services, and provides fulllifecycle services to provision, run, and support your infrastructure.
• AWS Managed Services delivers consistent operations management and 
predictable results by following ITIL® best practices, and provides tooling and 
automation to increase efficiency, and reduce your operational overhead and risk.
• https://aws.amazon.com/managed-services/#

# ANALYTICS

## AMAZON ATHENA
• Amazon Athena is an interactive query service that makes it easy to analyze data in 
Amazon S3 using standard SQL.
• Athena is serverless, so there is no infrastructure to manage, and you pay only for 
the queries that you run.
• With a few clicks in the AWS Management Console, customers can point Athena at 
their data stored in S3 and begin using standard SQL to run ad-hoc queries and get 
results in seconds.
• You can use Athena to process logs, perform ad-hoc analysis, and run interactive 
queries
• Athena scales automatically – executing queries in parallel – so results are fast, 
even with large datasets and complex queries.
• https://aws.amazon.com/athena/features/

## AMAZON EMR
• Amazon Elastic Map Reduce (EMR) provides a managed Hadoop framework that 
makes it easy, fast, and cost-effective to process vast amounts of data across 
dynamically scalable Amazon EC2 instances.
• You can also run other popular distributed frameworks such as Apache 
Spark, HBase, Presto, and Flink in Amazon EMR, and interact with data in other 
AWS data stores such as Amazon S3 and Amazon DynamoDB.
• Amazon EMR securely and reliably handles a broad set of big data use cases, 
including log analysis, web indexing, data transformations (ETL), machine learning, 
financial analysis, scientific simulation, and bioinformatic.
• https://aws.amazon.com/emr/features/

## AMAZON CLOUDSEARCH
• Amazon CloudSearch is a managed service in the AWS Cloud that makes it simple 
and cost-effective to set up, manage, and scale a search solution for your website 
or application.
• Amazon CloudSearch supports 34 languages and popular search features such as 
highlighting, autocomplete, and geospatial search.
• https://aws.amazon.com/cloudsearch/

## AMAZON ELASTICSEARCH
• Amazon Elasticsearch Service is a fully managed service that makes it easy for you 
to deploy, secure, operate, and scale Elasticsearch to search, analyze, and visualize 
data in real-time.
• With Amazon Elasticsearch Service you get easy-to-use APIs and real-time analytics 
capabilities to power use-cases such as log analytics, full-text search, application 
monitoring, and clickstream analytics, with enterprise-grade availability, scalability, 
and security.
• https://aws.amazon.com/elasticsearch-service/features/

## AMAZON KINESIS
• Amazon Kinesis makes it easy to collect, process, and analyze real-time, streaming 
data so you can get timely insights and react quickly to new information.
• There are four types of Kinesis service:
o Kinesis Video Streams makes it easy to securely stream video from connected 
devices to AWS for analytics, machine learning (ML), and other processing.
o Kinesis Data Streams enables you to build custom applications that process or 
analyze streaming data for specialized needs.
o Kinesis Data Firehose is the easiest way to load streaming data into data stores 
and analytics tools.
o Amazon Kinesis Data Analytics is the easiest way to process and analyze realtime, streaming data.
• https://aws.amazon.com/kinesis/
• https://digitalcloud.training/certification-training/aws-solutions-architectassociate/analytics/amazon-kinesis/

## AWS DATA PIPELINE
• AWS Data Pipeline is a web service that helps you reliably process and move data 
between different AWS compute and storage services, as well as on-premises data 
sources, at specified intervals.
• With AWS Data Pipeline, you can regularly access your data where it’s stored, 
transform, and process it at scale, and efficiently transfer the results to AWS 
services such as Amazon S3, Amazon RDS, Amazon DynamoDB, and Amazon EMR.
• AWS Data Pipeline helps you easily create complex data processing workloads that 
are fault tolerant, repeatable, and highly available.
• https://aws.amazon.com/datapipeline/

## AWS GLUE
• AWS Glue is a fully managed extract, transform, and load (ETL) service that makes it easy for customers to prepare and load their data for analytics.
• You can create and run an ETL job with a few clicks in the AWS Management 
Console.
• You simply point AWS Glue to your data stored on AWS, and AWS Glue discovers 
your data and stores the associated metadata (e.g. table definition and schema) in 
the AWS Glue Data Catalog.
• Once cataloged, your data is immediately searchable, queryable, and available for 
ETL.
• AWS Glue generates the code to execute your data transformations and data 
loading processes.
• https://aws.amazon.com/glue/features/


# MEDIA SERVICES

## AMAZON ELASTIC TRANSCODER
• Amazon Elastic Transcoder is media transcoding in the cloud.
• It is designed to be a highly scalable, easy to use and a cost-effective way for 
developers and businesses to convert (or “transcode”) media files from their 
source format into versions that will playback on devices like smartphones, tablets, 
and PCs.
• https://aws.amazon.com/elastictranscoder/

# MOBILE SERVICES
## AWS APPSYNC
• AWS AppSync makes it easy to build data-driven mobile and browser-based apps 
that deliver responsive, collaborative experiences by keeping the data updated 
when devices are connected, enabling the app to use local data when offline, and 
synchronizing the data when the devices reconnect.
• AWS AppSync uses the open standard GraphQL query language so you can request, 
change, and subscribe to the exact data you need with just a few lines of code.
• https://aws.amazon.com/appsync/product-details/

## AWS DEVICE FARM
• AWS Device Farm is an app testing service that lets you test and interact with your 
Android, iOS, and web apps on many devices at once, or reproduce issues on a 
device in real time.
• View video, screenshots, logs, and performance data to pinpoint and fix issues and 
increase quality before shipping your app.
• https://aws.amazon.com/device-farm/


# END USER COMPUTING

## AMAZON WORKSPACES
• Amazon WorkSpaces is a managed, secure cloud desktop service. You can use 
Amazon WorkSpaces to provision either Windows or Linux desktops in just a few 
minutes and quickly scale to provide thousands of desktops to workers across the 
globe.
• Amazon WorkSpaces offers you an easy way to provide a secure, managed, cloudbased virtual desktop experience to your end-users.
• Unlike traditional on-premises Virtual Desktop Infrastructure (VDI) solutions, you 
don’t have to worry about procuring, deploying, and managing a complex 
environment – Amazon WorkSpaces takes care of the heavy lifting and provides a 
fully managed service.
• https://aws.amazon.com/workspaces/features/

## AWS APPSTREAM
• Fully managed non-persistent application streaming service.
• Alternative to popular products such as Citrix XenApp.
• https://aws.amazon.com/appstream2/features/

## AWS WORKLINK
• Provides secure, one-click access to your internal websites and web apps using 
mobile phone browsers.
• Does not require VPN client or App.
• https://aws.amazon.com/worklink/features/

## AWS WORKDOCS
• Fully managed, secure content creation, storage, and collaboration service
• Create, edit, and share content that’s centrally stored on AWS.
• https://aws.amazon.com/workdocs/features/


# INTERNET OF THINGS (IOT)

## AWS IOT CORE
• Describes the network of physical objects that are embedded with sensors or 
software.
• Each IoT device can communicate and exchange data with other devices and 
systems.
• Use cases include:
o Smart home automation.
o Smart healthcare.
o Manufacturing.
o Agriculture.


• Allows you to connect IoT devices to the AWS cloud without the need to provision 
or manage servers.
• Can support billions of devices and trillions of messages.
• https://aws.amazon.com/iot-core/features/

## ADDITIONAL AWS SERVICES QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: A company moves data between Amazon S3, RDS and EMR. Which service 
can help to process and move data between services?
1. Amazon Athena
2. Amazon QuickSight
3. AWS Data Pipeline

Question 2: Which service can be used to migrate an on-premises database to Amazon 
RDS?
1. AWS Server Migration Service 
2. AWS Transfer for SMTP
3. Application Discovery Service
4. Database Migration Service

Question 3: Which service can be used to migrate exabytes of data into the AWS Cloud?
1. AWS Snowmobile
2. AWS Snowball

Question 4: Which service can be used to migrate 50TB of data quickly and affordably to 
Amazon S3 for a company with a slow Internet connection?
1. Amazon S3 Transfer Acceleration
2. Amazon S3 multi-part upload
3. AWS Snowball
4. AWS Snowmobile

Question 5: How can a company migrate a database from Amazon EC2 to RDS without 
downtime?
1. Create an RDS read replica and then promote replica to master
2. Create a new database from an EBS snapshot
3. Migrate using the AWS Database Migration Service (DMS)

Question 6: A company needs to migrate several TB of data from an on-premises 
NAS device to Amazon FSx. Which service can the company use to migrate the data over 
a VPN connection?
1. AWS Database Migration Service (DMS)
2. AWS Snowball Edge
3. AWS DataSync
4. Amazon S3 Transfer Acceleration








