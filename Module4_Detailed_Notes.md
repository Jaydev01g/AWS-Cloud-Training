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

   


