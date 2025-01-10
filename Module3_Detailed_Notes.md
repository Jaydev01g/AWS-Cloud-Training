# AWS COMPUTE
This article discusses AWS Compute in the context of the AWS Certified Cloud Practitioner Exam. This is one of the key technology areas covered in the exam guide.
## AMAZON EC2
Amazon Elastic Compute Cloud (Amazon EC2) is a web service with which you can run virtual server “instances” in the cloud.
Amazon EC2 instances can run the Windows, Linux, or MacOS operating systems.The EC2 simple web service interface allows you to obtain and configure capacity with 
minimal friction. EC2 is designed to make web-scale cloud computing easier for developers. Amazon EC2 changes the economics of computing by allowing you to pay only for capacity 
that you use. Amazon EC2 provides developers the tools to build failure resilient applications and isolate them from common failure scenarios.

#### Benefits of EC2 include:
• Elastic Web-Scale computing – you can increase or decrease capacity within minutes not hours and commission one to thousands of instances simultaneously.
• Completely controlled – You have complete control include root access to each instance and can stop and start instances without losing data and using web 
service APIs.
• Flexible Cloud Hosting Services – you can choose from multiple instance types, operating systems, and software packages as well as instances with varying 
memory, CPU, and storage configurations.
• Integrated – EC2 is integrated with most AWS services such as S3, RDS, and VPC to provide a complete, secure solution.
• Reliable – EC2 offers a highly reliable environment where replacement instances can be rapidly and predictably commissioned with SLAs of 99.99% for each region.
• Secure – EC2 works in conjunction with VPC to provide a secure location with an IP address range you specify and offers Security Groups, Network ACLs, and IPSec 
VPN features.
• Inexpensive – Amazon passes on the financial benefits of scale by charging very low rates and on a capacity consumed basis.

An Amazon Machine Image (AMI) is a special type of virtual appliance that is used to create a virtual machine within the Amazon Elastic Compute Cloud (“EC2”).
An AMI includes the following:
• One or more EBS snapshots, or, for instance-store-backed AMIs, a template for the 
root volume of the instance (for example, an operating system, an application 
server, and applications).

• Launch permissions that control which AWS accounts can use the AMI to launchinstances.

• A block device mapping that specifies the volumes to attach to the instance when 
it’s launched.

AMIs come in three main categories:
• Community AMIs – free to use, generally you just select the operating system you 
want.

• AWS Marketplace AMIs – pay to use, generally come packaged with additional, 
licensed software.

• My AMIs – AMIs that you create yourself.

Metadata and User Data:
• User data is data that is supplied by the user at instance launch in the form of a script.
• Instance metadata is data about your instance that you can use to configure or manage the running instance.
• User data is limited to 16KB.
• User data and metadata are not encrypted.
• Instance metadata is available at http://169.254.169.254/latest/meta-data.

The Instance Metadata Query tool allows you to query the instance metadata without having to type out the full URI or category names.

### PRICING
#### On-demand:
• Good for users that want the low cost and flexibility of EC2 without any up-front payment or long-term commitment.
• Applications with short term, spiky, or unpredictable workloads that cannot beinterrupted.
• Applications being developed or tested on EC2 for the first time.

#### Reserved:
• Applications with steady state or predictable usage.
• Applications that require reserved capacity.
• Users can make up-front payments to reduce their total computing costs even 
further.
• Standard Reserved Instances (RIs) provide up to 75% off on-demand price.
• Convertible RIs provide up to 54% off on-demand price – provides the capability to 
change the attributes of the RI if the exchange results in the creation of RIs of 
equal or greater value.
• Scheduled RIs are available to launch within the time window you reserve. This 
option allows you to match your capacity reservation to a predictable recurring 
schedule that only requires a fraction of a day, a week, or a month.

#### Spot:
• Applications that have flexible start and end times.
• Applications that are only feasible at very low compute prices.
• Users with an urgent need for a large amount of additional compute capacity.
• If Amazon terminate your instances, you do not pay, if you terminate you pay for 
the hour.

#### Dedicated hosts:
• Physical servers dedicated just for your use.
• You then have control over which instances are deployed on that host.
• Available as On-Demand or with Dedicated Host Reservation.
• Useful if you have server-bound software licenses that use metrics like per-core, 
per-socket, or per-VM.
• Each dedicated host can only run one EC2 instance size and type.
• Good for regulatory compliance or licensing requirements.
• Predictable performance.
• Complete isolation.
• Most expensive option.
• Billing is per host.

#### Dedicated instances:
• Virtualized instances on hardware just for you.
• Also uses physically dedicated EC2 servers.
• Does not provide the additional visibility and controls of dedicated hosts (e.g. how 
instances are placed on a server).
• Billing is per instance.
• May share hardware with other non-dedicated instances in the same account.
• Available as On-Demand, Reserved Instances, and Spot Instances.
• Cost additional $2 per hour per region.
• Savings Plans is a flexible pricing model that provides savings of up to 72% on your AWS compute usage.
• This pricing model offers lower prices on Amazon EC2 instances usage, regardless of instance family, size, OS, tenancy, or AWS Region.
• Also applies to AWS Fargate and AWS Lambda usage.

#### INSTANCE TYPES
Amazon EC2 provides a wide selection of instance types optimized to fit different use cases.Instance types comprise varying combinations of CPU, memory, storage, and networking capacity and give you the flexibility to choose the appropriate mix of resources for your applications.Each instance type includes one or more instance sizes, allowing you to scale your resources to the requirements of your target workload.
The table below helps you to understand some of the various EC2 instance families and their intended use case:
![image](https://github.com/user-attachments/assets/f31d17b5-e14c-4d07-8483-3dc849905edb)


# AMAZON ELASTIC CONTAINER SERVICE (ECS)

Amazon Elastic Container Service (ECS) is another product in the AWS Compute category. It provides a highly scalable, high performance container management service that supports Docker containers and allows you to easily run applications on a managed cluster of Amazon EC2 instances.Amazon ECS eliminates the need for you to install, operate, and scale your own cluster management infrastructure. Using API calls you can launch and stop container-enabled applications, query the 
complete state of clusters, and access many familiar features like security groups, Elastic Load Balancing, EBS volumes and IAM roles.Amazon ECS can be used to schedule the placement of containers across clusters based on resource needs and availability requirements. An Amazon ECS launch type determines the type of infrastructure on which your tasks and services are hosted.

There are two launch types, and the table below describes some of the differences between the two launch types:

![image](https://github.com/user-attachments/assets/533d16be-4b03-4da2-8db3-e1d0a612c407)


## AWS LAMBDA
AWS Lambda is a serverless computing technology that allows you to run code without provisioning or managing servers.AWS Lambda executes code only when needed and scales automatically.You pay only for the compute time you consume (you pay nothing when your code is not running).
#### Benefits of AWS Lambda:
• No servers to manage.
• Continuous scaling.
• Millisecond billing.
• Integrates with almost all other AWS services.

##### Primary use cases for AWS Lambda:
• Data processing.
• Real-time file processing.
• Real-time stream processing.
• Build serverless backends for web, mobile, IOT, and 3rd party API requests.

## AMAZON LIGHTSAIL
##### Amazon LightSail Instances
Amazon LightSail is one of the newest services in the AWS Compute suite of products. Amazon LightSail is great for users who do not have deep AWS technical expertise as it 
makes it very easy to provision compute services. Amazon LightSail provides developers compute, storage, and networking capacity and capabilities to deploy and manage websites, web applications, and databases in the cloud. Amazon LightSail includes everything you need to launch your project quickly – a virtual machine, SSD-based storage, data transfer, DNS management, and a static IP .Amazon LightSail provides preconfigured virtual private servers (instances) that include everything required to deploy and application or create a database. The underlying infrastructure and operating system are managed by Amazon LightSail.

Best suited to projects that require a few dozen instances or fewer.

Provides a simple management interface.

Good for blogs, websites, web applications, e-commerce etc.

Can deploy load balancers and attach block storage.

Public API.

databases, and 5 load balancers per account.

Up to 20 certificates per calendar year.

Can connect to each other and other AWS resources through public Internet and private (VPC peering) networking.

Application templates include WordPress, WordPress Multisite, Drupal, Joomla!, Magento, Redmine, LAMP, Nginx (LEMP), MEAN, Node.js, and more.

Amazon LightSail currently supports 6 Linux or Unix-like distributions: Amazon Linux, CentOS, Debian, FreeBSD, OpenSUSE, and Ubuntu, as well as 2 Windows Server versions: 
2012 R2 and 2016.

### AMAZON LIGHTSAIL DATABASES
Amazon LightSail databases are instances that are dedicated to running databases.
An Amazon LightSail database can contain multiple user-created databases, and you can 
access it by using the same tools and applications that you use with a stand-alone 
database.
Amazon LightSail managed databases provide an easy, low maintenance way to store your 
data in the cloud.
Amazon LightSail manages a range of maintenance activities and security for your database 
and its underlying infrastructure.
Amazon LightSail automatically backs up your database and allows point in time restore 
from the past 7 days using the database restore tool.
Amazon LightSail databases support the latest major versions of MySQL. Currently, these 
versions are 5.6, 5.7, and 8.0 for MySQL.
Amazon LightSail databases are available in Standard and High Availability plans.
High Availability plans add redundancy and durability to your database, by automatically 
creating standby database in a separate Availability Zone.
Amazon LightSail is very affordable.
Amazon LightSail plans are billed on an on-demand hourly rate, so you pay only for what 
you use.
For every Amazon LightSail plan you use, we charge you the fixed hourly price, up to the 
maximum monthly plan cost.

### AWS ELASTIC BEANSTALK
AWS Elastic Beanstalk is the fastest and simplest way to get web applications up and 
running on AWS.
Developers simply upload their application code, and the service automatically handles all 
the details such as resource provisioning, load balancing, auto-scaling, and monitoring.
Elastic Beanstalk is ideal if you have a PHP, Java, Python, Ruby, Node.js, .NET, Go, or Docker 
web application.
Elastic Beanstalk uses core AWS services such as Amazon EC2, Amazon Elastic Container 
Service (Amazon ECS), Auto Scaling, and Elastic Load Balancing to easily support 
applications that need to scale to serve millions of users.

### AWS BATCH
AWS Batch enables developers, scientists, and engineers to run hundreds of thousands of 
batch computing jobs easily and efficiently on AWS.
AWS Batch dynamically provisions the optimal quantity and type of compute resources 
(e.g., CPU or memory optimized instances) based on the volume and specific resource 
requirements of the batch jobs submitted.
With AWS Batch, you simply package the code for your batch jobs, specify their 
dependencies, and submit your batch job using the AWS Management Console, CLIs, or 
SDKs.
AWS Batch allows you to specify execution parameters and job dependencies and
facilitates integration with a broad range of popular batch computing workflow engines 
and languages (e.g., Pegasus WMS, Luigi, and AWS Step Functions).
AWS Batch efficiently and dynamically provisions and scales Amazon 
EC2 and Spot Instances based on the requirements of your jobs. AWS Batch provides 
default job queues and compute environment definitions that enable you to get started 
quickly.

#### AWS COMPUTE QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question: Question 1: Which of the following is NOT a benefit of AWS Lambda?
1. No servers to manage
2. Pay only when your code is running
3. Continuous scaling
4. Multiple instance types to choose from

Question 2: Which service can assist a developer with quickly deploying and managing a 
web application on AWS?
1. AWS CloudFormation
2. AWS Elastic Beanstalk
   
Question 3: AWS Elastic Beanstalk is an example of which cloud computing service 
model?
1. On-premises
2. Infrastructure as a Service (IaaS)
3. Platform as a Service (PaaS)
4. Software as a Service (SaaS)
   
Question 4: What is a benefit of Amazon EC2 compared to traditional servers?
1. You can use specialized hardware
2. You have more control over the operating system
3. You can scale elastically within minutes
4. You get more compute power in the cloud
   
Question 5: How can you run commands on an Amazon EC2 instance at launch time?
1. With metadata
2. With user data
3. With a container
4. With a snapshot
   
Question 6: Which service allows you to run Docker containers on AWS?
1. Amazon EC2
2. AWS Lambda
3. Amazon ECS
4. Amazon EBS
   
Question 7: Which service is good for running compute workloads for people who don't 
have technical expertise with AWS?
1. Amazon ECS
2. Amazon EC2
3. Amazon LightSail
4. AWS Lambda
   
### AWS COMPUTE ANSWERS

Question: Question 1: Which of the following is NOT a benefit of AWS Lambda?
1. No servers to manage
2. Pay only when your code is running
3. Continuous scaling
4. Multiple instance types to choose from
Answer: 4

Explanation:
1 is incorrect. This is a benefit of AWS Lambda - there are no servers to manage which 
is why it is known as a "serverless" service
2 is incorrect. You do only pay when your code is running, and this is a great benefit of AWS Lambda
3 is incorrect. AWS Lambda includes continuous scaling which means it elastically adjusts to demand
4 is correct. As AWS Lambda is a serverless service, there are no instance types to choose from

Question 2: Which service can assist a developer with quickly deploying and managing a 
web application on AWS?
1. AWS CloudFormation
2. AWS Elastic Beanstalk
Answer: 2
Explanation:
1 is incorrect. Think of CloudFormation as deploying infrastructure as code, whilst 
Elastic Beanstalk is more focused on deploying applications on EC2 (PaaS)
2 is correct. AWS Elastic Beanstalk can be used to quickly deploy and manage 
applications in the AWS Cloud

Question 3: AWS Elastic Beanstalk is an example of which cloud computing service 
model?
1. On-premises
2. Infrastructure as a Service (IaaS)
3. Platform as a Service (PaaS)
4. Software as a Service (SaaS)
Answer: 3
Explanation:
1 is incorrect. Elastic Beanstalk cannot be used on-premises
2 is incorrect. An example of IaaS is Amazon EC2
3 is correct. Elastic Beanstalk is considered to be a PaaS service. This means the 
underlying infrastructure and the runtime engine are managed for you and you only 
need to upload the code
4 is incorrect. Examples of SaaS are Salesforce, Facebook and Gmail

Question 4: What is a benefit of Amazon EC2 compared to traditional servers?
1. You can use specialized hardware
2. You have more control over the operating system
3. You can scale elastically within minutes
4. You get more compute power in the cloud
Answer: 3
Explanation:
1 is incorrect. You cannot use specialized hardware in the cloud. You launch instances 
on the AWS platform and have no control over the hardware they use
2 is incorrect. You don't have any more control over the operating system in the cloud 
as in both on-premise and the cloud you have full control
3 is correct. This is a key benefit of the AWS Cloud. You can elastically increase or 
decrease capacity by changing instance types whenever you need to
4 is incorrect. This is not necessarily true. You can build very powerful compute 
platforms in your own data center (however it would be very expensive)

Question 5: How can you run commands on an Amazon EC2 instance at launch time?
1. With metadata
2. With user data
3. With a container
4. With a snapshot
Answer: 2
Explanation:
1 is incorrect. Metadata is information about the instance. You can use metadata for 
finding information such as the availability zone an instance is in or its IP address
2 is correct. User data can be run at instance launch time. You can use it to run 
commands
3 is incorrect. Containers are another type of compute type; you cannot use a 
container to run commands on an EC2 instance at launch time
4 is incorrect. Snapshots are copies of EBS volumes that can be used as a backup

Question 6: Which service allows you to run Docker containers on AWS?
1. Amazon EC2
2. AWS Lambda
3. Amazon ECS
4. Amazon EBS
Answer: 3
Explanation:
1 is incorrect. Amazon EC2 is not the service that enables you to use Docker. However, 
with the EC2 launch type it is used to run the container platform
2 is incorrect. AWS Lambda is used to run functions, not Docker containers
3 is correct. Amazon Elastic Container Service (ECS) is used to run Docker containers on AWS
4 is incorrect. Amazon Elastic Block Store (EBS) is a storage solution that creates 
"virtual hard drives in the cloud"

Question 7: Which service is good for running compute workloads for people who don't 
have technical expertise with AWS?
1. Amazon ECS
2. Amazon EC2
3. Amazon LightSail
4. AWS Lambda
Answer: 3
Explanation:
1 is incorrect. Managing Amazon ECS requires good technical knowledge of AWS
2 is incorrect. Managing Amazon EC2 requires good technical knowledge of AWS
3 is correct. Amazon LightSail is great for users who do not have deep AWS technical 
expertise as it makes it very easy to provision compute services
4 is incorrect. Managing AWS Lambda requires good technical knowledge of AWS






## AWS STORAGE
This article discusses AWS Compute in the context of the AWS Certified Cloud Practitioner 
Exam. This is one of the key technology areas covered in the exam guide.
### AMAZON SIMPLE STORAGE SERVICE (S3)
Amazon S3 is object storage built to store and retrieve any amount of data from anywhere 
– web sites and mobile apps, corporate applications, and data from IoT sensors or devices.
You can store any type of file in S3.
S3 is designed to deliver 99.999999999% durability, and stores data for millions of 
applications used by market leaders in every industry.
S3 provides comprehensive security and compliance capabilities that meet even the most 
stringent regulatory requirements.
S3 gives customers flexibility in the way they manage data for cost optimization, access 
control, and compliance.
Typical use cases include:
• Backup and Storage – Provide data backup and storage services for others.
• Application Hosting – Provide services that deploy, install, and manage web 
applications.
• Media Hosting – Build a redundant, scalable, and highly available infrastructure 
that hosts video, photo, or music uploads and downloads.
• Software Delivery – Host your software applications that customers can download.
• Static Website – you can configure a static website to run from an S3 bucket.
S3 provides query-in-place functionality, allowing you to run powerful analytics directly on 
your data at rest in S3. And Amazon S3 is the most supported cloud storage service 
available, with integration from the largest community of third-party solutions, systems 
integrator partners, and other AWS services.
Files can be anywhere from 0 bytes to 5 TB.
There is unlimited storage available.
Files are stored in buckets.
Buckets are root level folders.
Any subfolder within a bucket is known as a “folder”.
S3 is a universal namespace so bucket names must be unique globally.
There are seven S3 storage classes.
• S3 Standard (durable, immediately available, frequently accessed).
• S3 Intelligent-Tiering (automatically moves data to the most cost-effective tier).
• S3 Standard-IA (durable, immediately available, infrequently accessed).
• S3 One Zone-IA (lower cost for infrequently accessed data with less resilience).
• S3 Glacier Instant Retrieval (data that is rarely accessed and requires retrieval in 
milliseconds).
• S3 Glacier Flexible Retrieval (archived data, retrieval times in minutes or hours).
• S3 Glacier Deep Archive (lowest cost storage class for long term retention).
The table below provides the details of each Amazon S3 storage class:
![image](https://github.com/user-attachments/assets/c9c76861-99b7-4847-bb15-c8cdd67565be)
When you successfully upload a file to S3 you receive a HTTP 200 code.
S3 is a persistent, highly durable data store.
Persistent data stores are non-volatile storage systems that retain data when powered off.
This contrasts with transient data stores and ephemeral data stores which lose the data 
when powered off.
The following table provides a description of persistent, transient, and ephemeral data 
stores and which AWS service to use:
![image](https://github.com/user-attachments/assets/88b1b379-0bee-4d61-920b-b2c94a169e2c)
![image](https://github.com/user-attachments/assets/ecd5503a-37d8-4ba7-ab91-1ca46d176695)
Bucket names must follow a set of rules:
• Names must be unique across all of AWS.
• Names must be 3 to 63 characters in length.
• Names can only contain lowercase letters, numbers, and hyphens.
• Names cannot be formatted as an IP address.
Objects consist of:
• Key (name of the object).
• Value (data made up of a sequence of bytes).
• Version ID (used for versioning).
• Metadata (data about the data that is stored).
Subresources:
• Access control lists.
• Torrent.
Object sharing – the ability to make any object publicly available via a URL.
Lifecycle management – set rules to transfer objects between storage classes at defined 
time intervals.
Versioning – automatically keep multiple versions of an object (when enabled).
Encryption can be enabled for bucket.
Data is secured using ACLs and bucket policies.
Charges:
• Storage.
• Requests.
• Storage management pricing.
• Data transfer pricing.
• Transfer acceleration.
When you create a bucket, you need to select the region where it will be created.
It is a best practice to create buckets in regions that are physically closest to your users to 
reduce latency.
Additional capabilities offered by Amazon S3 include:![image](https://github.com/user-attachments/assets/5cafdcb1-0fd8-4c38-91da-194b4fe3d3d6)![image](https://github.com/user-attachments/assets/38f565bf-2b80-469a-b995-4ef76d500b29)

### AWS SNOWBALL
With AWS Snowball (Snowball), you can transfer hundreds of terabytes or petabytes of 
data between your on-premises data centers and Amazon Simple Storage Service (Amazon 
S3).
Uses a secure storage device for physical transportation.
AWS Snowball Client is software that is installed on a local computer and is used to 
identify, compress, encrypt, and transfer data.
Uses 256-bit encryption (managed with the AWS KMS) and tamper-resistant enclosures 
with TPM.
The table below describes the AWS Snow offerings at a high-level:![image](https://github.com/user-attachments/assets/d7941fe3-5f03-48d9-aaba-06ed42d88452)
Snowball can import to S3 or export from S3.
Import/export is when you send your own disks into AWS – this is being deprecated in 
favor of Snowball.
Snowball must be ordered from and returned to the same region.
To speed up data transfer it is recommended to run simultaneous instances of the AWS 
Snowball Client in multiple terminals and transfer small files as batches.

### AMAZON ELASTIC BLOCK STORE (EBS)
Amazon Elastic Block Store (Amazon EBS) provides persistent block storage volumes for 
use with Amazon EC2 instances in the AWS Cloud.
Each Amazon EBS volume is automatically replicated within its Availability Zone to protect 
you from component failure, offering high availability and durability.
Amazon EBS volumes offer the consistent and low-latency performance needed to run your workloads. With Amazon EBS, you can scale your usage up or down within minutes –
all while paying a low price for only what you provision.
The following EBS volumes appear most often on the AWS exams:![image](https://github.com/user-attachments/assets/739cff8a-2b25-4bc6-b32f-c584eba43cf6)
EBS volume data persists independently of the life of the instance.
EBS volumes do not need to be attached to an instance.
You can attach multiple EBS volumes to an instance.
You cannot attach an EBS volume to multiple instances (use Elastic File Store instead).
EBS volumes must be in the same AZ as the instances they are attached to.
Termination protection is turned off by default and must be manually enabled (keeps the 
volume/data when the instance is terminated).
Root EBS volumes are deleted on termination by default.
Extra non-boot volumes are not deleted on termination by default.
The behavior can be changed by altering the “DeleteOnTermination” attribute.
EBS Snapshots:
• Snapshots capture a point-in-time state of an instance.
• Snapshots are stored on S3.
• Does not provide granular backup (not a replacement for backup software).
• If you make periodic snapshots of a volume, the snapshots are incremental, which 
means that only the blocks on the device that have changed after your last 
snapshot are saved in the new snapshot.
• Even though snapshots are saved incrementally, the snapshot deletion process is 
designed so that you need to retain only the most recent snapshot to restore the 
volume.
• Snapshots can only be accessed through the EC2 APIs.
• EBS volumes are AZ specific, but snapshots are region specific.

## INSTANCE STORE VOLUMES
Instance store volumes are high performance local disks that are physically attached to the 
host computer on which an EC2 instance runs.
Instance stores are ephemeral which means the data is lost when powered off (nonpersistent).
Instances stores are ideal for temporary storage of information that changes frequently, 
such as buffers, caches, or scratch data.
Instance store volume root devices are created from AMI templates stored on S3.
Instance store volumes cannot be detached/reattached.

## AMAZON ELASTIC FILE SYSTEM (EFS)
EFS is a fully managed service that makes it easy to set up and scale file storage in the 
Amazon Cloud.
Good for big data and analytics, media processing workflows, content management, web 
serving, home directories etc.
EFS uses the NFS protocol.
Pay for what you use (no pre-provisioning required).
Can scale up to petabytes.
EFS is elastic and grows and shrinks as you add and remove data.
Can concurrently connect 1 to 1000s of EC2 instances, from multiple AZs.
A file system can be accessed concurrently from all AZs in the region where it is located.
By default, you can create up to 10 file systems per account.
On-premises access can be enabled via Direct Connect or AWS VPN.
Can choose General Purpose or Max I/O (both SSD).
The VPC of the connecting instance must have DNS hostnames enabled.
EFS provides a file system interface, file system access semantics (such as strong 
consistency and file locking).
Data is stored across multiple AZs within a region.
Read after write consistency.
Need to create mount targets and choose AZs to include (recommended to include all 
AZ’s).
Instances can be behind an ELB.

There are two performance modes:
• “General Purpose” performance mode is appropriate for most file systems.
• “Max I/O” performance mode is optimized for applications where tens, hundreds, 
or thousands of EC2 instances are accessing the file system.

### AWS STORAGE GATEWAY
AWS Storage Gateway is a hybrid cloud storage service that gives you on-premises access 
to virtually unlimited cloud storage.
Customers use Storage Gateway to simplify storage management and reduce costs for key 
hybrid cloud storage use cases.
These include moving backups to the cloud, using on-premises file shares backed by cloud 
storage, and providing low latency access to data in AWS for on-premises applications.
To support these use cases, Storage Gateway offers three different types of gateways:
• File Gateway – provides file system interfaces to on-premises servers.
• Volume Gateway – provides block-based access for on-premises servers.
• Tape Gateway – provides a virtual tape library that is compatible with common 
backup software (block and file interfaces).
#### AWS STORAGE QUIZ QUESTIONS

Answers and explanations are provided below after the last question in this section.

Question 1: What is the most cost-effective storage tier for data that is not often 
accessed, will be retained for 7 years, and needs to be retrievable within 24 hours?
1. Amazon S3 Standard
2. Amazon S3 Glacier
3. Amazon S3 Standard-Infrequent Access
4. Amazon S3 Glacier Deep Archive
   
Question 2: Which storage classes are available for the Amazon Elastic File System?
1. Standard, Provisioned Throughput
2. Standard, Deep Archive
3. Standard, Infrequent Access Storage
4. Standard, One-Zone IA
   
Question 3: Amazon S3 is an example of what type of storage system?
1. Object
2. Block
3. File
4. Hybrid
   
Question 4: With Amazon S3, objects are stored in which type of root-level container?
1. A folder
2. A file-system
3. A bucket
4. A region
   
Question 5: Amazon Elastic Block Store (EBS) volumes are stored within which construct?
1. A region
2. An edge location
3. A snapshot
4. An availability zone
   
Question 6: Which storage service can be used on-premises to access cloud storage?
1. Amazon S3 Glacier
2. Amazon Storage Block
3. AWS Storage Gateway
4. AWS Hybrid Service
   
Question 7: With default settings, what will happen to a root EBS volume when the 
Amazon EC2 instance is terminated?
1. It will be deleted
2. It will be retained
3. A snapshot will be retained
4. An AMI will be created
   
Question 8: Which Amazon Machine Image can be used to mount an Amazon Elastic File 
System (EFS) file system?
1. Microsoft Windows Server 2019 with Containers
2. Microsoft Windows Server 2016 Core
3. Amazon Linux 2 AMI
4. All of the above
Question 9: Which storage device is physically attached to the Amazon EC2 host servers?
1. Amazon Elastic Block Store (EBS) volume
2. Amazon Machine Image (AMI)
3. Instance Store volume
4. Elastic Network Adapter
Question 10: Which Amazon S3 storage class is used for archiving data for long term 
retention?
1. S3 Standard
2. S3 Intelligent-Tiering
3. S3 One Zone-IA
4. S3 Glacier Deep Archive
Question 11: Which storage service is used by Amazon EC2 instances for the root 
volume?
1. Amazon Simple Storage Service (S3)
2. Amazon Elastic File System (EFS)
3. Amazon Elastic Block Store (EBS)
4. Amazon Storage Gateway
#### AWS STORAGE ANSWERS

Question 1: What is the most cost-effective storage tier for data that is not often 
accessed, will be retained for 7 years, and needs to be retrievable within 24 hours?
1. Amazon S3 Standard
2. Amazon S3 Glacier
3. Amazon S3 Standard-Infrequent Access
4. Amazon S3 Glacier Deep Archive
Answer: 4
Explanation:
1 is incorrect. This is not the most affordable option for long term data storage
2 is incorrect. This is not the most affordable option for long term data storage where 
retrieval times of 24 hours are acceptable
3 is incorrect. This is not the most affordable option for long term data storage where 
retrieval times of 24 hours are acceptable
4 is correct. This is the most affordable option for long term data storage where 
retrieval times of 24 hours are acceptable

Question 2: Which storage classes are available for the Amazon Elastic File System?
1. Standard, Provisioned Throughput
2. 2. Standard, Deep Archive
3. Standard, Infrequent Access Storage
4. Standard, One-Zone IA
Answer: 3
Explanation:
1 is incorrect. Provisioned throughput is not a storage class, it is a way you can get 
better performance for additional cost
2 is incorrect. Deep Archive is a tier of Glacier storage, not EFS
3 is correct. These are the two storage classes available for EFS
4 is incorrect. One-Zone IA is an Amazon S3 storage class

Question 3: Amazon S3 is an example of what type of storage system?
1. Object
2. Block
3. File
4. Hybrid
Answer: 1
Explanation:
1 is correct. Amazon Simple Storage Service (S3) is an object-based storage system
2 is incorrect. Amazon Simple Storage Service (S3) is not a block-based storage system
3 is incorrect. Amazon Simple Storage Service (S3) is not a file-based storage system
4 is incorrect. Amazon Simple Storage Service (S3) is not a hybrid storage system. An 
example of a hybrid storage system would be Amazon Storage Gateway

Question 4: With Amazon S3, objects are stored in which type of root-level container?
1. A folder
2. A file-system
3. A bucket
4. A region
Answer: 3
Explanation:
1 is incorrect. You can create folders with Amazon S3 to mimic a hierarchy, but they 
are not root-level containers
2 is incorrect. Amazon S3 is an object-based storage system, there is no such thing as a 
file-system
3 is correct. A bucket is the root-level container in Amazon S3. You upload your objects 
into buckets
4 is incorrect. A region is not the root-level container in Amazon S3. Buckets are 
created within a region

Question 5: Amazon Elastic Block Store (EBS) volumes are stored within which construct?
1. A region
2. An edge location
3. A snapshot
4. An availability zone
Answer: 4
Explanation:
1 is incorrect. Amazon EBS volumes are not stored within a region. They are stored 
within another construct that is within a region. Guess again!
2 is incorrect. An edge location is not where you store EBS volumes. Edge Locations are 
used by the Amazon CloudFront service and will be discussed later in the course
3 is incorrect. You don't store an Amazon EBS volume in a snapshot, you take 
snapshots of EBS volumes to get point-in-time backups of the data in the volume
4 is correct. Amazon EBS volumes are stored with an availability zone.

Question 6: Which storage service can be used on-premises to access cloud storage?
1. Amazon S3 Glacier
2. Amazon Storage Block
3. AWS Storage Gateway
4. AWS Hybrid Service
Answer: 3
Explanation:
1 is incorrect. Amazon S3 Glacier is a cloud storage solution used for archiving data
2 is incorrect. There's no such thing as "Amazon Storage Block"
3 is correct. AWS Storage Gateway is a hybrid cloud storage service that gives you onpremises access to virtually unlimited cloud storage
4 is incorrect. There's no such thing as "AWS Hybrid Service"

Question 7: With default settings, what will happen to a root EBS volume when the 
Amazon EC2 instance is terminated?
1. It will be deleted
2. It will be retained
3. A snapshot will be retained
4. An AMI will be created
Answer: 1
Explanation:
1 is correct. With default settings an Amazon EBS root volume will be deleted when 
the instance is terminated
2 is incorrect. This is, not true with default settings. However, you can configure EBS volumes to be retained by changing the "Delete on termination" attribute
3 is incorrect. A snapshot is not automatically created when an instance is terminated
4 is incorrect. An AMI will not be created

Question 8: Which Amazon Machine Image can be used to mount an Amazon Elastic File 
System (EFS) file system?
1. Microsoft Windows Server 2019 with Containers
2. Microsoft Windows Server 2016 Core
3. Amazon Linux 2 AMI
4. All of the above
Answer: 3
Explanation:
1 is incorrect. You cannot use Microsoft Windows AMIs with Amazon EFS
2 is incorrect. You cannot use Microsoft Windows AMIs with Amazon EFS
3 is correct. Only Linux AMIs can be used with Amazon EFS
4 is incorrect. You cannot use Microsoft Windows AMIs with Amazon EFS

Question 9: Which storage device is physically attached to the Amazon EC2 host servers?
1. Amazon Elastic Block Store (EBS) volume
2. Amazon Machine Image (AMI)
3. Instance Store volume
4. Elastic Network Adapter
Answer: 3
Explanation:
1 is incorrect. Amazon EBS volumes are attached over a network, they are not 
physically attached to the EC2 host servers
2 is incorrect. An AMI is used to launch an instance, it is not a storage device
3 is correct. Instance store volumes are physically attached to EC2 host servers. They 
are ephemeral storage which means the data is lost when powered off
4 is incorrect. An ENA is not a storage device

Question 10: Which Amazon S3 storage class is used for archiving data for long term 
retention?
1. S3 Standard
2. S3 Intelligent-Tiering
3. S3 One Zone-IA
4. S3 Glacier Deep Archive
1 is incorrect. S3 Standard is durable, immediately available, frequently accessed 
storage
2 is incorrect. S3 Intelligent-Tiering automatically moves data to the most costeffective tier
3 is incorrect. S3 One Zone-IA is lower cost storage for infrequently accessed data with 
less resilience
4 is correct. S3 Glacier Deep Archive is the lowest cost storage class for long term 
retention

Question 11: Which storage service is used by Amazon EC2 instances for the root 
volume?
1. Amazon Simple Storage Service (S3)
2. Amazon Elastic File System (EFS)
3. Amazon Elastic Block Store (EBS)
4. Amazon Storage Gateway
Answer: 3
Explanation:
1 is incorrect. Amazon S3 is an object-based storage system and is not used for EC2 
root volumes
2 is incorrect. Amazon Elastic File System (EFS) is a file-based storage service. You can 
mount EFS filesystems to an EC2 instance, but you cannot use them for root volumes
3 is correct. Amazon Elastic Block Store (EBS) is used for the root volume on EBSbacked instances
4 is incorrect. Amazon Storage Gateway is a storage solution used for hybrid storage 
between on-premises and AWS Cloud







# AWS NETWORKING
This article covers AWS Networking which is a key technology area in the Cloud 
Practitioner exam blueprint
### AMAZON VIRTUAL PRIVATE CLOUD (VPC)
A virtual private cloud (VPC) is a virtual network dedicated to your AWS account.
Analogous to having your own DC inside AWS.
It is logically isolated from other virtual networks in the AWS Cloud.
Provides complete control over the virtual networking environment including selection of 
IP ranges, creation of subnets, and configuration of route tables and gateways.
You can launch your AWS resources, such as Amazon EC2 instances, into your VPC.
When you create a VPC, you must specify a range of IPv4 addresses for the VPC in the form 
of a Classless Inter-Domain Routing (CIDR) block; for example, 10.0.0.0/16.
This is the primary CIDR block for your VPC.
A VPC spans all the Availability Zones in the region.
You have full control over who has access to the AWS resources inside your VPC.
You can create your own IP address ranges, and create subnets, route tables and network 
gateways.
When you first create your AWS account a default VPC is created for you in each AWS 
region.
A default VPC is created in each region with a subnet in each AZ.
By default, you can create up to 5 VPCs per region.You can define dedicated tenancy for a VPC to ensure instances are launched on dedicated 
hardware (overrides the configuration specified at launch).
A default VPC is automatically created for each AWS account the first time Amazon EC2 
resources are provisioned.
The default VPC has all-public subnets.
Public subnets are subnets that have:
• “Auto-assign public IPv4 address” set to “Yes”.
• The subnet route table has an attached Internet Gateway.
Instances in the default VPC always have both a public and private IP address.
AZs names are mapped to different zones for different users (i.e. the AZ “ap-southeast-2a” 
may map to a different physical zone for a different user).
Components of a VPC:
• A Virtual Private Cloud: A logically isolated virtual network in the AWS cloud. You 
define a VPC’s IP address space from ranges you select.
• Subnet: A segment of a VPC’s IP address range where you can place groups of 
isolated resources (maps to an AZ, 1:1).
• Internet Gateway: The Amazon VPC side of a connection to the public Internet.
• NAT Gateway: A highly available, managed Network Address Translation (NAT) 
service for your resources in a private subnet to access the Internet.
• Hardware VPN Connection: A hardware-based VPN connection between your 
Amazon VPC and your datacenter, home network, or co-location facility.
• Virtual Private Gateway: The Amazon VPC side of a VPN connection.
• Customer Gateway: Your side of a VPN connection.
• Router: Routers interconnect subnets and direct traffic between Internet 
gateways, virtual private gateways, NAT gateways, and subnets.
• Peering Connection: A peering connection enables you to route traffic via private 
IP addresses between two peered VPCs.
• VPC Endpoints: Enables private connectivity to services hosted in AWS, from 
within your VPC without using an Internet Gateway, VPN, Network Address 
Translation (NAT) devices, or firewall proxies.
• Egress-only Internet Gateway: A stateful gateway to provide egress only access for 
IPv6 traffic from the VPC to the Internet.
Options for securely connecting to a VPC are:
• AWS managed VPN – fast to setup.
• Direct Connect – high bandwidth, low-latency but takes weeks to months to setup.
• VPN CloudHub – used for connecting multiple sites to AWS.
• Software VPN – use 3rd party software.

An Elastic Network Interface (ENI) is a logical networking component that represents a NIC.
ENIs can be attached and detached from EC2 instances, and the configuration of the ENI 
will be maintained.
Flow Logs capture information about the IP traffic going to and from network interfaces in a VPC.
Flow log data is stored using Amazon CloudWatch Logs.
Flow logs can be created at the following levels:
• VPC.
• Subnet.
• Network interface.
Peering connections can be created with VPCs in different regions (available in most 
regions now).

### SUBNETS
After creating a VPC, you can add one or more subnets in each Availability Zone.
When you create a subnet, you specify the CIDR block for the subnet, which is a subset of 
the VPC CIDR block.
Each subnet must reside entirely within one Availability Zone and cannot span zones.
Types of subnets:
• If a subnet’s traffic is routed to an internet gateway, the subnet is known as 
a public subnet.
• If a subnet doesn’t have a route to the internet gateway, the subnet is known as 
a private subnet.
• If a subnet doesn’t have a route to the internet gateway, but has its traffic routed 
to a virtual private gateway for a VPN connection, the subnet is known as a VPNonly subnet.
An Internet Gateway is a horizontally scaled, redundant, and highly available VPC 
component that allows communication between instances in your VPC and the internet.

### FIREWALLS
Network Access Control Lists (ACLs) provide a firewall/security layer at the subnet level.
Security Groups provide a firewall/security layer at the instance level.
The table below describes some differences between Security Groups and Network ACLs:![image](https://github.com/user-attachments/assets/eb4a57e8-aecf-46c1-b639-454f9770b41a)

#### VPC WIZARD
The VPC Wizard can be used to create the following four configurations:
VPC with a Single Public Subnet:
• Your instances run in a private, isolated section of the AWS cloud with direct 
access to the Internet.
• Network access control lists and security groups can be used to provide strict 
control over inbound and outbound network traffic to your instances.
• Creates a /16 network with a /24 subnet. Public subnet instances use Elastic IPs or 
Public IPs to access the Internet.
VPC with Public and Private Subnets:
• In addition to containing a public subnet, this configuration adds a private subnet 
whose instances are not addressable from the Internet.
• Instances in the private subnet can establish outbound connections to the Internet 
via the public subnet using Network Address Translation (NAT).
• Creates a /16 network with two /24 subnets.
• Public subnet instances use Elastic IPs to access the Internet.
• Private subnet instances access the Internet via Network Address Translation 
(NAT).
VPC with Public and Private Subnets and Hardware VPN Access:
• This configuration adds an IPsec Virtual Private Network (VPN) connection 
between your Amazon VPC and your data center – effectively extending your data 
center to the cloud while also providing direct access to the Internet for public 
subnet instances in your Amazon VPC.
• Creates a /16 network with two /24 subnets.
• One subnet is directly connected to the Internet while the other subnet is 
connected to your corporate network via an IPsec VPN tunnel.
VPC with a Private Subnet Only and Hardware VPN Access:
• Your instances run in a private, isolated section of the AWS cloud with a private 
subnet whose instances are not addressable from the Internet.
• You can connect this private subnet to your corporate data center via an IPsec 
Virtual Private Network (VPN) tunnel.
• Creates a /16 network with a /24 subnet and provisions an IPsec VPN tunnel 
between your Amazon VPC and your corporate network.
### NAT INSTANCES
NAT instances are managed by you.
Used to enable private subnet instances to access the Internet.
When creating NAT instances always disable the source/destination check on the instance.
NAT instances must be in a single public subnet.
NAT instances need to be assigned to security groups.
NAT Gateways
NAT gateways are managed for you by AWS.
NAT gateways are highly available in each AZ into which they are deployed.
They are preferred by enterprises.
Can scale automatically up to 45Gbps.
No need to patch.
Not associated with any security groups.
The table below describes some differences between NAT instances and NAT gateways:
![image](https://github.com/user-attachments/assets/81056f90-a287-4e7c-bb93-a5e6393f9102)
#### AWS DIRECT CONNECT (DX)
AWS Direct Connect is a network service that provides an alternative to using the Internet 
to connect a customer’s on-premises sites to AWS.
Data is transmitted through a private network connection between AWS and a customer’s 
data center or corporate network.
Benefits of Direct Connect:
• Reduce cost when using large volumes of traffic.
• Increase reliability (predictable performance).
• Increase bandwidth (predictable bandwidth).
• Decrease latency.
Each AWS Direct Connect connection can be configured with one or more virtual interfaces 
(VIFs).
Public VIFs allow access to public services such as S3, EC2, and DynamoDB.
Private VIFs allow access to your VPC.
From Direct Connect you can connect to all AZs within the Region.
You can establish IPSec connections over public VIFs to remote regions.
Direct Connect is charged by port hours and data transfer.
Available in 1Gbps and 10Gbps.
Speeds of 50Mbps, 100Mbps, 200Mbps, 300Mbps, 400Mbps, and 500Mbps can be 
purchased through AWS Direct Connect Partners.
Each connection consists of a single dedicated connection between ports on the customer 
router and an Amazon router.
for HA you must have 2 DX connections – can be active/active or active/standby.
Route tables need to be updated to point to a Direct Connect connection.

### AWS GLOBAL ACCELERATOR
AWS Global Accelerator is a service that improves the availability and performance of 
applications with local or global users.
It provides static IP addresses that act as a fixed entry point to application endpoints in a 
single or multiple AWS Regions, such as Application Load Balancers, Network Load 
Balancers or EC2 instances.
Uses the AWS global network to optimize the path from users to applications, improving 
the performance of TCP and UDP traffic.
AWS Global Accelerator continually monitors the health of application endpoints and will 
detect an unhealthy endpoint and redirect traffic to healthy endpoints in less than 1 
minute.
#### DETAILS AND BENEFITS
Uses redundant (two) static anycast IP addresses in different network zones (A and B).
The redundant pair are globally advertised.
Uses AWS Edge Locations – addresses are announced from multiple edge locations at the 
same time.
Addresses are associated to regional AWS resources or endpoints.
AWS Global Accelerator’s IP addresses serve as the frontend interface of applications.
Intelligent traffic distribution: Routes connections to the closest point of presence for 
applications.
Targets can be Amazon EC2 instances or Elastic Load Balancers (ALB and NLB).
By using the static IP addresses, you don’t need to make any client-facing changes or 
update DNS records as you modify or replace endpoints.
The addresses are assigned to your accelerator for as long as it exists, even if you disable 
the accelerator and it no longer accepts or routes traffic.

#### AWS OUTPOSTS
AWS Outposts is a fully managed service that offers the same AWS infrastructure, AWS 
services, APIs, and tools to virtually any datacenter, co-location space, or on-premises 
facility for a truly consistent hybrid experience.
AWS Outposts is ideal for workloads that require low latency access to on-premises 
systems, local data processing, data residency, and migration of applications with local 
system interdependencies.
AWS compute, storage, database, and other services run locally on Outposts, and you can 
access the full range of AWS services available in the Region to build, manage, and scale 
your on-premises applications using familiar AWS services and tools.
Outposts is available as a 42U rack that can scale from 1 rack to 96 racks to create pools of 
compute and storage capacity.
Services you can run on AWS Outposts include:
• Amazon EC2.
• Amazon EBS.
• Amazon S3.
• Amazon VPC.
• Amazon ECS/EKS.
• Amazon RDS.
• Amazon EMR.
#### AWS NETWORKING QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: What is the scope of an Amazon VPC?
1. A data center
2. A region
3. An availability zone
4. A subnet
   
Question 2: Which type of firewall operates at the instance level?
1. A security group
2. A network access control list (NACL)
3. A route table
4. A NAT Gateway
Question 3: How can an organization create a private hybrid cloud connection between 
their on-premises data center and the AWS Cloud?
1. AWS managed VPN
2. VPN CloudHub
3. Software VPN
4. AWS Direct Connect
Question 4: Which type of public IP address is retained when the instance is stopped?
1. Public IP address
2. Private IP address
3. Elastic IP address
4. Local IP address
Question 5: Which AWS-managed network service can be used to enable Internet 
connectivity for EC2 instances in private subnets?
1. NAT Instance
2. NAT Gateway
3. Internet Gateway
4. Network ACL
Question 6: A company needs a network connection to the AWS cloud with predictable 
performance. What should they use?
1. AWS managed VPN
2. AWS Direct Connect
3. VPN CloudHub
4. VPC Peering
Question 7: With Amazon Virtual Private Cloud (VPC) what must you pay for?
1. Internet Gateway
2. Route Table
3. Security Group
4. VPN Connection
AWS NETWORKING ANSWERS
Question 1: What is the scope of an Amazon VPC?
1. A data center
2. A region
3. An availability zone
4. A subnet
Answer: 2
Explanation:
1 is incorrect. The scope of a VPC is not a data center. AWS never talk in terms of data 
centers as these are transparent to the user
2 is correct. An Amazon VPC is created within a region. You can create multiple VPCs 
within a region and there is a default VPC created in every AWS region by default
3 is incorrect. You do not create VPC's within availability zones. AZs are actually 
constructs to which you assign subnets within your VPC
4 is incorrect. A subnet is assigned to an availability zone, you don't create a VPC in a 
subnet
Question 2: Which type of firewall operates at the instance level?
1. A security group
2. A network access control list (NACL)
3. A route table
4. A NAT Gateway
Answer: 1
Explanation:
1 is correct. Security groups are considered to be instance-level firewalls
2 is incorrect. A network access control list or NACL is a subnet-level firewall
3 is incorrect. A route table is not a firewall. It is used to direct network traffic
4 is incorrect. A NAT Gateway is not a firewall. It is used to provide Internet access to 
EC2 instances in private subnets
Question 3: How can an organization create a private hybrid cloud connection between 
their on-premises data center and the AWS Cloud?
1. AWS managed VPN
2. VPN CloudHub
3. Software VPN
4. AWS Direct Connect
Answer: 4
Explanation:
1 is incorrect. A virtual private network (VPN) is a connection over the public Internet 
and is therefore not considered private
2 is incorrect. A virtual private network (VPN) is a connection over the public Internet 
and is therefore not considered private
3 is incorrect. A virtual private network (VPN) is a connection over the public Internet 
and is therefore not considered private
4 is correct. AWS Direct Connect is a private network connection to the AWS Cloud. It 
provides high bandwidth and low latency with reliable performance
Question 4: Which type of public IP address is retained when the instance is stopped?
1. Public IP address
2. Private IP address
3. Elastic IP address
5. Local IP address
Answer: 3
Explanation:
1 is incorrect. Public IP addresses are lost when the instance is stopped
2 is incorrect. A private IP address is not a public IP address
3 is correct. With Elastic IP addresses, the address is retained when the instance is 
stopped. Remember that you do pay for unused Elastic IP addresses
4 is incorrect. This is not a type of Public IP address
Question 5: Which AWS-managed network service can be used to enable Internet 
connectivity for EC2 instances in private subnets?
1. NAT Instance
2. NAT Gateway
3. Internet Gateway
4. Network ACL
Answer: 2
Explanation:
1 is incorrect. A NAT instance is an EC2 instance managed by you that can be used for 
enabling instance in private subnets to access the Internet
2 is correct. A NAT Gateway is an AWS managed service that can be used for enabling 
instance in private subnets to access the Internet
3 is incorrect. An Internet Gateway is attached to a VPC to enable Internet 
connectivity. However, you need a NAT Instance or NAT Gateway to enable instance 
in private subnets to access the Internet using the Internet Gateway
4 is incorrect. A network ACL is a subnet-level firewall
Question 6: A company needs a network connection to the AWS cloud with predictable 
performance. What should they use?
1. AWS managed VPN
2. AWS Direct Connect
3. VPN CloudHub
4. VPC Peering
Answer: 2
Explanation:
1 is incorrect. Because a VPN uses the public Internet, it doesn't offer predictable 
performance
2 is correct. AWS Direct Connect is a private network connection and offers predictable 
performance
3 is incorrect. Because a VPN uses the public Internet, it doesn't offer predictable 
performance
4 is incorrect. VPC Peering is a method of connecting two VPCs together, not for 
connecting into AWS from an organization
Question 7: With Amazon Virtual Private Cloud (VPC) what must you pay for?
1. Internet Gateway
2. Route Table
3. Security Group
4. VPN Connection
Answer: 4
Explanation:
1 is incorrect. You do not need to pay for Internet Gateways
2 is incorrect. You do not need to pay for Route Tables
3 is incorrect. You do not need to pay for Security Groups
4 is correct. You do need to pay for VPN connections





# AWS DATABASES

This article covers AWS Databases for the AWS Cloud Practitioner exam. This is one of the 
key technology areas covered in the exam blueprint.
USE CASES FOR DIFFERENT DATABASE TYPES
The table below provides guidance on the typical use cases for several AWS database/data 
store services:
![image](https://github.com/user-attachments/assets/8c3f9165-a3fb-4824-bab8-8e84b112990b)

## AMAZON RELATIONAL DATABASE SERVICE (RDS)
Amazon Relational Database Service (Amazon RDS) is a managed service that makes it easy 
to set up, operate, and scale a relational database in the cloud.
Relational databases are known as Structured Query Language (SQL) databases.
Non-relational databases are known as NoSQL databases.
RDS is an Online Transaction Processing (OLTP) type of database.
RDS features and benefits:
• SQL type of database.
• Can be used to perform complex queries and joins.
• Easy to setup, highly available, fault tolerant, and scalable.
• Used when data is clearly defined.
• Common use cases include online stores and banking systems.
Amazon RDS supports the following database engines:
• SQL Server.
• Oracle.
• MySQL Server.
• PostgreSQL.
• Aurora.
• MariaDB.
Aurora is Amazon’s proprietary database.
RDS is a fully managed service and you do not have access to the underlying EC2 instance 
(no root access).
The RDS service includes the following:
• Security and patching of the DB instances.
• Automated backup for the DB instances.
• Software updates for the DB engine.
• Easy scaling for storage and compute.
• Multi-AZ option with synchronous replication.
• Automatic failover for Multi-AZ option.
• Read replicas option for read heavy workloads.
A DB instance is a database environment in the cloud with the compute and storage 
resources you specify.
Encryption:
• You can encrypt your Amazon RDS instances and snapshots at rest by enabling the 
encryption option for your Amazon RDS DB instance.
• Encryption at rest is supported for all DB types and uses AWS KMS.
• You cannot encrypt an existing DB, you need to create a snapshot, copy it, encrypt 
the copy, then build an encrypted DB from the snapshot.
DB Subnet Groups:
• A DB subnet group is a collection of subnets (typically private) that you create in a 
VPC and that you then designate for your DB instances.
• Each DB subnet group should have subnets in at least two Availability Zones in 
each region.
• It is recommended to configure a subnet group with subnets in each AZ (even for 
standalone instances).
AWS Charge for:
• DB instance hours (partial hours are charged as full hours).
• Storage GB/month.
• I/O requests/month – for magnetic storage.
• Provisioned IOPS/month – for RDS provisioned IOPS SSD.
• Egress data transfer.
• Backup storage (DB backups and manual snapshots).
Scalability:
• You can only scale RDS up (compute and storage).
• You cannot decrease the allocated storage for an RDS instance.
• You can scale storage and change the storage type for all DB engines except MS 
SQL.
RDS provides multi-AZ for disaster recovery which provides fault tolerance across 
availability zones:
• Multi-AZ RDS creates a replica in another AZ and synchronously replicates to it (DR 
only).
• There is an option to choose multi-AZ during the launch wizard.
• AWS recommends the use of provisioned IOPS storage for multi-AZ RDS DB 
instances.
• Each AZ runs on its own physically distinct, independent infrastructure, and is 
engineered to be highly reliable.
• You cannot choose which AZ in the region will be chosen to create the standby DB 
instance.
Read Replicas – provide improved performance for reads:
• Read replicas are used for read heavy DBs and replication is asynchronous.
• Read replicas are for workload sharing and offloading.
• Read replicas provide read-only DR.
• Read replicas are created from a snapshot of the master instance.
• Must have automated backups enabled on the primary (retention period > 0)

## AMAZON DYNAMODB

Amazon DynamoDB is a fully managed NoSQL database service that provides fast and 
predictable performance with seamless scalability.
Dynamo DB features and benefits:
• NoSQL type of database (non-relational).
• Fast, highly available, and fully managed.
• Used when data is fluid and can change.
• Common use cases include social networks and web analytics.
Push button scaling means that you can scale the DB at any time without incurring 
downtime.
SSD based and uses limited indexing on attributes for performance.
DynamoDB is a Web service that uses HTTP over SSL (HTTPS) as a transport and JSON as a 
message serialization format.
Amazon DynamoDB stores three geographically distributed replicas of each table to enable 
high availability and data durability.
Data is synchronously replicated across 3 facilities (AZs) in a region.
Cross-region replication allows you to replicate across regions:
• Amazon DynamoDB global tables provides a fully managed solution for deploying a 
multi-region, multi-master database.
• When you create a global table, you specify the AWS regions where you want the 
table to be available.
• DynamoDB performs all the necessary tasks to create identical tables in these 
regions and propagate ongoing data changes to all of them.
Provides low read and write latency.
Scale storage and throughput up or down as needed without code changes or downtime.
DynamoDB is schema-less.
DynamoDB can be used for storing session state.
Provides two read models.
Eventually consistent reads (Default):
• The eventual consistency option maximizes your read throughput (best read 
performance).
• An eventually consistent read might not reflect the results of a recently completed 
write.
• Consistency across all copies reached within 1 second.
Strongly consistent reads:
• A strongly consistent read returns a result that reflects all writes that received a 
successful response prior to the read (faster consistency).
Amazon DynamoDB Accelerator (DAX) is a fully managed, highly available, in-memory cache for DynamoDB that delivers up to a 10x performance improvement – from 
milliseconds to microseconds – even at millions of requests per second.
AMAZON REDSHIFT
Amazon Redshift is a fast, fully managed data warehouse that makes it simple and costeffective to analyze all your data using standard SQL and existing Business Intelligence (BI) 
tools.
RedShift is a SQL based data warehouse used for analytics applications.
RedShift is a relational database that is used for Online Analytics Processing (OLAP) use 
cases.
RedShift is used for running complex analytic queries against petabytes of structured data, 
using sophisticated query optimization, columnar storage on high-performance local disks, 
and massively parallel query execution.
RedShift is ideal for processing large amounts of data for business intelligence.
RedShift is 10x faster than a traditional SQL DB.
RedShift uses columnar data storage:
• Data is stored sequentially in columns instead of rows.
• Columnar based DB is ideal for data warehousing and analytics.
• Requires fewer I/Os which greatly enhances performance.
RedShift provides advanced compression:
• Data is stored sequentially in columns which allows for much better performance 
and less storage space.
• RedShift automatically selects the compression scheme.
RedShift uses replication and continuous backups to enhance availability and improve 
durability and can automatically recover from component and node failures.
RedShift always keeps three copies of your data:
• The original.
• A replica on compute nodes (within the cluster).
• A backup copy on S3.
RedShift provides continuous/incremental backups:
• Multiple copies within a cluster.
• Continuous and incremental backups to S3.
• Continuous and incremental backups across regions.
• Streaming restore.
RedShift provides fault tolerance for the following failures:
• Disk failures.
• Nodes failures.
• Network failures.
• AZ/region level disasters.
AMAZON ELASTICACHE
ElastiCache is a web service that makes it easy to deploy and run Memcached or Redis 
protocol-compliant server nodes in the cloud.
The in-memory caching provided by ElastiCache can be used to significantly improve 
latency and throughput for many read-heavy application workloads or compute-intensive 
workloads.
Best for scenarios where the DB load is based on Online Analytics Processing (OLAP) 
transactions.
The following table describes a few typical use cases for ElastiCache:
![image](https://github.com/user-attachments/assets/e3733eea-5a7d-474c-8f3f-ebbf44442f4c)

ElastiCache EC2 nodes cannot be accessed from the Internet, nor can they be accessed by 
EC2 instances in other VPCs.
Can be on-demand or reserved instances too (but not Spot instances).
ElastiCache can be used for storing session state.
There are two types of ElastiCache engine:
• Memcached – simplest model, can run large nodes with multiple cores/threads, 
can be scaled in and out, can cache objects such as DBs.
• Redis – complex model, supports encryption, master / slave replication, cross AZ 
(HA), automatic failover and backup/restore.


## AMAZON EMR
Amazon EMR is a web service that enables businesses, researchers, data analysts, and 
developers to process vast amounts of data easily and cost-effectively.
EMR utilizes a hosted Hadoop framework running on Amazon EC2 and Amazon S3.
Managed Hadoop framework for processing huge amounts of data.
Also support Apache Spark, HBase, Presto and Flink.
Most commonly used for log analysis, financial analysis, or extract, translate and loading 
(ETL) activities.

## AWS DATABASES QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: Amazon Relational Database Service (RDS) is an example of what type of 
database?
1. Online transaction processing (OLTP)
2. Online analytics processing (OLAP)
3. No-SQL
4. Data warehouse
   
Question 2: Which AWS database service offers seamless horizontal scaling?
1. Amazon RDS
2. Amazon RedShift
3. Amazon DynamoDB
4. Database on Amazon EC2
   
Question 3: How can fault tolerance be added to an Amazon RDS database?
1. Using read replicas
2. Using multi-AZ
3. Using Global Replicas
4. Using EBS snapshots
   
Question 4: How can an organization enable microsecond latency for a 
DynamoDB database?
1. Using Amazon ElastiCache
2. Using DynamoDB Auto Scaling
3. Using Read Replicas
4. Using DynamoDB Accelerator (DAX)
   
Question 5: Which AWS database service is a relational, data warehouse? 
1. Amazon RedShift
2. Amazon RDS Aurora
3. Amazon DynamoDB
4. Amazon ElastiCache
   
Question 6: Why might an organization decide to move an on-premises database to 
Amazon RDS?
1. To reduce operational overhead
2. To increase flexibility
3. To eliminate the need to patch management
4. To benefit from seamless scalability
   
Question 7: How do you increase the capacity of an Amazon RDS database?
1. Scaling horizontally, by adding instances
2. Scaling horizontally, by adding RCUs/WCUs
3. Scaling vertically, by changing instance type
4. Scaling vertically by adding CPUs
   
Question 8: Amazon DynamoDB is good for which use case?
1. Structured data, rigid schema
2. Unstructured data, flexible schema
   





















