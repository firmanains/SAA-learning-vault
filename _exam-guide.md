---
title: SAA-C03 exam guide (local cache)
tags: [aws, saa-c03, exam-guide]
---

# SAA-C03 exam guide (local cache)

- **Source URL:** https://d1.awsstatic.com/training-and-certification/docs-sa-assoc/AWS-Certified-Solutions-Architect-Associate_Exam-Guide.pdf
- **Accessed:** 2026-11-08
- **Exam version:** Version 1.1 SAA-C03
- Scope facts only. Not a source for how services work.

## Exam format (from the guide)
- 50 scored questions and 15 unscored. Passing score 720 on a scale of 100–1,000. Compensatory scoring: only the overall exam must be passed.

## Domains and weights
1. Domain 1: Design Secure Architectures — 30%
2. Domain 2: Design Resilient Architectures — 26%
3. Domain 3: Design High-Performing Architectures — 24%
4. Domain 4: Design Cost-Optimized Architectures — 20%

## Task statements
**Domain 1**
- 1.1 Design secure access to AWS resources (multi-account access control, federation and IAM Identity Center, least privilege, shared responsibility; MFA for IAM and root users; users/groups/roles/policies; STS, role switching, cross-account access; Control Tower and SCPs; resource policies; federating a directory service with IAM roles)
- 1.2 Design secure workloads and applications (credentials security, endpoints, Cognito/GuardDuty/Macie, SGs, route tables, NACLs, NAT, public/private subnets, Shield, WAF, Identity Center, Secrets Manager, VPN, Direct Connect)
- 1.3 Determine appropriate data security controls (KMS, ACM/TLS, key policies, backups and replication, lifecycle, key rotation, certificate renewal)

**Domain 2**
- 2.1 Design scalable and loosely coupled architectures
- 2.2 Design highly available and/or fault-tolerant architectures

**Domain 3**
- 3.1 Determine high-performing and/or scalable storage solutions
- 3.2 Design high-performing and elastic compute solutions
- 3.3 Determine high-performing database solutions
- 3.4 Determine high-performing and/or scalable network architectures
- 3.5 Determine high-performing data ingestion and transformation solutions

**Domain 4**
- 4.1 Design cost-optimized storage solutions
- 4.2 Design cost-optimized compute solutions
- 4.3 Design cost-optimized database solutions
- 4.4 Design cost-optimized network architectures

## In-scope services (appendix, "non-exhaustive and subject to change")
- **Security, Identity, and Compliance:** AWS Artifact, Audit Manager, ACM, CloudHSM, Amazon Cognito, Amazon Detective, AWS Directory Service, AWS Firewall Manager, Amazon GuardDuty, AWS IAM Identity Center (AWS Single Sign-On), AWS IAM, Amazon Inspector, AWS KMS, Amazon Macie, AWS Network Firewall, AWS RAM, AWS Secrets Manager, AWS Security Hub, AWS Shield, AWS WAF
- **Management and Governance:** AWS Auto Scaling, CloudFormation, CloudTrail, Amazon CloudWatch, AWS CLI, Compute Optimizer, AWS Config, AWS Control Tower, Health Dashboard, License Manager, Managed Grafana, Managed Service for Prometheus, Management Console, AWS Organizations, Proton, Service Catalog, Systems Manager, Trusted Advisor, Well-Architected Tool
- **Networking and Content Delivery:** Client VPN, CloudFront, Direct Connect, ELB, Global Accelerator, PrivateLink, Route 53, Site-to-Site VPN, Transit Gateway, Amazon VPC
- **Storage:** AWS Backup, EBS, EFS, FSx (all types), S3, S3 Glacier, Storage Gateway
- **Compute:** Batch, EC2, EC2 Auto Scaling, Elastic Beanstalk, Outposts, Serverless Application Repository, VMware Cloud on AWS, Wavelength
- **Containers:** ECS Anywhere, EKS Anywhere, EKS Distro, ECR, ECS, EKS
- **Serverless:** AppSync, Fargate, Lambda
- **Database:** Aurora, Aurora Serverless, DocumentDB, DynamoDB, ElastiCache, Keyspaces, Neptune, QLDB, RDS, Redshift
- **Application Integration:** AppFlow, AppSync, EventBridge, Amazon MQ, SNS, SQS, Step Functions
- **Analytics:** Athena, Data Exchange, Data Pipeline, EMR, Glue, Kinesis, Lake Formation, MSK, OpenSearch Service, QuickSight, Redshift
- **Migration and Transfer:** Application Discovery Service, Application Migration Service, DMS, DataSync, Migration Hub, Snow Family, Transfer Family
- **AWS Cost Management:** Budgets, Cost and Usage Report, Cost Explorer, Savings Plans
- Other listed categories (Developer Tools, Front-End Web and Mobile, Machine Learning, Media Services) are in the guide's appendix and not copied here.
- Out-of-scope examples listed on page 20 start with Amazon CloudSearch, Amazon MWAA, Amazon Sumerian. The rest of that list was not read.
