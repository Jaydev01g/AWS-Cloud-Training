# AWS CLOUD COMPUTING CONCEPTS 
Cloud computing is the on-demand delivery of compute power, database storage, 
applications, and other IT resources through a cloud services platform via the Internet with 
pay-as-you-go pricing.
Cloud computing provides a simple way to access servers, storage, databases, and a broad 
set of application services over the Internet.
A cloud services platform such as Amazon Web Services owns and maintains the networkconnected hardware required for these application services, while you provision and use 
what you need via a web application.

## THE 6 ADVANTAGES OF CLOUD
You must understand the following 6 advantages of cloud:
1. Trade capital expense for variable expense.
2. Benefit from massive economies of scale.
3. Stop guessing about capacity.
4. Increase speed and agility.
5. Stop spending money running and maintaining data centers.
6. Go global in minutes.

#### TRADE CAPITAL EXPENSE FOR VARIABLE EXPENSE
Instead of having to invest heavily in data centers and servers before you know how you’re 
going to use them, you can pay only when you consume computing resources, and pay 
only for how much you consume.
#### BENEFIT FROM MASSIVE ECONOMIES OF SCALE
By using cloud computing, you can achieve a lower variable cost than you can get on your 
own. Because usage from hundreds of thousands of customers is aggregated in the cloud, 
providers such as AWS can achieve higher economies of scale, which translates into lower 
pay as-you-go price.
#### STOP GUESSING ABOUT CAPACITY
Eliminate guessing on your infrastructure capacity needs. When you make a capacity 
decision prior to deploying an application, you often end up either sitting on expensive idle 
resources or dealing with limited capacity.
With cloud computing, these problems go away. You can access as much or as little 
capacity as you need and scale up and down as required with only a few minutes’ notice.
#### INCREASE SPEED AND AGILITY
In a cloud computing environment, new IT resources are only a click away, which means 
that you reduce the time to make those resources available to your developers from weeks 
to just minutes.
This results in a dramatic increase in agility for the organization since the cost and time it 
takes to experiment and develop is significantly lower.
#### STOP SPENDING MONEY RUNNING AND MAINTAINING DATA CENTERS
Focus on projects that differentiate your business, not the infrastructure. Cloud computing 
lets you focus on your own customers, rather than on the heavy lifting of racking, stacking, 
and powering servers.
#### GO GLOBAL IN MINUTES
Easily deploy your application in multiple regions around the world with just a few clicks. 
This means you can provide lower latency and a better experience for your customers at 
minimal cost.


## CLOUD COMPUTING MODELS
There are 3 common types of cloud computing model that come up in the exam:
1. Infrastructure as a service (IaaS).
2. Platform as a service (PaaS).
3. Software as a service (SaaS).
#### INFRASTRUCTURE AS A SERVICE (IAAS)
Infrastructure as a Service (IaaS) contains the basic building blocks for cloud IT and typically 
provide access to networking features, computers (virtual or on dedicated hardware), and 
data storage space.
IaaS provides you with the highest level of flexibility and management control over your IT 
resources and is very similar to the existing IT resources that many IT departments and 
developers are familiar with today.
#### PLATFORM AS A SERVICE (PAAS)
Platform as a Service (PaaS) removes the need for your organization to manage the 
underlying infrastructure (usually hardware and operating systems) and allows you to 
focus on the deployment and management of your applications.
This helps you be more efficient as you don’t need to worry about resource procurement, 
capacity planning, software maintenance, patching, or any of the other undifferentiated 
heavy lifting involved in running your application.
#### SOFTWARE AS A SERVICE (SAAS)
Software as a Service (SaaS) provides you with a completed product that is run and 
managed by the service provider. In most cases, people referring to Software as a Service 
are referring to end-user applications.
With a SaaS offering you do not have to think about how the service is maintained or how 
the underlying infrastructure is managed; you only need to think about how you will use 
that piece of software.
A common example of a SaaS application is web-based email which you can use to send 
and receive email without having to manage feature additions to the email product or 
maintain the servers and operating systems that the email program is running on.
SaaS provides high availability, fault tolerance, scalability an elasticity.

## TYPES OF CLOUD DEPLOYMENT
There are 3 common types of cloud deployment that come up in the exam:
1. Public Cloud – e.g. AWS, Microsoft Azure, Google Cloud Platform (GCP).
2. Hybrid Cloud – a mixture of public and private clouds.
3. Private Cloud (on-premises) – a cloud managed in your own data center, e.g. 
Hyper-V, OpenStack, VMware.
### PUBLIC CLOUD
A cloud-based application is fully deployed in the cloud and all parts of the application run 
in the cloud. Applications in the cloud have either been created in the cloud or have been 
migrated from an existing infrastructure to take advantage of the benefits of cloud 
computing.
Cloud-based applications can be built on low-level infrastructure pieces or can use higher 
level services that provide abstraction from the management, architecting, and scaling 
requirements of core infrastructure.
### HYBRID
A hybrid deployment is a way to connect infrastructure and applications between cloudbased resources and existing resources that are not located in the cloud.
The most common method of hybrid deployment is between the cloud and existing onpremises infrastructure to extend, and grow, an organization’s infrastructure into the cloud 
while connecting cloud resources to the internal system.
### ON-PREMISES
The deployment of resources on-premises, using virtualization and resource management tools, is sometimes called the “private cloud.”
On-premises deployment doesn’t provide many of the benefits of cloud computing but is 
sometimes sought for its ability to provide dedicated resources.
In most cases this deployment model is the same as legacy IT infrastructure while using application management and virtualization technologies to try and increase resource utilization.

### CLOUD COMPUTING CONCEPTS
Answers and explanations are provided below after the last question in this section.
Question 1: What is a key cost advantage of moving to the AWS Cloud?
1. Many services are free
2. You can provision what you need and scale on demand
3. You can deploy services using an API
4. You can scale almost limitlessly
Question 2: Which of the following is an advantage of cloud computing?
1. Trade capital expense for variable expense
2. Trade operational expense for capital expense
3. Go global in days
4. Outsource all application development
#### CLOUD COMPUTING CONCEPTS ANSWERS
Question 1: What is a key cost advantage of moving to the AWS Cloud?
1. Many services are free
2. You can provision what you need and scale on demand
3. You can deploy services using an API
4. You can scale almost limitlessly
Answer: 2
Explanation:
1 is incorrect. This is true, but it's not the best reason to move to AWS as you still have 
to pay for most compute and storage services
2 is correct. This is a great reason to move to the cloud and a key cost benefit. This 
means you are only ever paying for resources that you are actually using, with little 
or no idle capacity
3 is incorrect. This is an advantage of the cloud, but not related to cost
4 is incorrect. This is true but not a key cost advantage.
Question 2: Which of the following is an advantage of cloud computing?
1. Trade capital expense for variable expense
2. Trade operational expense for capital expense
3. Go global in days
4. Outsource all application development
Answer: 1
Explanation:
1 is correct. This is an advantage of cloud computing. You can reduce or eliminate 
capital expense in favor of variable operational expenses
2 is incorrect. This is the opposite of what you want, it is better to trade capital 
expense for operational/variable expense
3 is incorrect. It should be "Go global in minutes"!
4 is incorrect. You cannot outsource all application development with AWS.

## AWS GLOBAL INFRASTRUCTURE
This article covers AWS Global Infrastructure training which is a key technology area 
covered in the Cloud Practitioner exam blueprint. The AWS infrastructure is built around 
Regions and Availability Zones (AZs).
An AWS Region is a physical location in the world where AWS have multiple AZs.
AZs consist of one or more discrete data centers, each with redundant power, networking, 
and connectivity, housed in separate facilities.
Each region is completely independent. Each Availability Zone is isolated, but the 
Availability Zones in a region are connected through low-latency links.
AWS are constantly expanding around the world and currently there are:
#### REGIONS
A region is a geographical area.
Each region consists of 2 or more availability zones.
Each Amazon Region is designed to be completely isolated from the other Amazon 
Regions.
Each AWS Region has multiple Availability Zones and data centers.
You can replicate data within a region and between regions using private or public Internet 
connections.
You retain complete control and ownership over the region in which your data is physically 
located, making it easy to meet regional compliance and data residency requirements.
Note that there is a charge for data transfer between regions.
When you launch an EC2 instance, you must select an AMI that’s in the same region. If the 
AMI is in another region, you can copy the AMI to the region you’re using.
#### Regions and Endpoints:
• When you work with an instance using the command line interface or API actions, 
you must specify its regional endpoint.
• To reduce data latency in your applications, most Amazon Web Services offer a 
regional endpoint to make your requests.
• An endpoint is a URL that is the entry point for a web service.
• For example, https://dynamodb.us-west-2.amazonaws.com is an entry point for 
the Amazon DynamoDB service.
#### AVAILABILITY ZONES
Availability Zones are physically separate and isolated from each other.
AZs span one or more data centers and have direct, low-latency, high throughput, and 
redundant network connections between each other.
Each AZ is designed as an independent failure zone.
When you launch an instance, you can select an Availability Zone or let AWS choose one 
for you.
If you distribute your EC2 instances across multiple Availability Zones and one instance 
fails, you can design your application so that an instance in another Availability Zone can 
handle requests.
You can also use Elastic IP addresses to mask the failure of an instance in one Availability 
Zone by rapidly remapping the address to an instance in another Availability Zone.
An Availability Zone is represented by a region code followed by a letter identifier; for 
example, us-east-1a.
To ensure that resources are distributed across the Availability Zones for a region, AWS 
independently map Availability Zones to names for each AWS account.
For example, the Availability Zone us-east-1a for your AWS account might not be the same 
location as us-east-1a for another AWS account.
To coordinate Availability Zones across accounts, you must use the AZ ID, which is a unique 
and consistent identifier for an Availability Zone.
AZs are physically separated within a typical metropolitan region and are in lower risk flood 
plains.
AZs use discrete UPS and onsite backup generation facilities and are fed via different grids 
from independent facilities.
AZs are all redundantly connected to multiple tier-1 transit providers.
The following graphic shows three AWS Regions each of which has three Availability Zones:
#### LOCAL ZONES
AWS Local Zones place compute, storage, database, and other select AWS services closer 
to end-users.
With AWS Local Zones, you can easily run highly demanding applications that require 
single-digit millisecond latencies to your end-users.
Each AWS Local Zone location is an extension of an AWS Region where you can run your 
latency sensitive applications using AWS services such as Amazon Elastic Compute Cloud, 
Amazon Virtual Private Cloud, Amazon Elastic Block Store, Amazon File Storage, and 
Amazon Elastic Load Balancing in geographic proximity to end-users.
AWS Local Zones provide a high-bandwidth, secure connection between local workloads 
and those running in the AWS Region, allowing you to seamlessly connect to the full range 
of in-region services through the same APIs and tool sets.
#### AWS WAVELENGTH
AWS Wavelength enables developers to build applications that deliver single-digit 
millisecond latencies to mobile devices and end-users.
AWS developers can deploy their applications to Wavelength Zones, AWS infrastructure 
deployments that embed AWS compute and storage services within the 
telecommunications providers’ datacenters at the edge of the 5G networks, and 
seamlessly access the breadth of AWS services in the region.
AWS Wavelength brings AWS services to the edge of the 5G network, minimizing the 
latency to connect to an application from a mobile device.
#### AWS OUTPOSTS
AWS Outposts bring native AWS services, infrastructure, and operating models to virtually any data center, co-location space, or on-premises facility.
You can use the same AWS APIs, tools, and infrastructure across on-premises and the AWS 
cloud to deliver a truly consistent hybrid experience.
AWS Outposts is designed for connected environments and can be used to support 
workloads that need to remain on-premises due to low latency or local data processing 
needs.
#### EDGE LOCATIONS AND REGIONAL EDGE CACHES
Edge locations are Content Delivery Network (CDN) endpoints for CloudFront.
There are many more edge locations than regions.
Currently there are over 200 edge locations.
Regional Edge Caches sit between your CloudFront Origin servers and the Edge Locations.
A Regional Edge Cache has a larger cache-width than each of the individual Edge Locations.
The following diagram shows CloudFront Edge locations:
#### AWS GLOBAL INFRASTRUCTURE QUIZ 
##### QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: What is an availability zone composed of?
1. A collection of edge locations
2. A collection of VPCs
3. One or more DCs in a location
4. One or more regions

Question 2: What is an AWS Region composed of?
1. Two or more Virtual Private Clouds (VPC)
2. Two or more availability zones
3. At least one availability zone
4. A collection of EC2 instances

#### AWS GLOBAL INFRASTRUCTURE ANSWERS
Question 1: What is an availability zone composed of?
1. A collection of edge locations
2. A collection of VPCs
3. One or more DCs in a location
4. One or more regions
Answer: 3
Explanation:
1 is incorrect. An availability zone is not a collection of edge locations.
2 is incorrect. An availability zone is not a collection of VPCs.
3 is correct. Availability Zones are physically separate and isolated from each other. 
They are located in one or more data centers in a geographical area.
4 is incorrect. Availability zones are contained within regions, not the other way 
around.
Question 2: What is an AWS Region composed of?
1. Two or more Virtual Private Clouds (VPC)
2. Two or more availability zones
3. At least one availability zone
4. A collection of EC2 instances
Answer: 2
Explanation:
1 is incorrect. Virtual Private Clouds (VPCs), which will be discussed later in the course, 
are contained within a region but it's not necessary to have more than one VPC in a 
region
2 is correct. Every region has at least 2 availability zones which are composed of one or 
more data centers
3 is incorrect. There are always at least 2 availability zones in a region
4 is incorrect. EC2 instances, which are computer instances, run in a VPC and within a 
region, but this is not how we define a region.
#### AWS IAM
AWS Identity and Access Management (IAM) is a web service that helps you securely 
control access to AWS resources.
You use IAM to control who is authenticated (signed in) and authorized (has permissions) 
to use resources.
IAM makes it easy to provide multiple users secure access to AWS resources.
When you first create an AWS account, you begin with a single sign-in identity that has 
complete access to all AWS services and resources in the account.
This identity is called the AWS account root user and is accessed by signing in with the 
email address and password that you used to create the account.
IAM can be used to manage:
• Users.
• Groups.
• Access policies.
• Roles.
• User credentials.
• User password policies.
• Multi-factor authentication (MFA).
• API keys for programmatic access (CLI).
IAM provides the following features:
• Shared access to your AWS account.
• Granular permissions.
• Secure access to AWS resources for application that run on Amazon EC2.
• Multi-Factor authentication.
• Identity federation.
• Identity information for assurance.
• PCI DSS compliance.
• Integrated with many AWS services.
• Eventually consistent.
• Free to use.
You can work with AWS Identity and Access Management in any of the following ways:
• AWS Management Console.
• AWS Command Line Tools.
• AWS SDKs.
• IAM HTTPS API.
By default, new users are created with NO access to any AWS services – they can only login 
to the AWS console.
Permission must be explicitly granted to allow a user to access an AWS service.
IAM users are individuals who have been granted access to an AWS account.
Each IAM user has three main components:
• A username.
• A password.
• Permissions to access various resources.
You can apply granular permissions with IAM.
You can assign users individual security credentials such as access keys, passwords, and 
multi-factor authentication devices.
IAM is not used for application-level authentication.
Identity Federation (including AD, Facebook etc.) can be configured allowing secure access 
to resources in an AWS account without creating an IAM user account.
Multi-factor authentication (MFA) can be enabled/enforced for the AWS account and for 
individual users under the account.
MFA uses an authentication device that continually generates random, six-digit, single-use 
authentication codes.
You can authenticate using an MFA device in the following two ways:
• Through the AWS Management Console – the user is prompted for a user name, 
password, and authentication code.
• Using the AWS API – restrictions are added to IAM policies and developers can 
request temporary security credentials and pass MFA parameters in their AWS STS 
API requests.
• Using the AWS CLI by obtaining temporary security credentials from STS (aws sts 
get-session-token).
It is a best practice to always setup multi-factor authentication on the root account.
IAM is universal (global) and does not apply to regions.
IAM replicates data across multiple data centers around the world.
The “root account” is the account created when you setup the AWS account. It has 
complete Admin access and is the only account that has this access by default.
It is a best practice to avoid using the root account for anything other than billing.
Power user access allows all permissions except the management of groups and users in 
IAM.
Temporary security credentials consist of the AWS access key ID, secret access key, and 
security token.
IAM can assign temporary security credentials to provide users with temporary access to 
services/resources.
To sign-in you must provide your account ID or account alias in addition to a user name 
and password.
The sign-in URL includes the account ID or account alias, e.g.:
https://My_AWS_Account_ID.signin.aws.amazon.com/console/.
Alternatively, you can sign-in at the following URL and enter your account ID or alias.
manually:
https://console.aws.amazon.com/
IAM integrates with many different AWS services.
Authentication Methods
Console password:
• A password that the user can enter to sign in to interactive sessions such as the 
#### AWS Management Console.
• You can allow users to change their own passwords.
• You can allow selected IAM users to change their passwords by disabling the 
option for all users and using an IAM policy to grant permissions for the selected 
users.
Access Keys:
• A combination of an access key ID and a secret access key.
• You can assign two active access keys to a user at a time.
• These can be used to make programmatic calls to AWS when using the API in 
program code or at a command prompt when using the AWS CLI or the AWS 
PowerShell tools.
• You can create, modify, view, or rotate access keys.
• When created IAM returns the access key ID and secret access key.
• The secret access is returned only at creation time and if lost a new key must be 
created.
• Ensure access keys and secret access keys are stored securely.
• Users can be given access to change their own keys through IAM policy (not from 
the console).
• You can disable a user’s access key which prevents it from being used for API calls.
Server certificates:
• SSL/TLS certificates that you can use to authenticate with some AWS services.
• AWS recommends that you use the AWS Certificate Manager (ACM) to provision, 
manage and deploy your server certificates.
• Use IAM only when you must support HTTPS connections in a region that is not 
supported by ACM.
#### IAM USERS
An IAM user is an entity that represents a person or service.
Can be assigned:
• An access key ID and secret access key for programmatic access to the AWS API, 
CLI, SDK, and other development tools.
• A password for access to the management console.
By default, users cannot access anything in your account.
The account root user credentials are the email address used to create the account and a 
password.
The root account has full administrative permissions, and these cannot be restricted.
Best practice for root accounts:
• Don’t use the root user credentials.
• Don’t share the root user credentials.
• Create an IAM user and assign administrative permissions as required.
• Enable MFA.
IAM users can be created to represent applications, and these are known as “service 
accounts”.
You can have up to 5000 users per AWS account.
Each user account has a friendly name and an ARN which uniquely identifies the user 
across AWS.
A unique ID is also created which is returned only when you create the user using the API, 
Tools for Windows PowerShell, or the AWS CLI.
You should create individual IAM accounts for users (best practice not to share accounts).
The Access Key ID and Secret Access Key are not the same as a password and cannot be 
used to login to the AWS console.
The Access Key ID and Secret Access Key can only be used once and must be regenerated if 
lost.
A password policy can be defined for enforcing password length, complexity etc. (applies 
to all users).
You can allow or disallow the ability to change passwords using an IAM policy.
Access keys and passwords should be changed regularly.
### GROUPS
Groups are collections of users and have policies attached to them.
A group is not an identity and cannot be identified as a principal in an IAM policy.
Use groups to assign permissions to users.
Use the principle of least privilege when assigning permissions.
You cannot nest groups (groups within groups).
### ROLES
Roles are created and then “assumed” by trusted entities and define a set 
of permissions for making AWS service requests.
With IAM Roles you can delegate permissions to resources for users and services without 
using permanent credentials (e.g. user name and password).
IAM users or AWS services can assume a role to obtain temporary security credentials that 
can be used to make AWS API calls.
You can delegate using roles.
There are no credentials associated with a role (password or access keys).
IAM users can temporarily assume a role to take on permissions for a specific task.
A role can be assigned to a federated user who signs in using an external identity provider.
Temporary credentials are primarily used with IAM roles and automatically expire.
Roles can be assumed temporarily through the console or programmatically with the AWS 
CLI, Tools for Windows PowerShell, or the API.
IAM roles with EC2 instances:
• IAM roles can be used for granting applications running on EC2 instances 
permissions to AWS API requests using instance profiles.
• Only one role can be assigned to an EC2 instance at a time.
• A role can be assigned at the EC2 instance creation time or at any time afterwards.
• When using the AWS CLI or API instance profiles must be created manually (it’s 
automatic and transparent through the console).
• Applications retrieve temporary security credentials from the instance metadata.

## AWS SECURITY TOKEN SERVICE (AWS STS)
The AWS STS is a web service that enables you to request temporary, limited-privilege 
credentials for IAM users or for users that you authenticate (federated users).
Temporary security credentials work almost identically to long-term access key credentials 
that IAM users can use, with the following differences:
• Temporary security credentials are short-term.
• They can be configured to last anywhere from a few minutes to several hours.
• After the credentials expire, AWS no longer recognizes them or allows any kind of 
access to API requests made with them.
• Temporary security credentials are not stored with the user but are generated 
dynamically and provided to the user when requested.
• When (or even before) the temporary security credentials expire, the user can 
request new credentials, if the user requesting them still has permission to do so.
Advantages of STS are:
• You do not have to distribute or embed long-term AWS security credentials with 
an application.
• You can provide access to your AWS resources to users without having to define an 
AWS identity for them (temporary security credentials are the basis for IAM Roles 
and ID Federation).
• The temporary security credentials have a limited lifetime, so you do not have to 
rotate them or explicitly revoke them when they’re no longer needed.
• After temporary security credentials expire, they cannot be reused (you can specify 
how long the credentials are valid for, up to a maximum limit)
Users can come from three sources.
1) Federation (typically AD):
• Uses SAML 2.0.
• Grants temporary access based on the users AD credentials.
• Does not need to be a user in IAM.
• Single sign-on allows users to login to the AWS console without assigning IAM 
credentials.
2) Federation with Mobile Apps:
• Use Facebook/Amazon/Google or other OpenID providers to login.
3) Cross Account Access:
• Allows users from one AWS account access resources in another.
• To make a request in a different account the resource in that account must have 
an attached resource-based policy with the permissions you need.
• Or you must assume a role (identity-based policy) within that account with the 
permissions you need.

## IAM BEST PRACTICES
Lock away the AWS root user access keys.
Create individual IAM users.
Use AWS defined policies to assign permissions whenever possible.
Use groups to assign permissions to IAM users.
Grant least privilege.
Use access levels to review IAM permissions.
Configure a strong password policy for users.
Enable MFA.
Use roles for applications that run on AWS EC2 instances.
Delegate by using roles instead of sharing credentials.
Rotate credentials regularly.
Remove unnecessary credentials.
Use policy conditions for extra security.
Monitor activity in your AWS account.

### AWS IDENTITY AND ACCESS MANAGEMENT QUIZ 
#### QUESTIONS
Answers and explanations are provided below after the last question in this section.
Question 1: An access key ID and secret access key is associated with which IAM entity?
1. User
2. Group
3. Role
4. Policy
Question 2: What is the main credential for an AWS root account?
1. Administrator
2. root
3. The email address used to create the account
4. The account number
Question 3: Which principle should be used when assigning permissions to users or 
groups?
1. Most privilege
2. Least privilege
3. Nesting
4. Most restrictive
Question 4: Which IAM entity can be used to delegate permissions?
1. User 
2. Group
3. Role
4. Policy
Question 5: How can you add an extra level of security to your root account?
1. By adding an access key ID and secret access key
35 © 2025 Digital Cloud Training
2. By adding multi-factor authentication (MFA)
3. By setting a strong password
4. By deleting the root account
Question 6: Which of the following is NOT an IAM security best practice?
1. Use groups to assign permissions to IAM users
2. Configure a strong password policy for users
3. Grant most privilege
4. Rotate credentials regularly
Question 7: By default, users are created with what permissions?
1. Full permissions
2. No permissions
3. Minimal permissions
4. No access to the AWS management console
AWS IDENTITY AND ACCESS MANAGEMENT
ANSWERS
Question 1: An access key ID and secret access key is associated with which IAM entity?
1. User
2. Group
3. Role
4. Policy
Answer: 1
Explanation:
1 is correct. An access key ID and secret access key is associated with a user and is used 
for granting programmatic access using the CLI or API
2 is incorrect. You cannot assign an access key ID and secret access key to a group
3 is incorrect. You cannot assign an access key ID and secret access key to a role
4 is incorrect. You cannot assign an access key ID and secret access key to a policy
Question 2: What is the main credential for an AWS root account?
1. Administrator
2. root
3. The email address used to create the account
4. The account number
Answer: 3
Explanation:
1 is incorrect. Administrator is not a credential used with AWS
© 2025 Digital Cloud Training 36
2 is incorrect. root is the username associated with some operating systems such as 
Linux, it is not an actual user name used in your AWS account
3 is correct. The account root user credential is the email address used to create the 
account and a password
4 is incorrect. The account number or alias is used to sign in when using an IAM 
account, rather than the root credentials
Question 3: Which principle should be used when assigning permissions to users or 
groups?
1. Most privilege
2. Least privilege
3. Nesting
4. Most restrictive
Answer: 2
Explanation:
1 is incorrect. This would be a bad practice as it would provide more privileges to users 
than they need to perform their jobs
2 is correct. When assigning permissions always grant the least privileges required. 
This is a security best practice
3 is incorrect. Nesting is not a security practice
4 is incorrect. This would lead to users having too few permissions. You always want to 
make sure people can perform their jobs whilst not providing too much freedom.
Question 4: Which IAM entity can be used to delegate permissions?
1. User 
2. Group
3. Role
4. Policy
Answer: 3
Explanation:
1 is incorrect. You cannot delegate using users
2 is incorrect. You cannot delegate using Groups, but you can assign permissions to 
multiple users through groups.
3 is correct. You can delegate permissions using roles. It's a great way to provide 
permissions to resources for users and services without using permanent credentials
4 is incorrect. You cannot delegate using a policy. You delegate using a role and you 
define permissions to the role through a policy
Question 5: How can you add an extra level of security to your root account?
1. By adding an access key ID and secret access key
2. By adding multi-factor authentication (MFA)
3. By setting a strong password
4. By deleting the root account
Answer: 2
Explanation:
1 is incorrect. No, this will not add security. In fact, it's a security best practice to either 
remove these from your root account or at least minimize their usage
2 is correct. Adding multi-factor authentication (MFA) to your root account adds an 
extra level of security as a device is needed to login as well as a username and 
password. This is a security best practice
3 is incorrect. This is definitely recommended, however this isn't considered an extra 
level of security
4 is incorrect. You cannot delete the root account
Question 6: Which of the following is NOT an IAM security best practice?
1. Use groups to assign permissions to IAM users
2. Configure a strong password policy for users
3. Grant most privilege
4. Rotate credentials regularly
Answer: 3
Explanation:
1 is incorrect. This is an IAM security best practice
2 is incorrect. This is an IAM security best practice
3 is correct. This is not a security best practice. AWS recommend granting least 
privilege when assigning permissions
4 is incorrect. This is an IAM security best practice
Question 7: By default, users are created with what permissions?
1. Full permissions
2. No permissions
3. Minimal permissions
4. No access to the AWS management console
Answer: 2
Explanation:
1 is incorrect. Users are not created with full permissions
2 is correct. Users are created with no permissions. You can then assign permissions 
using groups and policies
3 is incorrect. Users are not created with minimal permissions, they are created with 
no permissions
4 is incorrect. Users will have access to the AWS management console; however they 
won't have any permissions to services by default.


















