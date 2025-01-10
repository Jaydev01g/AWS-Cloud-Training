### Module 3: AWS Services

#### Compute Services
1. **Amazon EC2 (Elastic Compute Cloud)**
   - **Overview**: Provides scalable computing capacity in the AWS cloud, allowing you to run virtual servers.
   - **Key Features**:
     - **Instance Types**: Various types optimized for different use cases (e.g., compute-optimized, memory-optimized).
     - **Auto Scaling**: Automatically adjusts the number of instances based on demand.
     - **Elastic Load Balancing**: Distributes incoming traffic across multiple instances.
     - **Security**: Includes features like security groups, key pairs, and network ACLs.

2. **AWS Lambda**
   - **Overview**: A serverless compute service that runs your code in response to events and automatically manages the underlying compute resources.
   - **Key Features**:
     - **Event-Driven**: Executes code in response to triggers such as changes in data, shifts in system state, or user actions.
     - **Scalability**: Automatically scales from a few requests per day to thousands per second.
     - **Cost-Effective**: You only pay for the compute time you consume.
     - **Integration**: Works seamlessly with other AWS services like S3, DynamoDB, and API Gateway.

#### Storage Services
1. **Amazon S3 (Simple Storage Service)**
   - **Overview**: Object storage service that offers industry-leading scalability, data availability, security, and performance.
   - **Key Features**:
     - **Storage Classes**: Different classes for various use cases (e.g., S3 Standard, S3 Glacier).
     - **Data Management**: Features like versioning, lifecycle policies, and cross-region replication.
     - **Security**: Supports encryption, access control policies, and logging.
     - **Integration**: Easily integrates with other AWS services for data processing and analytics.

2. **Amazon EBS (Elastic Block Store)**
   - **Overview**: Provides persistent block storage volumes for use with Amazon EC2 instances.
   - **Key Features**:
     - **Volume Types**: Various types optimized for different workloads (e.g., SSD, HDD).
     - **Snapshots**: Point-in-time snapshots for backup and recovery.
     - **Encryption**: Supports encryption at rest and in transit.
     - **Performance**: High performance and low-latency storage.

#### Networking Services
1. **Amazon VPC (Virtual Private Cloud)**
   - **Overview**: Enables you to launch AWS resources in a logically isolated virtual network.
   - **Key Features**:
     - **Subnets**: Segments of the VPC that can be public or private.
     - **Security**: Includes security groups, network ACLs, and VPN connections.
     - **Routing**: Customizable route tables for controlling traffic flow.
     - **Peering**: Connects VPCs to share resources across accounts or regions.

2. **Amazon Route 53**
   - **Overview**: A scalable and highly available Domain Name System (DNS) web service.
   - **Key Features**:
     - **Domain Registration**: Register and manage domain names.
     - **DNS Routing**: Various routing policies like simple, weighted, latency-based, and failover.
     - **Health Checks**: Monitors the health of your resources and routes traffic accordingly.
     - **Integration**: Works with other AWS services for seamless management.

#### Database Services
1. **Amazon RDS (Relational Database Service)**
   - **Overview**: Makes it easy to set up, operate, and scale a relational database in the cloud.
   - **Key Features**:
     - **Database Engines**: Supports multiple engines like MySQL, PostgreSQL, Oracle, and SQL Server.
     - **Automated Management**: Handles backups, patching, and scaling.
     - **High Availability**: Multi-AZ deployments for fault tolerance.
     - **Security**: Encryption at rest and in transit, and network isolation.

2. **Amazon DynamoDB**
   - **Overview**: A fast and flexible NoSQL database service for any scale.
   - **Key Features**:
     - **Performance**: Single-digit millisecond response times.
     - **Scalability**: Automatically scales throughput capacity.
     - **Global Tables**: Multi-region, fully replicated tables for high availability.
     - **Security**: Encryption, fine-grained access control, and VPC integration.

3. **Amazon RedShift**
   - **Overview**: A fully managed data warehouse service that makes it simple and cost-effective to analyze all your data.
   - **Key Features**:
     - **Performance**: Optimized for high-performance queries on large datasets.
     - **Scalability**: Scales from a few hundred gigabytes to a petabyte or more.
     - **Integration**: Works with AWS data lakes and other analytics services.
     - **Security**: Encryption, VPC isolation, and compliance certifications.
