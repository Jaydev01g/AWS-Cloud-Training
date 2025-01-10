# AUTO SCALING AND ELASTIC LOAD BALANCING

Auto Scaling and Elastic Load Balancing are features of AWS that you can use separately or 
together for elasticity and high availability.

## AMAZON EC2 AUTO SCALING
Amazon EC2 Auto Scaling automates the process of launching (scaling out) and terminating 
(scaling in) Amazon EC2 instances based on the traffic demand for your application.
Auto Scaling helps to ensure that you have the correct number of EC2 instances available 
to handle the application load.
Amazon EC2 Auto Scaling provides elasticity and scalability.
You create collections of EC2 instances, called an Auto Scaling group (ASG).
You can specify the minimum number of instances in each ASG, and AWS Auto Scaling will 
ensure the group never goes beneath this size.
You can also specify the maximum number of instances in each ASG, and the group will 
never go above this size.
A desired capacity can be configured, and AWS Auto Scaling will ensure the group has this 
number of instances.
You can also specify scaling policies that control when Auto Scaling launches or terminates 
instances.
Scaling policies determine when, if, and how the ASG scales and shrinks (ondemand/dynamic scaling, cyclic/scheduled scaling).
Scaling Plans define the triggers and when instances should be provisioned/de-provisioned.
A launch configuration is the template used to create new EC2 instances and includes parameters such as instance family, instance type, AMI, key pair, and security groups.

## AMAZON ELASTIC LOAD BALANCING (ELB)
ELB automatically distributes incoming application traffic across multiple targets, such as 
Amazon EC2 instances, containers, and IP addresses.
ELB can handle the varying load of your application traffic in a single Availability Zone or 
across multiple Availability Zones.
ELB features high availability, automatic scaling, and robust security necessary to make 
your applications fault tolerant.
There are four types of Elastic Load Balancer (ELB) on AWS:
• Application Load Balancer (ALB) – layer 7 load balancer that routes connections 
based on the content of the request.
• Network Load Balancer (NLB) – layer 4 load balancer that routes connections 
based on IP protocol data.
• Classic Load Balancer (CLB) – this is the oldest of the three and provides basic load 
balancing at both layer 4 and layer 7 (not on the exam anymore).
• Gateway Load Balancer (GLB) – distributes connections to virtual appliances and 
scales them up or down (not on the exam).
APPLICATION LOAD BALANCER (ALB)
ALB is best suited for load balancing of HTTP and HTTPS traffic and provides advanced 
request routing targeted at the delivery of modern application architectures, including 
microservices and containers.
Operating at the individual request level (Layer 7), Application Load Balancer routes traffic 
to targets within Amazon Virtual Private Cloud (Amazon VPC) based on the content of the 
request.

### NETWORK LOAD BALANCER (NLB)
NLB is best suited for load balancing of TCP traffic where extreme performance is required.
Operating at the connection level (Layer 4), Network Load Balancer routes traffic to targets 
within Amazon Virtual Private Cloud (Amazon VPC) and is capable of handling millions of 
requests per second while maintaining ultra-low latencies.
Network Load Balancer is also optimized to handle sudden and volatile traffic patterns.

### AUTO SCALING AND ELASTIC LOAD BALANCING QUIZ QUESTIONS

Answers and explanations are provided below after the last question in this section.

Question 1: How can a company enable elasticity for an application running on Amazon EC2?
1. By using Amazon EC2 Auto Scaling
2. By using Elastic Load Balancing
3. By configuring multi-AZ
4. By enabling failover in Amazon EC2

Question 2: Which type of Elastic Load Balancer can direct traffic based on the domain name?
1. Classic Load Balancer
2. Network Load Balancer
3. Application Load Balancer
4. Amazon EC2 Load Balancer

Question 3: How does Amazon EC2 Auto Scaling assist with cost-effectiveness?
1. By choosing the most cost-effective instance type
2. By balancing load between instances evenly
3. By launching and terminating instances as demand changes
4. By automating application failover

Question 4: How does Elastic Load Balancing (ELB) assist with fault tolerance?
1. By distributing connections to multiple back-end instances
2. By directing traffic according to latency
3. By caching content closer to users
4. By automatically launching instances

Question 5: Which of the following statements is INCORRECT about Elastic Load 
Balancing?
1. ELB can distribute connections across availability zones
2. ELB can be Internet facing
3. ELB enables high availability and fault tolerance
4. ELB can distribute connections across regions

Question 6: What does Elastic Load Balancing use to ensure instances are available?
1. EC2 Status Checks
2. CloudWatch Metrics
3. Scaling Plans
4. Health Checks

Question 7: Which type of Elastic Load Balancer routes connections based on IP protocol 
data at layer 4 only?
1. Classic Load Balancer
2. Network Load Balancer
3. Application Load Balancer

Question 8: What type of template is used by Amazon EC2 Auto Scaling to define 
instance family, AMI key pair, and security groups?
1. Scaling Plan
2. Launch Configuration
3. Scaling Policy
4. Auto Scaling Group


# CONTENT DELIVERY AND DNS SERVICES
This category of AWS services includes services for caching content around the world and 
providing intelligent Domain Name System (DNS) services for your applications.
## AMAZON ROUTE 53
Amazon Route 53 is the AWS Domain Name Service.
Route 53 performs three main functions:
• Domain registration – Route 53 allows you to register domain names.
• Domain Name Service (DNS) – Route 53 translates name to IP addresses using a 
global network of authoritative DNS servers.
• Health checking – Route 53 sends automated requests to your application to verify 
that it’s reachable, available, and functional.
You can use any combination of these functions.
Route 53 benefits:
• Domain registration.
• DNS service.
• Traffic Flow (send users to the best endpoint).
• Health checking.
• DNS failover (automatically change domain endpoint if system fails).
• Integrates with ELB, S3, and CloudFront as endpoints.
Routing policies determine how Route 53 DNS responds to queries.
The following table highlights the key function of each type of routing policy:
Policy What it Does
Simple Simple DNS response providing the IP address associated with a 
name
Failover If primary is down (based on health checks), routes to 
secondary destination
Geolocation Uses geographic location you’re in (e.g. Europe) to route you to 
the closest region
Geoproximity Routes you to the closest region within a geographic area
Latency Directs you based on the lowest latency route to resources
Multivalue answer Returns several IP addresses and functions as a basic load 
balancer
Weighted Uses the relative weights assigned to resources to determine 
which to route to

## AMAZON CLOUDFRONT
Amazon CloudFront is a content delivery network (CDN) that allows you to store (cache) 
your content at “edge locations” located around the world.
This allows customers to access content more quickly and provides security against DDoS 
attacks.
CloudFront can be used for data, videos, applications, and APIs.
CloudFront benefits:
• Cache content at Edge Location for fast distribution to customers.
• Built-in Distributed Denial of Service (DDoS) attack protection.
• Integrates with many AWS services (S3, EC2, ELB, Route 53, Lambda).
Origins and Distributions:
• An origin is the origin of the files that the CDN will distribute.
• Origins can be either an S3 bucket, an EC2 instance, an Elastic Load Balancer, or 
Route 53 – can also be external (non-AWS).
• To distribute content with CloudFront you need to create a distribution.
• There are two types of distribution: Web Distribution and RTMP Distribution.
CloudFront uses Edge Locations and Regional Edge Caches:
• An edge location is the location where content is cached (separate to AWS 
regions/AZs).
• Requests are automatically routed to the nearest edge location.
• Regional Edge Caches are located between origin web servers and global edge 
locations and have a larger cache.
• Regional Edge caches aim to get content closer to users.

## CONTENT DELIVERY AND DNS SERVICES QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: Which services does Amazon Route 53 provide?
1. Domain registration, DNS, firewall protection
2. Health checking, DNS, domain registration
3. Health checking, DNS, IP routing
4. Domain registration, DNS, content distribution

Question 2: In Amazon Route 53, what is the name for the configuration item that holds 
a collection of records belonging to a domain?
1. DNS record
2. Alias
3. Hosted zone
4. Routing Policy
   
Question 3: How can an organization improve performance for users around the world 
accessing online videos?
1. Use Amazon Route 53 Failover routing
2. Create an Amazon CloudFront Distribution to host the videos
3. Use Amazon S3 cross-region replication to distribute the media around the world
4. Use Amazon S3 Transfer acceleration to speed up downloads
   
Question 4: Which services have a Global scope?
1. Amazon CloudFront, Amazon Route 53, Amazon VPC
2. 2. Amazon CloudFront, Amazon Route 53, Amazon CloudWatch
3. AWS Lambda, Amazon CloudFront, Amazon Route 53
4. AWS IAM, Amazon CloudFront, Amazon Route 53
   
Question 5: Which service has built-in Distributed Denial of Service (DDoS) protection?
1. Amazon Route 53
2. Internet Gateway
3. Amazon CloudFront
4. AWS Direct Connect
   
Question 6: Which of the following is used to cache data to bring it closer to end users?
1. Amazon CloudFront Edge Location
2. Amazon CloudFront Distribution
3. Amazon CloudFront Origin
4. Amazon CloudFront Bucket
   
Question 7: Which types of Origin does Amazon CloudFront support?
1. S3 bucket, EC2 instance
2. S3 bucket, RDS database
3. EC2 instance, EFS filesystem
4. EC2 instance, Auto Scaling Group
   
Question 8: In Amazon Route 53, what is the name for the configuration item that holds 
a collection of records belonging to a domain?
1. DNS record
2. Alias
3. Hosted zone
4. Routing Policy


   
# MONITORING AND LOGGING SERVICES
This category of AWS services includes services that provide logging, monitoring, and 
auditing for your applications running on AWS.

## AMAZON CLOUDWATCH
Amazon CloudWatch is a monitoring service for AWS cloud resources and the applications 
you run on AWS.CloudWatch is for performance monitoring (CloudTrail is for auditing).Used to collect and track metrics, collect, and monitor log files, and set alarms.
Automatically react to changes in your AWS resources.

Monitor resources such as:
• EC2 instances.
• DynamoDB tables.
• RDS DB instances.
• Custom metrics generated by applications and services.
• Any log files generated by your applications.

Gain system-wide visibility into resource utilization.
CloudWatch monitoring includes application performance.
Monitor operational health.
CloudWatch is accessed via API, command-line interface, AWS SDKs, and the AWS Management Console.
CloudWatch integrates with IAM.
Amazon CloudWatch Logs lets you monitor and troubleshoot your systems and applications using your existing system, application, and custom log files.
CloudWatch Logs can be used for real time application and system monitoring as well as long term log retention.
CloudWatch Logs keeps logs indefinitely by default.
CloudTrail logs can be sent to CloudWatch Logs for real-time monitoring.
CloudWatch Logs metric filters can evaluate CloudTrail logs for specific terms, phrases, or values.

CloudWatch retains metric data as follows:
• Data points with a period of less than 60 seconds are available for 3 hours. These 
data points are high-resolution custom metrics.
• Data points with a period of 60 seconds (1 minute) are available for 15 days.
• Data points with a period of 300 seconds (5 minute) are available for 63 days.
• Data points with a period of 3600 seconds (1 hour) are available for 455 days (15 
months).
Dashboards allow you to create, customize, interact with, and save graphs of AWS resources and custom metrics.
Alarms can be used to monitor any Amazon CloudWatch metric in your account.
Events are a stream of system events describing changes in your AWS resources.
Logs help you to aggregate, monitor and store logs.
Basic monitoring = 5 mins (free for EC2 Instances, EBS volumes, ELBs and RDS DBs).
Detailed monitoring = 1 min (chargeable).
Metrics are provided automatically for several AWS products and services.
There is no standard metric for memory usage on EC2 instances.
A custom metric is any metric you provide to Amazon CloudWatch (e.g. time to load a web 
page or application performance).
Options for storing logs:
• CloudWatch Logs.
• Centralized logging system (e.g. Splunk).
• Custom script and store on S3.

Do not store logs on non-persistent disks:
Best practice is to store logs in CloudWatch Logs or S3.
CloudWatch Logs subscription can be used across multiple AWS accounts (using cross account access).
Amazon CloudWatch uses Amazon SNS to send email.

# AWS CLOUDTRAIL
AWS CloudTrail is a web service that records activity made on your account and delivers 
log files to an Amazon S3 bucket.
CloudTrail is for auditing (CloudWatch is for performance monitoring).
CloudTrail is about logging and saves a history of API calls for your AWS account.
Provides visibility into user activity by recording actions taken on your account.
API history enables security analysis, resource change tracking, and compliance auditing.
Logs API calls made via:
• AWS Management Console.
• AWS SDKs.
• Command line tools.
• Higher-level AWS services (such as CloudFormation).
CloudTrail records account activity and service events from most AWS services and logs the 
following records:
• The identity of the API caller.
• The time of the API call.
• The source IP address of the API caller.
• The request parameters.
103 © 2025 Digital Cloud Training
• The response elements returned by the AWS service.
CloudTrail is enabled by default.
CloudTrail is per AWS account.
You can consolidate logs from multiple accounts using an S3 bucket:
1. Turn on CloudTrail in the paying account.
2. Create a bucket policy that allows cross-account access.
3. Turn on CloudTrail in the other accounts and use the bucket in the paying account.
You can integrate CloudTrail with CloudWatch Logs to deliver data events captured by 
CloudTrail to a CloudWatch Logs log stream.
CloudTrail log file integrity validation feature allows you to determine whether a CloudTrail 
log file was unchanged, deleted, or modified since CloudTrail delivered it to the specified 
Amazon S3 bucket.

### MONITORING AND LOGGING SERVICES QUIZ QUESTIONS

Answers and explanations are provided below after the last question in this section.
Question 1: Which service can be used to record information about API activity in your 
AWS account?
1. Amazon CloudWatch
2. Amazon CloudTrail

Question 2: Which service can be used for alerting if the CPU is heavily loaded on an EC2 
instance?
1. Amazon CloudWatch
2. Amazon CloudTrail

Question 3: Does Amazon CloudTrail permanently record all API activity in your account 
by default?
1. Yes
2. No



# AWS BILLING AND PRICING
AWS Billing and Pricing is one of the key subjects on the AWS Certified Cloud Practitioner exam.
AWS works on a pay as you go model in which you only pay for what you use, when you are using it.
If you turn off resources, you don’t pay for them (you may pay for consumed storage).There are no upfront charges, and you stop paying for a service when you stop using it.Aside from EC2 reserved instances you are not locked into long term contracts and can terminate whenever you choose to.Volume discounts are available so the more you use a service the cheaper it gets (per unit used).There are no termination fees.The three fundamental drivers of cost with AWS are: compute, storage, and outbound data transfer.

In most cases, there is no charge for inbound data transfer or for data transfer between other AWS services within the same region (there are some exceptions). Outbound data transfer is aggregated across services and then charged at the outbound data transfer rate.
Free tier allows you to run certain resources for free.
Free tier includes offers that expire after 12 months and offers that never expire.
Pricing policies include:
• Pay as you go.
• Pay less when you reserve.
• Pay even less per unit when using more.
• Pay even less as AWS grows.
• Custom pricing (enterprise customers only).
Free services include:
• Amazon VPC.
• Elastic Beanstalk (but not the resources created).
• CloudFormation (but not the resources created).
• Identity Access Management (IAM).
• Auto Scaling (but not the resources created).
• OpsWorks.
• Consolidated Billing.
Fundamentally charges include:
1. Compute.
2. Storage.
3. Data out.


   
# AMAZON EC2 PRICING
EC2 pricing is based on:
• Clock hours of server uptime.
• Instance configuration.
• Instance type.
• Number of instances.
• Load balancing.
• Detailed monitoring.
• Auto Scaling (resources created).
• Elastic IP addresses (charged if allocated but not used).
• Operating systems and software packages.
There are several pricing models for AWS services, these include:
##### On Demand:
• Means you pay for compute or database capacity with no long-term commitments 
of upfront payments.
• You pay for the computer capacity per hour or per second (Linux only, and applies 
to On-Demand, Reserved and Spot instances).
• Recommended for users who prefer low cost and flexibility without upfront 
payment or long-term commitments.
• Good for applications with short-term, spiky, or unpredictable workloads that 
cannot be interrupted.
##### Dedicated Hosts:
• A dedicated host is an EC2 servers dedicated to a single customer.
• Runs in your VPC.
• Good for when you want to leverage existing server-bound software licenses such 
as Windows Server, SQL Server, and SUSE Linux Enterprise Server.
• Also good for meeting compliance requirements.
##### Dedicated Instances:
• Dedicated Instances are Amazon EC2 instances that run in a VPC on hardware 
that’s dedicated to a single customer.
• Dedicated instances are physically isolated at the host hardware level from 
instances that belong to other AWS accounts.
• Dedicated instances may share hardware with other instances from the same AWS 
account that are not Dedicated instances.
##### Spot Instances:
• Purchase spare computing capacity with no upfront commitment at discounted 
hourly rates.
• Provides up to 90% off the On-Demand price.
• Recommended for applications that have flexible start and end times, applications that are only feasible at very low compute prices, and users with urgent computing needs for a lot of additional capacity.
• In the old model Spot instances were terminated because of higher competing 
bids, in the new model this does not happen, but instances still may be terminated 
(with a 2-minute warning) when EC2 needs the capacity back – note: the exam may 
not be updated to reflect this yet.
##### Savings Plans:
• Commitment to a consistent amount of usage (EC2 + Fargate + Lambda); Pay by 
$/hour; 1 or 3-year commitment.
Reservations:
• Reserved instances provide significant discounts, up to 75% compared to OnDemand pricing, by paying for capacity ahead of time.
• Provide a capacity reservation when applied to a specific Availability Zone.
• Good for applications that have predictable usage, that need reserved capacity, 
and for customers who can commit to a 1 or 3-year term.
Reservations apply to various services, including:
• Amazon EC2 Reserved Instances.
• Amazon DynamoDB Reserved Capacity.
• Amazon ElastiCache Reserved Nodes.
• Amazon RDS Reserved Instances.
• Amazon RedShift Reserved Instances.
Reservation options include no upfront, partial upfront and all upfront.
Reservation terms are 1 or 3 years.


# AMAZON SIMPLE STORAGE SERVICE (S3) PRICING

Storage pricing is determined by:
• Storage class – e.g., Standard or IA.
• Storage quantity – data volume stored in your buckets on a per GB basis.
• Number of requests – the number and type of requests, e.g., GET, PUT, POST, LIST, 
COPY.
• Lifecycle transitions requests – moving data between storage classes.
• Data transfer – data transferred out of an S3 region is charged.
Amazon Glacier pricing
• Extremely low cost and you pay only for what you need with no commitments of 
upfront fees.
• Charged for requests and data transferred out of Glacier.
• “Amazon Glacier Select” pricing allows queries to run directly on data stored on 
Glacier without having to retrieve the archive. Priced on amount of data scanned, 
returned, and number of requests initiated.

## AWS SNOWBALL PRICING
Pay a service fee per data transfer job and the cost of shipping the appliance.
Each job allows use of Snowball appliance for 10 days onsite for free.
Data transfer into AWS is free and outbound is charged (per region pricing).
Amazon Relational Database Service (RDS) Pricing
RDS pricing is determined by:
• Clock hours of server uptime – amount of time the DB instance is running.
• Database characteristics – e.g. database engine, size, and memory class.
• Database purchase type – e.g. On-Demand, Reserved.
• Number of database instances.
• Provisioned storage – backup is included up to 100% of the size of the DB. After 
the DB is terminated backup storage is charged per GB per month.
• Additional storage – the amount of storage in addition to the provisioned storage 
is charged per GB per month.
• Requests – the number of input and output requests to the DB.
• Deployment type – single AZ or multi-AZ.
• Data transfer – inbound is free, outbound data transfer costs are tiered.
• Reserved Instances – RDS RIs can be purchased with No Upfront, Partial Upfront, 
or All Upfront terms. Available for Aurora, MySQL, MariaDB, Oracle and SQL 
Server.

## AMAZON CLOUDFRONT PRICING

CloudFront pricing is determined by:
• Traffic distribution – data transfer and request pricing, varies across regions, and is based on the edge location from which the content is served.
• Requests – the number and type of requests (HTTP or HTTPS) and the geographic 
region in which they are made.
• Data transfer out – quantity of data transferred out of CloudFront edge locations.
• There are additional chargeable items such as invalidation requests, field-level 
encryption requests, and custom SSL certificates.

### AWS LAMBDA PRICING

Pay only for what you use and charged based on the number of requests for functions and 
the time it takes to execute the code.Price is dependent on the amount of memory allocated to the function.
Amazon Elastic Block Store (EBS) Pricing Pricing is based on three factors:
• Volumes – volume storage for all EBS volumes type is charged by the amount of GB 
provisioned per month.
• Snapshots – based on the amount of space consumed by snapshots in S3. Copying 
snapshots is charged on the amount of data copied across regions.
• Data transfer – inbound data transfer is free, outbound data transfer charges are 
tiered.

## AMAZON DYNAMODB PRICING

Charged based on:
• Provisioned throughput (write).
• Provisioned throughput (read).
• Indexed data storage.
• Data transfer – no charge for data transfer between DynamoDB and other AWS 
services within the same region, across regions is charged on both sides of the 
transfer.
• Global tables – charged based on the resources associated with each replica of the 
table (replicated write capacity units, or rWCUs).
• Reserved Capacity – option available for a one-time upfront fee and commitment 
to paying a minimum usage level at specific hourly rates for the duration of the 
term. Additional throughput is charged at standard rates.
On-demand capacity mode:
• Charged for reads and writes
• No need to specify how much capacity is required
• Good for unpredictable workloads
Provisioned capacity mode:
• Specify number of reads and writes per second
• Can use Auto Scaling
• Good for predictable workloads
• Consistent traffic or gradual changes

## AWS SUPPORT PLANS
There are four AWS support plans available:
• Basic – billing and account support only (access to forums only).
• Developer – business hours support via email.
• Business – 24×7 email, chat, and phone support.
• Enterprise – 24×7 email, chat, and phone support.
Enterprise support comes with a Technical Account Manager (TAM).
Developer allows one person to open unlimited cases.
Business and Enterprise allow unlimited contacts to open unlimited cases.

![image](https://github.com/user-attachments/assets/f10eba51-68b9-4e31-9ec3-c953bc55a308)


## RESOURCE GROUPS AND TAGGING
Tags are key / value pairs that can be attached to AWS resources.
Tags contain metadata (data about data).
Tags can sometimes be inherited – e.g. resources created by Auto Scaling, CloudFormation or Elastic Beanstalk.
Resource groups make it easy to group resources using the tags that are assigned to them. 
You can group resources that share one or more tags.
Resource groups contain general information, such as:
• Region.
• Name.
• Health Checks.
And specific information, such as:
• Public & private IP addresses (for EC2).
• Port configurations (for ELB).
• Database engine (for RDS).

## AWS ORGANIZATIONS AND CONSOLIDATED BILLING
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
Consolidated billing has the following benefits:
• One bill – You get one bill for multiple accounts.
• Easy tracking – You can track the charges across multiple accounts and download 
the combined cost and usage data.
• Combined usage – You can combine the usage across all accounts in the organization to share the volume pricing discounts and Reserved Instance discounts. This can result in a lower charge for your project, department, or company than with individual standalone accounts.
• No extra fee – Consolidated billing is offered at no additional cost.
Limit of 20 linked accounts (by default).
One bill for multiple AWS accounts.
Easy to track charges and allocate costs.
Volume pricing discounts can be applied to resources.
Billing alerts enabled on the Paying account include data for all Linked accounts (or can be created per Linked account)
Consolidated billing allows you to get volume discounts on all your accounts.
Unused reserved instances (RIs) for EC2 are applied across the group.
CloudTrail is on a per account basis and per region basis but can be aggregated into a single 
bucket in the paying account.
Best practices:
• Always enable multi-factor authentication (MFA) on the root account.
• Always use a strong and complex password on the root account.
• The Paying account should be used for billing purposes only. Do not deploy resources into the Paying account.

## AWS QUICK STARTS
Quick Starts are built by AWS architects and partners to help you deploy popular solutions on AWS, based on AWS best practices for security and high availability.These reference deployments implement key technologies automatically on the AWS Cloud, often with a single click and in less than an hour.
Leverages CloudFormation.

### AWS Cost Calculators and Tools
• AWS Cost Explorer – enables you to visualize your usage patterns over time and to identify your underlying cost drivers.
• AWS Pricing Calculator – create cost estimates to suit your AWS use cases.

### AWS COST EXPLORER
The AWS Cost Explorer is a free tool that allows you to view charts of your costs.
You can view cost data for the past 13 months and forecast how much you are likely to 
spend over the next three months.
Cost Explorer can be used to discover patterns in how much you spend on AWS resources 
over time and to identify cost problem areas.
Cost Explorer can help you to identify service usage statistics such as:
• Which services you use the most.
• View metrics for which AZ has the most traffic.
• Which linked account is used the most.

## AWS PRICING CALCULATOR
AWS Pricing Calculator is a web-based service that you can use to create cost estimates to suit your AWS use cases.
AWS Pricing Calculator is useful both for people who have never used AWS and for those who want to reorganize or expand their usage.
AWS Pricing Calculator allows you to explore AWS services based on your use cases and create a cost estimate.

AWS COST & USAGE REPORT
Publish AWS billing reports to an Amazon S3 bucket.
Reports break down costs by:
• Hour, day, month, product, product resource, tags.
Can update the report up to three times a day.
Create, retrieve, and delete your reports using the AWS CUR API Reference.
AWS PRICE LIST API
Query the prices of AWS services.
Price List Service API (AKA the Query API) – query with JSON.
AWS Price List API (AKA the Bulk API) – query with HTML.
Alerts via Amazon SNS when prices change.
AWS BUDGETS
Used to track cost, usage, or coverage and utilization for your Reserved Instances and 
Savings Plans, across multiple dimensions, such as service, or Cost Categories.
Alerting through event-driven alert notifications for when actual or forecasted cost or 
usage exceeds your budget limit, or when your RI and Savings Plans’ coverage or utilization 
drops below your threshold.
Create annual, quarterly, monthly, or even daily budgets depending on your business 
needs.

### AWS BILLING AND PRICING QUIZ QUESTIONS
Answers and explanations are provided below after the last question in this section.

Question 1: Which pricing model is best suited for a batch computing workload that 
requires significant compute power and can be stopped at any time?
1. On-demand instances
2. Dedicated instances
3. Spot instances
4. Reserved instances

Question 2: Which AWS services are free?
1. Amazon EC2 Auto Scaling, CloudFormation, IAM
2. Amazon EC2, CloudFormation, IAM
3. Consolidated billing, EC2 Auto Scaling, NAT Gateway
4. IAM, Amazon S3, outbound data transfer

Question 3: With Amazon S3, which of the following are NOT chargeable items?
1. Quantity of data in S3 buckets
2. 2. Lifecycle transitions
3. Transfer Acceleration
4. Inbound data transfer

Question 4: What are the three fundamentals of pricing in AWS?
1. Compute, storage and inbound data transfer
2. Compute, database and Internet connectivity
3. Compute, storage and outbound data transfer
4. Elasticity, agility, and data transfer

Question 5: Which pricing model is highly flexible with no long-term commitments or 
upfront payments?
1. Dedicated instances
2. Spot instances
3. On-demand
4. Reservations

Question 6: What can you use to assign metadata to AWS resources for cost reporting?
1. Labels
2. Tags
3. ARNs
4. Templates

Question 7: Which AWS pricing feature can be used to take advantage of volume pricing 
discounts across multiple accounts?
1. Consolidated billing
2. TCO Calculator
3. Enterprise Agreement
4. Cost Explorer

Question 8: Which AWS support plan comes with a Technical Account Manager (TAM)
1. Basic
2. Developer
3. Business
4. Enterprise

Question 9: Which of the following is NOT a payment option for Amazon EC2 reserved 
instances?
1. No upfront
2. All upfront
3. All at the end
4. Partial upfront

Question 10: Which tool can an IT manager use to forecast costs over the next 3 months?
1. AWS Organizations
2. AWS TCO Calculator
3. AWS Cost Explorer
4. Amazon CloudWatch








