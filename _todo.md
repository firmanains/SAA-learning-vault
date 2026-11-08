---
title: SAA-C03 Study Notes — To-do
tags: [aws, saa-c03, todo]
---

# SAA-C03 Study Notes — To-do

Ordered by exam weight. One item = one run of the prompt (new chat each time).
Ticked items are done. ⚠️ means some claims were left out as unverified; check the note's report.

## Domain 1 — Design Secure Architectures (30%)
- [x] IAM fundamentals: users, groups, roles, policies, policy evaluation logic — [[iam-fundamentals]] (2026-11-08) ⚠️ 5 unverified
- [x] IAM advanced: STS, cross-account roles, AWS Organizations and SCPs, IAM Identity Center — [[iam-advanced]] (2026-11-08) ⚠️ 7 unverified
- [x] VPC fundamentals: CIDR, subnets, route tables, internet gateway, NAT gateway — [[vpc-fundamentals]] (2026-11-08) ⚠️ 6 unverified
- [x] VPC security: security groups vs network ACLs — [[security-groups-vs-nacls]] (2026-11-08) ⚠️ 4 unverified
- [x] VPC connectivity: peering, Transit Gateway, VPC endpoints, PrivateLink, Site-to-Site VPN, Direct Connect — [[_index-vpc-connectivity]] (2026-11-08) ⚠️ 13 unverified
- [x] Encryption and secrets: KMS, CloudHSM, ACM, Secrets Manager vs Systems Manager Parameter Store — [[_index-encryption-and-secrets]] (2026-11-08) ⚠️ 12 unverified
- [x] Threat protection: WAF, Shield, GuardDuty, Inspector, Macie, Cognito — [[_index-threat-protection]] (2026-11-08) ⚠️ 14 unverified

## Domain 2 — Design Resilient Architectures (26%)
- [x] EC2 fundamentals: instance types, AMIs, placement groups — [[ec2-fundamentals]] (2026-11-08) ⚠️ 7 unverified
- [x] Elastic Load Balancing: ALB vs NLB vs GWLB — [[elastic-load-balancing]] (2026-11-08) ⚠️ 7 unverified
- [x] EC2 Auto Scaling: groups, launch templates, scaling policies — [[ec2-auto-scaling]] (2026-11-08) ⚠️ 8 unverified
- [x] Decoupling: SQS, SNS, EventBridge, fan-out pattern — [[_index-decoupling]] (2026-11-08) ⚠️ 11 unverified
- [x] Route 53: record types, routing policies, health checks — [[route-53]] (2026-11-08) ⚠️ 9 unverified
- [x] Disaster recovery strategies and AWS Backup — [[disaster-recovery-and-aws-backup]] (2026-11-08) ⚠️ 7 unverified
- [ ] Monitoring and audit: CloudWatch, CloudTrail, AWS Config

## Domain 3 — Design High-Performing Architectures (24%)
- [ ] S3 fundamentals: storage classes, versioning, lifecycle, replication
- [ ] S3 security and performance: bucket policies, encryption, presigned URLs, multipart upload, Transfer Acceleration
- [ ] Block and file storage: EBS vs instance store vs EFS vs FSx
- [ ] RDS and Aurora: Multi-AZ vs read replicas, Aurora features, RDS Proxy
- [ ] DynamoDB: keys, capacity modes, DAX, global tables
- [ ] Caching and edge: ElastiCache, CloudFront, Global Accelerator
- [ ] Serverless and containers: Lambda, API Gateway, ECS, EKS, Fargate
- [ ] Data and analytics overview: Kinesis, Athena, Glue, Redshift
- [ ] Migration and hybrid: DMS, DataSync, Snow Family, Storage Gateway

## Domain 4 — Design Cost-Optimized Architectures (20%)
- [ ] EC2 purchasing options: On-Demand, Reserved, Savings Plans, Spot, Dedicated
- [ ] Cost tools and patterns: Cost Explorer, Budgets, cost-optimized storage and network design
