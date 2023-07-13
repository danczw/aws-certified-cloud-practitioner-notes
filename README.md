# AWS Cloud Practitioner - Learning Path Notes 


<br>

## Overview

**Institution:** Amazon<br>
**Course:** AWS Certified Cloud Practitioner<br>
**Tags:** [aws, aws_cloud_practitioner, aws_essentials]<br>
**Source:** https://aws.amazon.com/certification/certified-cloud-practitioner/<br>
**Links**
- [AWS Cloud Practitioner Essentials | Free Digital Training | AWS  (aws.amazon.com)](https://aws.amazon.com/training/digital/aws-cloud-practitioner-essentials/)
- [AWS glossary - AWS General Reference (docs.aws.amazon.com)](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html)
- [Whitepaper: Overview of AWS Services (pdf) (awsstatic.com)](https://d0.awsstatic.com/whitepapers/aws-overview.pdf)

**Exam Prep Documents**
- [Exam Guide - AWS Cloud Practitioner (pdf)](assets/files/AWS-Certified-Cloud-Practitioner_Exam-Guide.pdf)
- [Exam Sample Questions - AWS Cloud Practitioner (pdf)](assets/files/AWS-Certified-Cloud-Practitioner_Sample-Questions.pdf)

**Table of Contents**
- [1. Compute in the Cloud](#1-compute-in-the-cloud)
- [2. Global Infrastructure](#2-global-infrastructure)
- [3. Networking](#3-networking)
- [4. Storage and Databases](#4-storage-and-databases)
- [5. Security](#5-security)
- [6. Monitoring and Analytics](#6-monitoring-and-analytics)
- [7. Pricing and Support](#7-pricing-and-support)
- [8. Additional Resources](#8-additional-resources)

<br>

---
---

<br>

## **1. Compute in the Cloud**

### Notes
- [1.1: Cloud Computing](notes/1.1_Cloud_Computing.md)
- [1.2: EC2](notes/1.1_Cloud_Computing.md)
- [1.3: Elastic Load Balancing](notes/1.3_Elastic_Load_Balancing.md)
- [1.4: SNS and SQS](notes/1.4_SNS_and_SQS.md)
- [1.5: Additional Compute Services](notes/1.5_Additional_Compute_Services.md)

### Compute Summary
> - **cloud computing**: on-demand delivery of IT resources over the internet with pay-as-you-go pricing
>
> - **EC2**: dynamically spin up and spin down virtual servers called EC2 instances, when launching an EC2 instance, you choose the instance family. The instance family determines the hardware the instance runs on
>
> - **EC2 categories**: general purpose, compute optimized, memory optimized, accelerated computing, and storage optimized
>
> - **Scalinng EC2**: *vertically* by resizing the instance, or *horizontally* by launching new instances and adding them to the pool
>
> - **Amazon EC2 Auto Scaling**: automated horizontal scaling 
>
> - **Elastic Load Balancer**: distribute the incoming traffic across compute instances comes into play 
>
> - **EC2 pricing**: *On-Demand*, which is the most flexible and has no contract, *spot pricing*, which allows to utilize unused capacity at a discounted rate, *Savings Plans* or *Reserved Instances*, which allow to enter into a contract with AWS to get a discounted rate when committing to a certain level of usage, and *Savings Plans* which apply to AWS Lambda, and AWS Fargate, as well as EC2 instances. 
>
> - **Amazon Simple Queue Service (SQS)**: decouple system components - messages remain in the queue until they are either consumed or deleted
>
> - **Amazon Simple Notification Service (SNS)**: sending messages like emails, text messages, push notifications, or even HTTP requests - once a message is published, it is sent to all of these subscribers
>
> - **Amazon Elastic Container Service (ECS)**: container orchestration tools - use these tools with self managed EC2 instances
>
> - **Amazon Elastic Kubernetes Service (EKS)**: container orchestration tools - use these tools with self managed EC2 instances
>
> - **AWS Fargate**: allows to run containers on top of a serverless compute platform
>
> - **AWS Lambda**: allows to upload code, and configure it to run based on triggers - get charged for when the code is actually running (No containers, no virtual machines. Just code and configuration) 

### Additional Resources
- [Compute on AWS (aws.amazon.com)](https://aws.amazon.com/products/compute)
- [AWS Compute Blog (aws.amazon.com)](https://aws.amazon.com/blogs/compute/)
- [AWS Compute Services (docs.aws.amazon.com)](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/compute-services.html)
- [Hands-On Tutorials: Compute (aws.amazon.com)](https://aws.amazon.com/getting-started/hands-on/?awsf.getting-started-category=category%23compute&awsf.getting-started-content-type=content-type%23hands-on)
- [Category Deep Dive: Serverless (aws.amazon.com)](https://aws.amazon.com/getting-started/deep-dive-serverless/)
- [AWS Customer Stories: Serverless (aws.amazon.com)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23serverless)

<br>

---
---

<br>

## **2. Global Infrastructure and Reliability**

### Notes
- [2.1: Global Infrastructure](notes/2.1_Global_Infrastructure.md)
- [2.2: Edge Locations](notes/2.2_Edge_Locations.md)
- [2.3: Resource Provisioning](notes/2.3_Resource_Provisioning.md)

### Global Infrastructure Summary
> - **Regions**: geographically isolated areas, where services needed can be accessesd
>
> - **Availability Zones**: allow to run across physically separated buildings, tens of miles of separation within a region, while keeping the application logically unified -> Availability Zones help to solve high availability and disaster recovery scenarios, without any additional effort
>
> - **AWS Edge locations**: run *Amazon CloudFront* to help get content closer to customers, no matter where they are in the world

### Additional Resources

- [Global Infrastructure (aws.amazon.com)](https://aws.amazon.com/about-aws/global-infrastructure/)
- [Interactive map of the AWS Global Infrastructure (infrastructure.aws)](https://www.infrastructure.aws/)
- [Regions and Availability Zones (aws.amazon.com)](https://aws.amazon.com/about-aws/global-infrastructure/regions_az)
- [AWS Networking and Content Delivery Blog (aws.amazon.com)](https://aws.amazon.com/blogs/networking-and-content-delivery/)
- [Tools to Build on AWS (aws.amazon.com)](https://aws.amazon.com/tools/)
- [AWS Customer Stories: Content Delivery (aws.amazon.com)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23content-delivery)

<br>

---
---

<br>

## **3. Networking**

### Notes
- [3.1: Connectivity to AWS](notes/3.1_Connectivity_to_AWS.md)
- [3.2: Subnets and ACLs](notes/3.2_Subnets_and_ACLs.md)
- [3.3: Global Networking](notes/3.3_Global_Networking.md)

### Networking Summary

> - **Amazon Virtual Private Cloud (VPC)**: isolate workloads in AWS
>
> - **Gateways, Network ACLs, and security groups**: methods to craft a network that allows healthy traffic access while dropping subversive attacks before they reach your instance
>
> - **Connect to AWS through VPN and Direct Connect**: secure pipelines that are either encrypted over the general internet or exclusive fiber used by you and you alone
>
> - **Global Networking**: use *Route 53* for DNS and cache content closer to consumers via CloudFront

### Additional Resources

- [Networking and Content Delivery on AWS (aws.amazon.com)](https://aws.amazon.com/products/networking)
- [AWS Networking & Content Delivery Blog (aws.amazon.com)](https://aws.amazon.com/blogs/networking-and-content-delivery/)
- [Amazon Virtual Private Cloud (aws.amazon.com)](https://aws.amazon.com/vpc)
- [What is Amazon VPC? (docs.aws.amazon.com)](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
- [How Amazon VPC works (docs.aws.amazon.com)](https://docs.aws.amazon.com/vpc/latest/userguide/how-it-works.html)

<br>

---
---

<br>

## **4. Storage and Databases**

### Notes
- [4.1: Instance Stores and Amazon EBS](notes/4.1_Instance_Stores_and_Amazon_EBS.md)
- [4.2: Simple Storage Service S3](notes/4.2_Simple_Storage_Service_S3.md)
- [4.3: Elastic File System EFS](notes/4.3_Elastic_File_System_EFS.md)
- [4.4: Relational Database RDS](notes/4.4_Relational_Database_RDS.md)
- [4.5: DynamoDB](notes/4.5_DynamoDB.md)
- [4.6: Redshift](notes/4.6_Redshift.md)
- [4.7: Database Migration Service](notes/4.7_Database_Migration_Service.md)

### Storage and Databases Summary
> - **Elastic Block Store**: local non-ephemeral storage for EC2 instances
>
> - **S3**: storing objects in AWS
>
> - **relational database**: relational data storage with SQL
>
> - **nonrelational database**: key-value pair bases storage systems such as DynamoDB
>
> - **Data Warehouse**: Amazon Redshift for big data BI
>
> - **DMS**: Database Migration Service to aid in migration of existing databases
>
> - **Further storage solutions**: for various specific needs use DocumentDB, Neptune, QLDB and Amazon Managed Blockchain
>
> - **Caching**: ElastiCach and DynamoDB Accelerator to increase speed via caching

### Additional Resources
- [Cloud Storage on AWS (aws.amazon.com)](https://aws.amazon.com/products/storage)
- [AWS Storage Blog (aws.amazon.com)](https://aws.amazon.com/blogs/storage/)
- [Hands-On Tutorials: Storage (aws.amazon.com)](https://aws.amazon.com/getting-started/hands-on/?awsf.getting-started-category=category%23storage&awsf.getting-started-content-type=content-type%23hands-on)
- [AWS Customer Stories: Storage (aws.amazon.com)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23storage)
- [AWS Database Migration Service (aws.amazon.com)](https://aws.amazon.com/dms/)
- [Databases on AWS](https://aws.amazon.com/products/databases)
- [Category Deep Dive: Databases (aws.amazon.com)](https://aws.amazon.com/getting-started/deep-dive-databases/)
- [AWS Database Blog](https://aws.amazon.com/blogs/database/)
- [AWS Customer Stories: Databases (aws.amazon.com)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23databases)

<br>

---
---

<br>

## **5. Security**

### Notes
- [5.1: Shared Responsibility Model in AWS](notes/5.1_Shared_Responsibility_Model_in_AWS.md)
- [5.2: User Permission and Access](notes/5.2_User_Permission_and_Access.md)
- [5.3: AWS Organizations](notes/5.3_Organizations.md)
- [5.4: Compliance](notes/5.4_Compliance.md)
- [5.5: Denial-of-service Attacks in AWS](notes/5.5_Denial-of-service_Attacks_in_AWS.md)
- [5.6: Additional Security Services](notes/5.6_Additional_Security_Services.md)

### Security Summary
> - AWS follows a **shared responsibility model**
>
> - AWS is responsible for **security of the cloud**, while customer is responsible for **security in the cloud**
>
> - with **IAM**, you have users, groups, roles, and policies:
>
>   - **users** log in with a username and password and by default they have no permissions
>
>   - **groups** are groupings of users
>
>   - **roles** are identities that can be assumed to gain access to temporary credentials and permissions for a configurable amount of time
>
>   - in order to give permissions to an identity, **policies** are needed that either explicitly allow or deny a specific action in AWS
>
> - turn on **multi-factor authentication** for users, but especially for the root user which has all the permissions by default and cannot be restricted
>
> - **AWS Organizations** helps to manage multiple accounts in a hierarchical fashion
>
> - use the **AWS Compliance Center** to find more information on compliance and **AWS Artifact** to gain access to compliance documents
>
> - combat DDoS attacks with AWS using tools like **ELB**, security groups, **AWS Shield**, and **AWS WAF**
>
> - pay attention to **encryption**, in transit and at rest.

### Additional Resources
- [Security, Identity, and Compliance on AWS (aws.amazon.com)](https://aws.amazon.com/products/security)
- [Whitepaper: Introduction to AWS Security (docs.aws.amazon.com)](https://docs.aws.amazon.com/whitepapers/latest/introduction-aws-security/welcome.html)
- [Know the AWS shared Resposnsibility Model (docs.aws.amazon.com)](https://docs.aws.amazon.com/whitepapers/latest/aws-security-best-practices/know-the-aws-shared-responsibility-model.html)
- [Whitepaper: Amazon Web Services - Overview of Security Processes (docs.aws.amazon.com)](https://docs.aws.amazon.com/whitepapers/latest/aws-overview-security-processes/aws-overview-security-processes.pdf)
- [AWS Security Blog (aws.amazon.com)](https://aws.amazon.com/blogs/security/)
- [AWS Compliance (aws.amazon.com)](https://aws.amazon.com/compliance)
- [AWS Customer Stories: Security, Identity, and Compliance (aws.amazon.com)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23security-identity-compliance)

<br>

---
---

<br>

## **6. Monitoring and Analytics**

### Notes
- [6.1: CloudWatch](notes/6.1_CloudWatch.md)
- [6.2: CloudTrail](notes/6.2_CloudTrail.md)
- [6.3: Trusted Advisor](notes/6.3_Trusted_Advisor.md)

### Monitoring and Analytics Summary
> - **CloudWatch** can provide near real-time understanding of how systems are behaving, including being alerted to conditions that require attention 
>
> - **CloudTrail** can help to know exactly who did what, when, and from where
>
> - **Trusted Advisor** compiles a quick dashboard of over 40 common concerns around cost, performance, security, and resilience

### Additional Resources

- [Management and Governance on AWS (aws.amazon.com)](https://aws.amazon.com/products/management-tools)
- [Monitoring and Observability (aws.amazon.com)](https://aws.amazon.com/products/management-tools/use-cases/monitoring-and-observability/)
- [Configuration, Compliance, and Auditing (aws.amazon.com)](https://aws.amazon.com/products/management-tools/use-cases/configuration-compliance-and-auditing/)
- [AWS Management & Governance Blog (aws.amazon.com)](https://aws.amazon.com/blogs/mt/)
- [Whitepaper: AWS Governance at Scale (docs.aws.amazon.com)](https://docs.aws.amazon.com/whitepapers/latest/aws-governance-at-scale/introduction.html)

<br>

---
---

<br>

## **7. Pricing and Support**

### Notes
- [7.1: Pricing and Support](notes/7.1_Pricing_and_Support.md)

### Pricing and Support Summary
> - Pay-as-you-go nature of using AWS cloud resources
>
> - Three types of **pricing offers** included in the AWS Free Tier: 12 months free, Always free, and Trials
>
> - Benefits of **consolidated billing** in AWS Organizations
>
> - Tools for planning, estimating, and reviewing AWS costs
>
> - Differences between the five **AWS Support plans**: Basic, Developer, Business, Enterprise On-Ramp, and Enterprise
>
> - How to discover software in **AWS Marketplace**

### Additional Resources

- [AWS Pricing (aws.amazon.com)](https://aws.amazon.com/pricing)
- [AWS Free Tier (aws.amazon.com)](https://aws.amazon.com/free)
- [AWS Cost Management (aws.amazon.com)](https://aws.amazon.com/aws-cost-management/)
- [Whitepaper: How AWS Pricing Works (awsstatic.com)](https://d1.awsstatic.com/whitepapers/aws_pricing_overview.pdf)
- [Whitepaper: Introduction to AWS Economics (awsstatic.com)](https://d1.awsstatic.com/whitepapers/introduction-to-aws-cloud-economics-final.pdf)
- [AWS Support (aws.amazon.com)](https://aws.amazon.com/premiumsupport)
- [AWS Knowledge Center (aws.amazon.com)](https://aws.amazon.com/premiumsupport/knowledge-center/)

<br>

---
---

<br>

## **8. Migration and Innovation**

### Notes
- [8.1: Cloud Adoption Framework CAF](notes/8.1_Cloud_Adoption_Framework_CAF.md)
- [8.2: Cloud Migration Strategies](notes/8.2_Cloud_Migration_Strategies.md)
- [8.3: Innovation with AWS](notes/8.3_Innovation_with_AWS.md)
- [8.4: Well-Architected Framework](notes/8.4_Well_Architected_Framework.md)

##### Migration and Innovation Summary
> - **AWS Cloud Adoption Framework** gives guidance on who to loop into a cloud migration, what their roles are, and the sorts of things that they should be focused on
>
> - there's the **Business**, **People**, and **Governance Perspectives** for nontechnical planning, and the **Platform**, **Security**, and **Operations Perspectives** for technical planning
>
> - 6 R's of migration (different strategies on moving solutions to the cloud): **Rehost, Replatform, Repurchase, Refactor, Retire, and Retain** 
>
> - **AWS Snowball** and **AWS Snowmobile**, which allow to fill in a physical device with data and have it shipped back to AWS who then uploads it for
>
> - 6 pillars of the **AWS Well-Architected Framework**: Operational excellence Security, Reliability, Performance efficiency, Cost optimization, Sustainability
>
> - 6 **advantages of cloud computing**: trade upfront expense for variable expense, benefit from massive economies of scale, stop guessing capacity, increase speed and agility, stop spending money running and maintaining data centers, go global in minutes.

### Additional Resources

- [Migration & Transfer on AWS (aws.amazon.com)](https://aws.amazon.com/products/migration-and-transfer)
- [A Process for Mass Migrations to the Cloud (aws.amazon.com)](https://aws.amazon.com/blogs/enterprise-strategy/214-2/)
- [6 Strategies for Migrating Applications to the Cloud (aws.amazon.com)](https://aws.amazon.com/blogs/enterprise-strategy/6-strategies-for-migrating-applications-to-the-cloud/)
- [AWS Cloud Adoption Framework (aws.amazon.com)](https://aws.amazon.com/professional-services/CAF/)
- [AWS Fundamentals: Core Concepts (aws.amazon.com)](https://aws.amazon.com/getting-started/fundamentals-core-concepts/)
- [AWS Cloud Enterprise Strategy Blog (aws.amazon.com)](https://aws.amazon.com/blogs/enterprise-strategy/)
- [Modernizing with AWS Blog (aws.amazon.com)](https://aws.amazon.com/blogs/modernizing-with-aws/)
- [AWS Customer Stories: Data Center Migration (aws.amazon.com)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23datacenter-migration)
- [AWS Well-Architected (aws.amazon.com)](https://aws.amazon.com/architecture/well-architected/)
- [AWS Well-Architected Framework (docs.aws.amazon.com)](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
- [AWS Architecture Center (aws.amazon.com)](https://aws.amazon.com/architecture)
- [Six Advantages of Cloud Computing (docs.aws.amazon.com)](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html)
- [AWS Architecture Blog (aws.amazon.com)](https://aws.amazon.com/blogs/architecture)

<br>

---
---

<br>

[Self-paced digital training on AWS - AWS Skill Builder](https://explore.skillbuilder.aws/learn/course/134/play/62437/aws-cloud-practitioner-essentials;lp=82)