---
title: VPC connectivity (index)
tags: [aws, saa-c03, domain/secure, service/vpc]
exam: SAA-C03
exam_domains: ["Domain 1: Design Secure Architectures"]
verified_on: 2026-11-08
status: verified
---

# VPC connectivity (index)

- [[vpc-peering-and-transit-gateway]] — connect VPCs to each other: one-to-one peering vs a transit gateway hub.
- [[vpc-endpoints-and-privatelink]] — reach AWS services or another VPC's service privately: gateway and interface endpoints.
- [[hybrid-connectivity-vpn-and-direct-connect]] — connect on-premises to AWS: Site-to-Site VPN and Direct Connect.

Prerequisites: [[vpc-fundamentals]], [[security-groups-vs-nacls]].

```mermaid
flowchart TD
  s{"What must connect?"}
  s -->|VPC to VPC| t1["Peering (two) or transit gateway (many)"]
  s -->|VPC to an AWS service or a service in another VPC| t2["Gateway endpoint (S3, DynamoDB) or PrivateLink"]
  s -->|On-premises to VPC| t3["Site-to-Site VPN or Direct Connect"]
```

> [!info] How to read this
> Pick the left-hand question first, then open the matching note.
