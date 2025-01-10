### Module 4: Security and Compliance

#### AWS Shared Responsibility Model
- **Overview**: The AWS Shared Responsibility Model delineates the security responsibilities of AWS and its customers.
- **AWS Responsibilities**:
  - **Security of the Cloud**: AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This includes hardware, software, networking, and facilities.
- **Customer Responsibilities**:
  - **Security in the Cloud**: Customers are responsible for managing their data, classifying their assets, and using AWS services securely. This includes configuring security settings, managing user access, and ensuring data encryption.

#### Security Services
1. **Amazon GuardDuty**
   - **Overview**: A threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads.
   - **Key Features**:
     - **Threat Detection**: Uses machine learning, anomaly detection, and integrated threat intelligence.
     - **Continuous Monitoring**: Monitors AWS CloudTrail, VPC Flow Logs, and DNS logs.
     - **Automated Response**: Integrates with AWS Lambda for automated remediation.

2. **AWS WAF (Web Application Firewall)**
   - **Overview**: Protects your web applications from common web exploits that could affect application availability, compromise security, or consume excessive resources.
   - **Key Features**:
     - **Rule-Based Filtering**: Allows you to create custom rules to block common attack patterns.
     - **Real-Time Monitoring**: Provides real-time visibility into web traffic.
     - **Integration**: Works with Amazon CloudFront and Application Load Balancer.

3. **AWS Shield**
   - **Overview**: A managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS.
   - **Key Features**:
     - **Standard Protection**: Automatically included at no extra cost for all AWS customers.
     - **Advanced Protection**: Offers additional detection and mitigation against larger and more sophisticated attacks.
     - **24/7 Support**: Access to the AWS DDoS Response Team (DRT) for advanced protection customers.

#### Compliance Programs
- **Overview**: AWS compliance programs help customers meet various regulatory and compliance requirements.
- **Key Programs**:
  - **ISO Certifications**: AWS is ISO 27001, 27017, and 27018 certified, ensuring adherence to international standards for information security management.
  - **SOC Reports**: AWS provides SOC 1, SOC 2, and SOC 3 reports, which are independent third-party examination reports that demonstrate how AWS achieves key compliance controls and objectives.
  - **GDPR Compliance**: AWS services comply with the General Data Protection Regulation (GDPR) to protect personal data and privacy in the European Union.
  - **HIPAA Compliance**: AWS supports HIPAA compliance for customers who store, process, or transmit protected health information.

#### Tools
1. **AWS Artifact**
   - **Overview**: A self-service portal for on-demand access to AWS compliance reports and select online agreements.
   - **Key Features**:
     - **Compliance Reports**: Access to various compliance reports such as SOC, ISO, and PCI.
     - **Agreements**: Manage agreements like Business Associate Addendum (BAA) for HIPAA compliance.
     - **Audit Support**: Provides documentation to support your internal and external audits.

2. **AWS Key Management Service (KMS)**
   - **Overview**: A managed service that makes it easy to create and control the encryption keys used to encrypt your data.
   - **Key Features**:
     - **Key Management**: Centralized control over the lifecycle and permissions of your encryption keys.
     - **Integration**: Seamlessly integrates with other AWS services for encryption at rest and in transit.
     - **Compliance**: Helps meet compliance requirements with features like key rotation and audit logging.

