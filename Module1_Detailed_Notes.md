### DOMAINS, OBJECTIVES AND EXAMPLES

The required knowledge is organized into four test “domains”. Within each test domain
there are several objectives that broadly describe the required knowledge and experience
to successfully pass the exam.

### Test Domain 1: Cloud Concepts

This domain makes up 24% of the exam and includes the following objectives:
• Define the benefits of the AWS Cloud
• Identify design principles of the AWS Cloud
• Understand the benefits of and strategies for migration to the AWS Cloud
• Understand the concepts of cloud economics

## What you need to know
You should be able to describe the benefits of public cloud services and define the types of
services available on AWS (such as IaaS, PaaS, SaaS). Make sure you understand the 6
advantages of cloud:
1. Trade capital expense for variable expense
2. Benefit from massive economies of scale
3. Stop guessing about capacity
4. Increase speed and agility
5. Stop spending money running and maintaining data centers
6. Go global in minutes
   
You need to understand how cloud is beneficial from a financial perspective and be familiar 
with the difference between CAPEX and OPEX, which relates to item 1 in the list above.
Additionally, you need to understand the design principles of creating cloud architectures. 
This includes concepts such as loose coupling, scaling (vertically and horizontally),
bootstrapping and automation, among others.

## Example questions
Question: Which feature of AWS allows you to deploy a new application for which the
requirements may change over time?
1. Elasticity
2. Fault tolerance
3. Disposable resources
4. High availability
   
Answer: 1. Elasticity allows you to deploy your application without worrying about
whether it will need more or less resources in the future. With elasticity, the infrastructure
can scale on-demand to meet the changing requirements

Question: What advantages do you get from using the AWS cloud? (choose 2)
1. Trade capital expense for variable expense
2. Stop guessing about capacity
3. Increased capital expenditure
4. Gain greater control of the infrastructure layer
5. Comply with all local security compliance programs
   
Answer: 1+2. With public cloud services such as AWS, you can pay on a variable (OPEX)
basis for the resources you use and scale on-demand, eliminating the need to guess how
much resources you need to deploy.

### Test Domain 2: Security & Compliance
This domain makes up 30% of the exam and includes the following objectives:
• Understand the AWS shared responsibility model
• Understand AWS Cloud security, governance, and compliance concepts
• Identify AWS access management capabilities
• Identify components and resources for security
What you need to know
You should understand the AWS shared responsibility model, which defines who is
responsible for different aspects of the technology stack, from the data center through to
servers, firewall rules, and data encryption.

AWS provide tools and services for implementing security, assessing your security position,
and generating alerts and compliance reports. You need to understand these services and
tools well enough to describe their usage and benefits. This includes services such as KMS,
CloudTrail, and AWS Artifact.

You also need to understand the services that are used for authentication, authorization
and access management. This includes services such as AWS IAM, and Amazon Cognito,
and the usage of access keys, key pairs and signed URLs.
Support services include real-time insights through AWS Trusted Advisor and proactive
support and advocacy through a Technical Account Manager (TAM). Make sure you know
which support packages include a TAM.

#### Example questions
Question: Under the AWS shared responsibility model what is the customer responsible
for? (choose 2)
1. Physical security of the data center
2. Replacement and disposal of disk drives
3. Configuration of security groups
4. Patch management of infrastructure
5. Encryption of customer data
   
Answer: 3+5. AWS are responsible for items such as the physical security of the data center, replacement of old disk drives, and patch management of the infrastructure
whereas customers are responsible for items such as configuring security groups, network
ACLs, patching their operating systems and encrypting their data.

Question: Which AWS service is used to enable multi-factor authentication?
1. Amazon STS
2. AWS IAM
3. Amazon EC2
4. AWS KMS
   
Answer: 2. AWS IAM (Identity and Access Management) is used to securely control
individual and group access to AWS resources and can be used to manage multi-factor
authentication (MFA).

### Test Domain 3: Cloud Technology and Services
This domain makes up 34% of the exam and includes the following objectives:
• Define methods of deploying and operating in the AWS Cloud
• Define the AWS global infrastructure
• Identify AWS compute services
• Identify AWS database services
• Identify AWS network services
• Identify AWS storage services
• Identify AWS artificial intelligence and machine learning (AI/ML) services and 
analytics services
• Identify services from other in-scope AWS service categories
What you need to know
You need to understand the core AWS services and what they are used for. While you
don’t need an in-depth level of knowledge of the specifics of each service, it’s important to
understand their purpose, benefits and use cases.
Core services include EC2, ECS, Lambda, LightSail, EBS, EFS, S3, RDS, DynamoDB, RedShift,
ElastiCache, Elastic Load Balancing, Auto Scaling, CloudFront, Route 53, CloudWatch,
CloudTrail, and SNS.
You should also understand the underlying global infrastructure that makes up the AWS
Cloud. This includes regions, availability zones, and edge locations. Make sure you
understand which services are globally or regionally defined.
Additionally, you need to know the customer configurable building blocks of cloud services
including VPCs, and subnets, and connectivity options such as Internet Gateways, VPN and
Direct Connect. Make sure you know the difference between NAT Instances and NAT
Gateways and the relative benefits of each service.

### Example questions
Question: What are the advantages of Availability Zones? (choose 2)
1. They allow regional disaster recovery
2. They provide fault isolation
3. They enable the caching of data for faster delivery to end users
4. They are connected by low-latency network connections
5. They enable you to connect your on-premises networks to AWS to form a hybrid
cloud

Answer: 2+4. Each AWS region contains multiple distinct locations known as Availability
Zones (AZs). Each AZ is engineered to be isolated from failures in other AZs. An AZ is a data
center, and in some cases, an AZ consists of multiple data centers. AZs within a region
provide inexpensive, low-latency network connectivity to other zones in the same region.
This allows you to replicate your data across data centers in a synchronous manner so that
failover can be automated and be transparent for your users.
Question: Which AWS support plans provide support via email, chat and phone? (choose 2)
1. Basic
2. Business
3. Developer
4. Global
5. Enterprise
   
Answer: 2+5. Only the business and enterprise plans provide support via email, chat and
phone.

### Test Domain 4: Billing, Pricing and Support
This domain makes up 12% of the exam and includes the following objectives:
• Compare AWS pricing models
• Understand resources for billing, budget, and cost management
• Identify AWS technical resources and AWS Support options
What you need to know
Most services on AWS are offered on a pay-per-use basis, but there are also options to
reduce costs by committing to 1- or 3-year contracts with various payment options. You
need to understand these pricing models and which services they apply to.
Make sure you understand what AWS charges you for and what is free of charge. For
instance, inbound data transfer is free whereas outbound data transfer typically incurs
costs.
Some services such as VPC, CloudFormation, and IAM are free, but the resources you
create with them may not be. You need to understand where costs may be incurred.
AWS accounts can be organized into Organizations for centralized management of policies
and consolidated billing. You need to understand the various accounts structures and the
benefits and use cases for implementing them.
For instance, you might want separate account structures to manage different policies for
production and non-production resources, or you might implement consolidated billing to
take advantage of volume discounts.
you should be familiar with the services and tools available, as well as the support levels 
offered through AWS support plans. 
Tools include AWS Cost Explorer, AWS Simple Monthly Calculator, and Total Cost of
Ownership (TCO) calculator.

### Example questions
Question: What are two ways an AWS customer can reduce their monthly spend? (choose
2)
1. Turn off resources that are not being used
2. Use more power efficient instance types
3. Reserve capacity where suitable
4. Be efficient with usage of Security Groups
5. Reduce the amount of data ingress charges
   
Answer: 1+3. Turning off resources that are not used can reduce spend. You can also use
reserved instances to reduce the monthly spend at the expense of having to lock into a 1
or 3-year contract – which is good for stable workloads.
Question: A company would like to maximize their potential volume and Reserved Instance 
(RI) discounts across multiple accounts and also apply service control policies to member
accounts. What can they use to gain these benefits?
1. AWS Budgets
2. AWS Cost Explorer
3. AWS IAM
4. AWS Organizations
   
Answer: 4. AWS Organizations enables you to create groups of AWS accounts and centrally 
manage policies across those accounts. AWS Organizations provides consolidated billing in 
both feature sets, enabling you to set up a single payment method in the organization’s 
master account while still receiving an invoice for individual activity in each member 
account. Volume pricing discounts can be applied to resources.






