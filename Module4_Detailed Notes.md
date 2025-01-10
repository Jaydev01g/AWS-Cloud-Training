# AWS SECURITY SERVICES

As an AWS customer you inherit all the best practices of AWS policies, architecture, and 
operational processes.
The AWS Cloud enables a shared responsibility model.
AWS manages security OF the cloud; you are responsible for security IN the cloud.
You retain control of the security you choose to implement to protect your own content, 
platform, applications, systems, and networks no differently than you would in an on-site 
data center.

### BENEFITS OF AWS SECURITY
• Keep Your Data Safe – the AWS infrastructure puts strong safeguards in place to 
help.
• Protect your privacy – All data is stored in highly secure AWS data centers.
• Meet Compliance Requirements – AWS manages dozens of compliance programs 
in its infrastructure. This means that segments of your compliance have already 
been completed.
• Save Money – cut costs by using AWS data centers. Maintain the highest standard 
of s security without having to manage your own facility.
• Scale Quickly – security scales with your AWS Cloud usage. No matter the size of 
your business, the AWS infrastructure is designed to keep your data safe.

### COMPLIANCE
AWS Cloud Compliance enables you to understand the robust controls in place at AWS to 
maintain security and data protection in the cloud.
As systems are built on top of AWS Cloud infrastructure, compliance responsibilities will be 
shared.
Compliance programs include:
• Certifications / attestations.
• Laws, regulations, and privacy.
• Alignments / frameworks.

## AWS ARTIFACT
AWS Artifact is your go-to, central resource for compliance-related information that 
matters to you.
It provides on-demand access to AWS’ security and compliance reports and select online 
agreements.
Reports available in AWS Artifact include our Service Organization Control (SOC) reports, 
Payment Card Industry (PCI) reports, and certifications from accreditation bodies across 
geographies and compliance verticals that validate the implementation and operating 
effectiveness of AWS security controls.
Agreements available in AWS Artifact include the Business Associate Addendum (BAA) and 
the Nondisclosure Agreement (NDA).

## AMAZON GUARDDUTY

Amazon GuardDuty offers threat detection and continuous security monitoring for 
malicious or unauthorized behavior to help you protect your AWS accounts and workloads.
Intelligent threat detection service.
Detects account compromise, instance compromise, malicious reconnaissance, and bucket 
compromise.
Continuous monitoring for events across:
• AWS CloudTrail Management Events.
• AWS CloudTrail S3 Data Events.
• Amazon VPC Flow Logs.
• DNS Logs.

## AWS WAF & AWS SHIELD
#### WAF:
• AWS WAF is a web application firewall.
• Protects against common exploits that could compromise application availability, 
compromise security, or consume excessive resources.
• WAF lets you create rules to filter web traffic based on conditions that include IP 
addresses, HTTP headers and body, or custom URIs.
• WAF makes it easy to create rules that block common web exploits like SQL 
injection and cross site scripting.
• The rules are known as Web ACLs.
#### Shield:
• AWS Shield is a managed Distributed Denial of Service (DDoS) protection service.
• Safeguards web application running on AWS with always-on detection and 
automatic inline mitigations.
• Helps to minimize application downtime and latency.
• Two tiers – Standard and Advanced.

## AWS KEY MANAGEMENT SERVICE (AWS KMS)
AWS Key Management Service gives you centralized control over the encryption keys used 
to protect your data.
You can create, import, rotate, disable, delete, define usage policies for, and audit the use 
of encryption keys used to encrypt your data.
AWS Key Management Service is integrated with most other AWS services making it easy 
to encrypt the data you store in these services with encryption keys you control.
AWS KMS is integrated with AWS CloudTrail which provides you the ability to audit who 
used which keys, on which resources, and when.
AWS KMS enables developers to easily encrypt data, whether through 1-click encryption in 
the AWS Management Console or using the AWS SDK to easily add encryption in their 
application code.

# AWS CLOUDHSM
AWS CloudHSM is a cloud-based hardware security module (HSM) that enables you to 
easily generate and use your own encryption keys on the AWS Cloud.
With CloudHSM, you can manage your own encryption keys using FIPS 140-2 Level 3 
validated HSMs.
CloudHSM offers you the flexibility to integrate with your applications using industrystandard APIs, such as PKCS#11, Java Cryptography Extensions (JCE), and Microsoft 
CryptoNG (CNG) libraries.

## AWS CERTIFICATE MANAGER
AWS Certificate Manager is a service that lets you easily provision, manage, and deploy 
public and private Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates for 
use with AWS services and your internal connected resources.
SSL/TLS certificates are used to secure network communications and establish the identity 
of websites over the Internet as well as resources on private networks.
AWS Certificate Manager removes the time-consuming manual process of purchasing, 
uploading, and renewing SSL/TLS certificates.

### AWS INSPECTOR AND AWS TRUSTED ADVISOR

#### AWS Inspector:
• Inspector is an automated security assessment service that helps improve thesecurity and compliance of applications deployed on AWS.
• Inspector automatically assesses applications for vulnerabilities or deviations from best practices.
• Uses an agent installed on EC2 instances.
• Instances must be tagged.

#### AWS Trusted Advisor:
• Trusted Advisor is an online resource that helps to reduce cost, increase 
performance, and improve security by optimizing your AWS environment.
• Trusted Advisor provides real time guidance to help you provision your resources 
following best practices.
• Advisor will advise you on Cost Optimization, Performance, Security, and Fault 
Tolerance.
Trusted Advisor scans your AWS infrastructure and compares is to AWS best practices in 
five categories:
• Cost Optimization.
• Performance.
• Security.
• Fault Tolerance.
• Service Limits.
Trusted Advisor comes in two versions.
##### Core Checks and Recommendations (free):
• Access to the 7 core checks to help increase security and performance.
• Checks include S3 bucket permissions, Security Groups, IAM use, MFA on root 
account, EBS public snapshots, RDS public snapshots.
Full Trusted Advisor Benefits (business and enterprise support plans):
• Full set of checks to help optimize your entire AWS infrastructure.
• Advises on security, performance, cost, fault tolerance and service limits.
• Additional benefits include weekly update notifications, alerts, automated actions 
with CloudWatch and programmatic access using the AWS Support API.

### PENETRATION TESTING
Penetration testing is the practice of testing one’s own application’s security for 
vulnerabilities by simulating an attack.
AWS allows penetration testing. There is a limited set of resources on which penetration 
testing can be performed.
You do not need permission to perform penetration testing against the following services:
• Amazon EC2 instances, NAT Gateways, and Elastic Load Balancers.
• Amazon RDS.
• Amazon CloudFront.
• Amazon Aurora.
• Amazon API Gateways.
• AWS Lambda and Lambda Edge functions.
• Amazon LightSail resources.
• Amazon Elastic Beanstalk environments.
You can read the full vulnerability and penetration testing support policy here.
In case an account is or may be compromised, AWS recommend that the following steps are taken:
1. Change your AWS root account password.
2. Change all IAM user’s passwords.
3. Delete or rotate all programmatic (API) access keys.
4. Delete any resources in your account that you did not create.
5. Respond to any notifications you received from AWS through the AWS Support 
Center and/or contact AWS Support to open a support case.

### AWS SINGLE SIGN-ON (AWS SSO)

AWS Single Sign-On is a cloud-based single sign-on (SSO) service that makes it easy to centrally manage SSO access to all your AWS accounts and cloud applications.
It helps you manage SSO access and user permissions across all your AWS accounts in AWS Organizations.
AWS SSO also helps you manage access and permissions to commonly used third-party software as a service (SaaS) applications, AWS SSO-integrated applications as well as 
custom applications that support Security Assertion Markup Language (SAML) 2.0.
AWS SSO includes a user portal where your end-users can find and access all their assigned AWS accounts, cloud applications, and custom applications in one place.

### AMAZON COGNITO
Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and 
mobile apps quickly and easily.
Amazon Cognito scales to millions of users and supports sign-in with social identity 
providers, such as Apple, Facebook, Google, and Amazon, and enterprise identity providers 
via SAML 2.0 and OpenID Connect.
The two main components of AWS Cognito are user pools and identity pools:
• User pools are user directories that provide sign-up and sign-in options for your 
app users.
• Identity pools enable you to grant your users access to other AWS services.
You can use identity pools and user pools separately or together.

#### AWS DIRECTORY SERVICES
AWS provides several directory types.
The following three types currently feature on the exam and will be covered on this page:
• Active Directory Service for Microsoft Active Directory.
• Simple AD.
• AD Connector.
As an alternative to the AWS Directory service, you can build your own Microsoft AD DCs in 
the AWS cloud (on EC2).
The table below summarizes the directory services covered on this page as well as a couple 
of others, and provides some typical use cases:![image](https://github.com/user-attachments/assets/b835a245-8e1f-48af-8ead-a08a6e3d2dca)

### AWS SYSTEMS MANAGER PARAMETER STORE

Provides secure, hierarchical storage for configuration data management and secrets management.
It is highly scalable, available, and durable.You can store data such as passwords, database strings, and license codes as parameter 
values.You can store values as plaintext (unencrypted data) or ciphertext (encrypted data).
You can then reference values by using the unique name that you specified when you created the parameter.

##### AWS SECRETS MANAGER
Like Parameter Store.
Allows native and automatic rotation of keys.
Fine-grained permissions.
Central auditing for secret rotation.
AWS ARTIFACT
AWS Artifact is your go-to, central resource for compliance-related information that 
matters to you.
It provides on-demand access to AWS’ security and compliance reports and select online 
agreements.
Reports available in AWS Artifact include our Service Organization Control (SOC) reports, 
Payment Card Industry (PCI) reports, and certifications from accreditation bodies across 
geographies and compliance verticals that validate the implementation and operating 
effectiveness of AWS security controls.Agreements available in AWS Artifact include the Business Associate Addendum (BAA) and 
the Nondisclosure Agreement (NDA).

### AWS SECURITY QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: Which tool can be used to find compliance information that relates to the 
AWS Cloud platform?
1. Amazon Inspector
2. AWS Trusted Advisor
3. AWS Artifact
4. AWS Personal Health Dashboard

Question 2: What is AWS' policy regarding penetration testing?
1. You can only perform penetration testing with permission from AWS
2. You can perform penetration testing against any service and account
3. You can perform penetration testing against selected services without approval
4. Penetration testing is not allowed under any circumstance

Question 3: Which service can assist with protecting against common web-based 
exploits?
1. AWS Shield
2. AWS Web Application Firewall (WAF)
3. Amazon Route 53
4. AWS CloudHSM

Question 4: Which service is involved with encryption?
1. AWS Key Management Service (KMS)
2. AWS WAF
3. AWS Shield

Question 5: In case of account compromise, which of the following actions should you 
perform?
1. Delete all IAM users
2. Delete all resources in your account
3. Open a support case with AWS
4. Immediately close your account



# AWS SHARED RESPONSIBILITY MODEL

The AWS shared responsibility model defines what you (as an AWS account holder/user) 
and AWS are responsible for when it comes to security and compliance.
Security and Compliance is a shared responsibility between AWS and the customer. This 
shared model can help relieve customer’s operational burdens as AWS operates, manages, 
and controls the components from the host operating system and virtualization layer down 
to the physical security of the facilities in which the service operates.
The customer assumes responsibility and management of the guest operating system 
(including updates and security patches), other associated application software as well as 
the configuration of the AWS provided security group firewall.
AWS are responsible for “Security of the Cloud”.
• AWS is responsible for protecting the infrastructure that runs all the services 
offered in the AWS Cloud.
• This infrastructure is composed of the hardware, software, networking, and 
facilities that run AWS Cloud services.
Customers are responsible for “Security in the Cloud”.
• For EC2 this includes network level security (NACLs, security groups), operating 
system patches and updates, IAM user access management, and client and serverside data encryption.

• Physical and Environmental controls.
Shared Controls – Controls which apply to both the infrastructure layer and customer 
layers, but in separate contexts or perspectives.
In the AWS shared security model, a shared control, AWS provides the requirements for 
the infrastructure and the customer must provide their own control implementation within 
their use of AWS services.
Examples of shared controls include:
• Patch Management – AWS is responsible for patching and fixing flaws within the 
infrastructure, but customers are responsible for patching their guest OS and 
applications.
• Configuration Management – AWS maintains the configuration of its 
infrastructure devices, but a customer is responsible for configuring their own 
guest operating systems, databases, and applications.
• Awareness & Training – AWS trains AWS employees, but a customer must train 
their own employees.
Customer Specific – Controls which are solely the responsibility of the customer based on 
the application they are deploying within AWS services.
Examples of customer specific controls include:
• Service and Communications Protection or Zone Security which may require a 
customer to route or zone data within specific security environments.
AWS SHARED RESPONSIBILITY MODEL QUIZ 
QUESTIONS
Answers and explanations are provided below after the last question in this section.

Question 1: According to the AWS Shared Responsibility model, who is responsible for 
operating system patching for Amazon EC2 instances?
1. AWS
2. The Customer

Question 2: According to the AWS Shared Responsibility model, who is responsible for 
configuring server-side encryption for Amazon S3?
1. AWS
2. The Customer

Question 3: According to the AWS Shared Responsibility model, who is responsible for 
data center security?
1. AWS
2. The customer

Question 4: Which service uses a hardware security module to protect encryption keys in 
the cloud?
1. AWS Key Management Service (KMS)
2. AWS CloudHSM
3. AWS Service Catalog

Question 5: Which service can be used to find reports on Payment Card Industry (PCI) 
compliance of the AWS cloud?
1. AWS Service Catalog
2. Amazon Inspector
3. AWS Artifact

Question 6: Who is responsible for patching networking equipment in AWS?
1. AWS
2. The Customer



# ARCHITECTING FOR THE CLOUD 
Architecting for the Cloud is one of the key subjects tested on the Cloud Practitioner exam. 
This can be dry subject, especially if you’re from a non-technical background, but please 
ensure you’re familiar with the concepts at a high-level as questions do come up on the 
exam.
Please read the following AWS Blog article for additional information:
https://aws.amazon.com/blogs/apn/the-6-pillars-of-the-aws-well-architected-framework/
Cloud computing differs from a traditional environment in the following ways:

## IT ASSETS BECOME PROGRAMMABLE RESOURCES
On AWS, servers, databases, storage, and higher-level application components can be 
instantiated within seconds.
You can treat these as temporary and disposable resources, free from the inflexibility and 
constraints of a fixed and finite IT infrastructure.
This resets the way you approach change management, testing, reliability, and capacity 
planning.

### GLOBAL, AVAILABLE, AND UNLIMITED CAPACITY
Using the global infrastructure of AWS, you can deploy your application to the AWS 
Region that best meets your requirements.
For global applications, you can reduce latency to end users around the world by using the 
Amazon CloudFront content delivery network.
It is also much easier to operate production applications and databases across multiple 
data centers to achieve high availability and fault tolerance.

### HIGHER LEVEL MANAGED SERVICES
AWS customers also have access to a broad set of compute, storage, database, analytics, 
application, and deployment services.
These services are instantly available to developers and can reduce dependency on inhouse specialized skills and allow organizations to deliver new solutions faster.
These services are managed by AWS, which can lower operational complexity and cost.

### SECURITY BUILT-IN
The AWS cloud provides governance capabilities that enable continuous monitoring of 
configuration changes to your IT resources.
Since AWS assets are programmable resources, your security policy can be formalized and 
embedded with the design of your infrastructure.

### DESIGN PRINCIPLES SCALABILITY
Systems that are expected to grow over time need to be built on top of a scalable 
architecture.


#### Scaling Vertically
Scaling vertically takes place through an increase in the specifications of an individual 
resource (e.g., upgrading a server with a larger hard drive or a faster CPU).
On Amazon EC2, this can easily be achieved by stopping an instance and resizing it to an 
instance type that has more RAM, CPU, IO, or networking capabilities.
#### Scaling Horizontally
Scaling horizontally takes place through an increase in the number of resources (e.g., 
adding more hard drives to a storage array or adding more servers to support an 
application).
This is a great way to build Internet-scale applications that leverage the elasticity of cloud 
computing.
The table below provides more information on the differences between horizontal and 
vertical scaling:![image](https://github.com/user-attachments/assets/c21a5859-31ac-4017-bbb1-7ee0ec98cd02)
Stateless applications:
• A stateless application is an application that needs no knowledge of previous 
interactions and stores no session information.
• A stateless application can scale horizontally since any request can be serviced by 
any of the available compute resources (e.g., EC2 instances, AWS Lambda 
functions).
Stateless components:
• Most applications need to maintain state information.
• For example, web applications need to track whether a user is signed in, or elsethey might present personalized content based on previous actions.
• Web applications can use HTTP cookies to store information about a session at the 
client’s browser (e.g., items in the shopping cart).
• Consider only storing a unique session identifier in a HTTP cookie and storing more 
detailed user session information server-side.
• DynamoDB is often used for storing session state to maintain a stateless 
architecture.
• For larger files a shared storage system can be used such as S3 or EFS.
• SWF can be used for a multi-step workflow.
Stateful components:
• Databases are stateful.
• Many legacy applications are stateful.
• Load balancing with session affinity can be used for horizontal scaling of stateful 
components.
• Session affinity is however not guaranteed and existing sessions do not benefit 
from newly launched nodes.
Distributed processing:
• Use cases that involve processing of very large amounts of data (e.g., anything that 
can’t be handled by a single compute resource in a timely manner) require a 
distributed processing approach.
• By dividing a task and its data into many small fragments of work, you can execute 
each of them in any of a larger set of available compute resources.



# DISPOSABLE RESOURCES INSTEAD OF FIXED SERVERS
Think of servers and other components as temporary resources.
Launch as many as you need and use them only for as long as you need them.
An issue with fixed, long-running servers is that of configuration drift (where change and 
software patches are applied over time).
This problem can be solved with the “immutable infrastructure” pattern where a server is 
never updated but instead is replaced with a new one as required.

## INSTANTIATING COMPUTE RESOURCES
You don’t want to manually set up new resources with their configuration and code.
Use automated, repeatable processes that avoid long lead times and are not prone to 
human error.
Bootstrapping:
• Execute automated bootstrapping actions to modify default configurations.
• This includes scripts that install software or copy data to bring that resource to a 
particular state.
• You can parameterize configuration details that vary between different environments.
Golden Images:
• Some resource types can be launched from a golden image.
• Examples are EC2 instances, RDS instances and EBS volumes.
• A golden image is a snapshot of a particular state for that resource.
• Compared to bootstrapping golden images provide faster start times and remove 
dependencies to configuration services or third-party repositories.
Infrastructure are Code:
• AWS assets are programmable, so you can apply techniques, practices, and tools 
from software development to make your whole infrastructure reusable, 
maintainable, extensible, and testable.

#### AUTOMATION
In a traditional IT infrastructure, you often must manually react to a variety of events.
When deploying on AWS there is a lot of opportunity for automation.
This improves both your system’s stability and the efficiency of your organization.
Examples of automations using AWS services include:
• AWS Elastic Beanstalk – the fastest and simplest way to get an application up and 
running on AWS.
• Amazon EC2 Auto Recovery – You can create an Amazon CloudWatch alarm that 
monitors an Amazon EC2 instance and automatically recovers it if it becomes 
impaired.
• Auto Scaling – With Auto Scaling, you can maintain application availability and 
scale your Amazon EC2 capacity up or down automatically according to conditions 
you define.
• Amazon CloudWatch Alarms – You can create a CloudWatch alarm that sends an 
Amazon Simple Notification Service (Amazon SNS) message when a particular 
metric goes beyond a specified threshold for a specified number of periods.
• Amazon CloudWatch Events – The CloudWatch service delivers a near real-time 
stream of system events that describe changes in AWS resources.
• AWS OpsWorks Lifecycle events – AWS OpsWorks supports continuous 
configuration through lifecycle events that automatically update your instances’ 
configuration to adapt to environment changes.
• AWS Lambda Scheduled events – These events allow you to create a Lambda 
function and direct AWS Lambda to execute it on a regular schedule.

### LOOSE COUPLING
As application complexity increases, a desirable attribute of an IT system is that it can be 
broken into smaller, loosely coupled components.
This means that IT systems should be designed in a way that reduces interdependencies—a 
change or a failure in one component should not cascade to other components.
Design principles include:
• Well-defined interfaces – reduce interdependencies in a system by enabling 
interaction only through specific, technology-agnostic interfaces (e.g. RESTful 
APIs).
• Service discovery – disparate resources must have a way of discovering each other 
without prior knowledge of the network topology.
• Asynchronous integration – this is another form of loose coupling where an 
interaction does not need an immediate response (think SQS queue or Kinesis).
• Graceful failure – build applications such that they handle failure in a graceful 
manner (reduce the impact of failure and implement retries).

### SERVICES, NOT SERVERS
With traditional IT infrastructure, organizations must build and operate a wide variety of 
technology components.
AWS offers a broad set of compute, storage, database, analytics, application, and 
deployment services that help organizations move faster and lower IT costs.
Managed services:
• On AWS, there is a set of services that provide building blocks that developers can 
consume to power their applications.
• These managed services include databases, machine learning, analytics, queuing, 
search, email, notifications, and more.
Serverless architectures:
• Another approach that can reduce the operational complexity of running 
applications is that of the serverless architectures.
• It is possible to build both event-driven and synchronous services for mobile, web, 
analytics, and the Internet of Things (IoT) without managing any server 
infrastructure.

### DATABASES
With traditional IT infrastructure, organizations were often limited to the database and 
storage technologies they could use.
With AWS, these constraints are removed by managed database services that offer 
enterprise performance at open-source cost.
#### RELATIONAL DATABASES
Relational databases (often called RDBS or SQL databases) normalize data into well-defined 
tabular structures known as tables, which consist of rows and columns.
They provide a powerful query language, flexible indexing capabilities, strong integrity 
controls, and the ability to combine data from multiple tables in a fast and efficient 
manner.
Amazon RDS is a relational database service.
Scalability:
• Relational databases can scale vertically (e.g. upgrading to a larger RDS DB 
instance).
• For read-heavy use cases, you can scale horizontally using read replicas.
• For scaling write capacity beyond a single instance data partitioning or sharding is 
required.
High Availability:
• For production DBs, Amazon recommend the use of RDS Multi-AZ which creates a 
synchronously replicated standby in another AZ.
• With Multi-AZ RDS can failover to the standby node without administrative 
intervention.
Anti-Patterns:
• If your application primarily indexes and queries data with no need for joins or 
complex transactions, consider a NoSQL database instead.
• If you have large binary files (audio, video, and image), it will be more efficient to 
store the actual files in S3 and only hold the metadata for the files in your 
database.

#### NOSQL DATABASES
NoSQL is a term used to describe databases that trade some of the query and transaction 
capabilities of relational databases for a more flexible data model that seamlessly scales 
horizontally.
NoSQL databases utilize a variety of data models, including graphs, key-value pairs, and 
JSON documents.
DynamoDB is Amazon’s NoSQL database service.
Scalability:
• NoSQL database engines will typically perform data partitioning and replication to 
scale both the reads and the writes in a horizontal fashion.
High Availability:
• DynamoDB synchronously replicates data across three facilities in an AWS region 
for fault tolerance.
Anti-Patterns:
• If your schema cannot be denormalized and your application requires joins or 
complex transactions, consider a relational database instead.
• If you have large binary files (audio, video, and image), consider storing the files in 
Amazon S3 and storing the metadata for the files in your database.

#### DATA WAREHOUSE
A data warehouse is a specialized type of relational database, optimized for analysis and 
reporting of large amounts of data.
It can be used to combine transactional data from disparate sources making them available
for analysis and decision-making.
Amazon Redshift is a managed data warehouse service that is designed to operate at less 
than a tenth the cost of traditional solutions.
Scalability:
• Amazon Redshift achieves efficient storage and optimum query performance 
through a combination of massively parallel processing (MPP), columnar data 
storage, and targeted data compression encoding schemes.
• RedShift is particularly suited to analytic and reporting workloads against very 
large data sets.
High Availability:
• Redshift has multiple features that enhance the reliability of your data warehouse 
cluster.
• Multi-node clusters replicate data to other nodes within the cluster.
• Data is continuously backed up to S3.
• RedShift continuously monitors the health of the cluster and re-replicates data 
from failed drives and replaces nodes as necessary.
Anti-Patterns:
• Because Amazon Redshift is a SQL-based relational database management system 
(RDBMS), it is compatible with other RDBMS applications and business intelligence 
tools.
• Although Amazon Redshift provides the functionality of a typical RDBMS, including 
online transaction processing (OLTP) functions, it is not designed for these 
workloads.
SEARCH
Applications that require sophisticated search functionality will typically outgrow the 
capabilities of relational or NoSQL databases.
A search service can be used to index and search both structured and free text format and 
can support functionality that is not available in other databases, such as customizable 
result ranking, faceting for filtering, synonyms, stemming, etc.
Scalability:
• Both Amazon CloudSearch and Amazon ES use data partitioning and replication to 
scale horizontally.
High Availability:
• Both services provide features that store data redundantly across Availability 
Zones.

#### REMOVING SINGLE POINTS OF FAILURE
A system is highly available when it can withstand the failure of an individual or multiple 
components.
Automate recovery and reduce disruption at every layer of your architecture.
##### INTRODUCING REDUNDANCY
Single points of failure can be removed by introducing redundancy.
In standby redundancy when a resource fails, functionality is recovered on a secondary 
resource using a process called failover, which typically take some time to complete.
In active redundancy, requests are distributed to multiple redundant compute resources, 
and when one of them fails, the rest can simply absorb a larger share of the workload.
##### DETECT FAILURE
Build as much automation as possible in both detecting and reacting to failure.
Services like ELB and Route53 mask failure by routing traffic to healthy endpoint.
Auto Scaling can be configured to automatically replace unhealthy nodes.
You can also replace unhealthy nodes using the EC2 auto- recovery, OpsWorks and Elastic 
Beanstalk.
##### DURABLE DATA STORAGE
Design your architecture to protect both data availability and integrity.
Data replication is the technique that introduces redundant copies of data.
It can help horizontally scale read capacity, but it also increases data durability and 
availability.
Replication can take place in a few different modes:
• Synchronous replication – transactions are acknowledged only after data has been 
durably stored in both the primary and replica instance. Can be used to protect 
data integrity (low RPO) and scaling read capacity (with strong consistency).
• Asynchronous replication – changes on the primary node are not immediately 
reflected on its replicas. Can be used to horizontally scale the system’s read 
capacity (with replication lag), and data durability (with some data loss).
• Quorum-based replication – combines synchronous and asynchronous replication 
and is good for large-scale distributed database systems.
##### AUTOMATED MULTI-DATA CENTER RESILIENCE
With traditional infrastructure, failing over between data centers is performed using a 
disaster recovery plan.
Long distances between data centers mean that latency makes synchronous replication 
impractical.
Failovers often lead to data loss and costly data recovery processes.
On AWS it is possible to adopt a simpler, more efficient protection from this type of failure.
Each AWS region contains multiple distinct locations called Availability Zones (AZs).
Each AZ is engineered to be isolated from failures in other AZs.
An AZ is a data center, and in some cases, an AZ consists of multiple data centers.
AZs within a region provide inexpensive, low-latency network connectivity to other zones
in the same region.
This allows you to replicate your data across data centers in a synchronous manner so that 
failover can be automated and be transparent for your users.
FAULT ISOLATION AND TRADITIONAL HORIZONTAL SCALING
Though the active redundancy pattern is great for balancing traffic and handling instance 
or Availability Zone disruptions, it is not sufficient if there is something harmful about the 
requests themselves.
If a particular request happens to trigger a bug that causes the system to fail over, then the 
caller may trigger a cascading failure by repeatedly trying the same request against all 
instances.
One fault-isolating improvement you can make to traditional horizontal scaling is called 
sharding.
Like the technique traditionally used with data storage systems, instead of spreading traffic 
from all customers across every node, you can group the instances into shards.
In this way, you can reduce the impact on customers in direct proportion to the number of 
shards you have.
##### OPTIMIZE FOR COST
Just by moving existing architectures into the cloud, organizations can reduce capital 
expenses and drive savings because of the AWS economies of scale.
By iterating and making use of more AWS capabilities there is further opportunity to create 
cost-optimized cloud architectures.
Right Sizing:
• In some cases, you should select the cheapest type that suits your workload’s 
requirements.
• In other cases, using fewer instances of a larger instance type might result in lower 
total cost or better performance.
• Benchmark and select the right instance type depending on how your workload 
utilizes CPU, RAM, network, storage size, and I/O.
• Reduce cost by selecting the right storage solution for your needs.
• E.g. S3 offers a variety of storage classes, including Standard, Reduced 
Redundancy, and Standard-Infrequent Access.
• EC2, RDS, and ES support different EBS volume types (magnetic, general-purpose 
SSD, provisioned IOPS SSD) that you should evaluate.
Elasticity:
• Plan to implement Auto Scaling for as many EC2 workloads as possible, so that you 
horizontally scale up when needed and scale down automatically to reduce cost.
• Automate turning off non-production workloads when not in use.
• Where possible, replace EC2 workloads with AWS managed services that don’t 
require you to take any capacity decisions. For example:
o ELB
o CloudFront.
o SQS.
o Kinesis Firehose.
o Lambda.
o SES.
o CloudSearch.
• Or use services for which you can modify capacity as and when need. For example:
o DynamoDB.
o RDS.
o Elasticsearch Service.
Take Advantage of the Variety of Purchasing Options:
• EC2 On-Demand instance pricing gives you maximum flexibility with no long-term 
commitments.
• There are two more ways to pay for Amazon EC2 instances that can help you 
reduce spend: Reserved Instances and Spot Instances.
### RESERVED CAPACITY
EC2 Reserved Instances allow you to reserve Amazon EC2 computing capacity in exchange 
for a significantly discounted hourly rate compared to On- Demand instance pricing.
This is ideal for applications with predictable minimum capacity requirements.
SPOT INSTANCES
For less steady workloads, you can consider the use of Spot Instances.
EC2 Spot Instances allow you to bid on spareEC2 computing capacity.
Since Spot Instances are often available at a discount compared to On-Demand pricing, you 
can significantly reduce the cost of running your applications.
Spot Instances are ideal for workloads that have flexible start and end times.
If the Spot market price increases above your bid price, your instance will be terminated 
automatically, and you will not be charged for the partial hour that your instance has run.
As a result, Spot Instances are great for workloads that have tolerance to interruption.
### CACHING
Caching is a technique that stores previously calculated data for future use.
This technique is used to improve application performance and increase the cost efficiency 
of an implementation.
It can be applied at multiple layers of an IT architecture.
APPLICATION DATA CACHING
Applications can be designed so that they store and retrieve information from fast, 
managed, in-memory caches.
Cached information may include the results of I/O-intensive database queries or the
outcome of computationally intensive processing.
#### EDGE CACHING
Copies of static content and dynamic content can be cached at Amazon CloudFront, which 
is a content delivery network (CDN) consisting of multiple edge locations around the world.
Edge caching allows content to be served by infrastructure that is closer to viewers, 
lowering latency and giving you the high, sustained data transfer rates needed to deliver 
large popular objects to end users at scale.
#### SECURITY
Most of the security tools and techniques that you might already be familiar with in a 
traditional IT infrastructure can be used in the cloud.
At the same time, AWS allows you to improve your security in a variety of ways.
AWS is a platform that allows you to formalize the design of security controls in the 
platform itself.
#### UTILIZE AWS FEATURES FOR DEFENSE IN DEPTH
Network level security includes building a VPC topology that isolates parts of the 
infrastructure using subnets, security groups, and routing controls.
Services like AWS WAF, a web application firewall, can help protect web applications from 
SQL injection and other vulnerabilities in application code.
For access control, you can use IAM to define a granular set of policies and assign them to 
users, groups, and AWS resources.
Finally, the AWS platform offers a breadth of options for protecting data, whether it is in 
transit or at rest with encryption.
#### OFFLOAD SECURITY RESPONSIBILITY TO AWS
AWS operates under a shared security responsibility model, where AWS is responsible for 
the security of the underlying cloud infrastructure, and you are responsible for securing 
the workloads you deploy in AWS.
#### REDUCE PRIVILEGED ACCESS
When you treat servers as programmable resources, you can capitalize on that for benefits 
in the security space as well.
Eliminate the need for guest operating system access to production environments.
If an instance experiences an issue, you can automatically or manually terminate and 
replace it.
In a traditional environment, service accounts would often be assigned long-term 
credentials stored in a configuration file.
On AWS, you can instead use IAM roles to grant permissions to applications running on 
Amazon EC2 instances using short-term credentials.
#### SECURITY AS CODE
Traditional security frameworks, regulations, and organizational policies define security 
requirements related to things such as firewall rules, network access controls, 
internal/external subnets, and operating system hardening.
You can implement these in an AWS environment as well, but you now can capture them 
all in a script that defines a “Golden Environment.”
This means you can create an AWS CloudFormation script that captures your security 
policy and reliably deploys it.
Security best practices can now be reused among multiple projects and become part of 
your continuous integration pipeline.
You can perform security testing as part of your release cycle, and automatically discover 
application gaps and drift from your security policy.
#### REAL-TIME AUDITING
Testing and auditing your environment is key to moving fast while staying safe.
Traditional approaches that involve periodic checks are not sufficient, especially in agile 
environments where change is constant.
On AWS, it is possible to implement continuous monitoring and automation of controls to 
minimize exposure to security risks.
Services like AWS Config, Amazon Inspector, and AWS Trusted Advisor continually monitor 
for compliance or vulnerabilities.
With AWS Config rules you will also know if some component was out of compliance even 
for a brief period.
You can implement extensive logging for your applications (using Amazon CloudWatch 
Logs) and for the actual AWS API calls by enabling AWS CloudTrail.
Logs can then be stored in an immutable manner and automatically processed to either 
notify or even act on your behalf, protecting your organization from non-compliance.
You can use AWS Lambda, Amazon EMR, the Amazon Elasticsearch Service, or third- party 
tools from the AWS Marketplace to scan logs to detect things like unused permissions, 
overuse of privileged accounts, usage of keys, anomalous logins, policy violations, and 
system abuse.

## ARCHITECTING FOR THE CLOUD QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: Which architectural benefit of the AWS Cloud assists with lowering 
operational cost?
1. Higher-level managed services
2. Horizontal scaling
3. Loose coupling
4. Design for failure

Question 2: AWS EC2 Auto Scaling provides which type of scaling?
1. Horizontal
2. Vertical

Question 3: Which type of scaling does an Amazon Read Replica provide?
1. Horizontal
2. Vertical

Question 4: Which of the following is a benefit of API-driven services?
1. You can programmatically and dynamically launch resources
2. You can define services through the AWS management console
3. You get greater fault tolerance
4. Increased reliability

Question 5: Which of the following is an architectural best practice?
1. Design for the future
2. Design monolithic applications
3. Design for failure 
4. Use close coupling

Question 6: The best practice "services, not servers" means what?
1. You should try to use more services such as managed services and serverless 
services
2. You should not use servers such as Amazon EC2
3. Try to only use serverless services

Question 7: How does DynamoDB scale?
1. Vertically 
2. Horizontally
3. Both vertically and horizontally

Question 8: Which architectural best practice aims to reduce interdependencies between 
application components?
1. Automation
2. Services, Not Servers
3. Removing Single Points of Failure
4. Loose Coupling

Question 9: Which of the following is NOT a limitation of scaling vertically?
1. Can reach a limit of maximum instance size
2. Often requires manual intervention
3. Requires a load balancer for distributing load
4. Typically requires downtime

Question 10: Which services can scale horizontally?
1. Amazon DynamoDB, Amazon EC2 Auto Scaling, Amazon S3
2. Amazon DynamoDB, Amazon EFS, Amazon EC2
3. Amazon EC2 Auto Scaling, Amazon S3, NAT Instance

Question 11: If using a well written templates, how can Amazon CloudFormation assist 
with building secure environments?
1. It does not require privileged access
2. It ensures consistent builds when building repeatably
3. The responsibility is shared with AWS






