---
title: Threat protection (index)
aliases: [threat protection index]
tags: [aws, saa-c03, domain/secure]
exam: SAA-C03
exam_domains: ["Domain 1: Design Secure Architectures"]
verified_on: 2026-11-08
status: verified
---

# Threat protection (index)

This topic was too large for one note. It maps to exam task statement 1.2 (design secure workloads and applications: Cognito, GuardDuty, Macie, Shield, WAF). Inspector is in the exam guide's in-scope services list.

- [[waf-and-shield]] — AWS WAF web ACLs, rate-based rules, Shield Standard vs Advanced.
- [[guardduty-inspector-macie]] — threat detection, vulnerability scanning, and sensitive data discovery.
- [[cognito]] — user pools vs identity pools.

```mermaid
flowchart TD
  q1{"Filter web requests by content or rate?"}
  q2{"DDoS protection?"}
  q3{"Detect suspicious activity from logs?"}
  q4{"Scan EC2, ECR, Lambda for vulnerabilities?"}
  q5{"Find sensitive data in S3?"}
  q6{"App sign-up and sign-in?"}
  q7{"App users need AWS credentials?"}
  waf["AWS WAF"]
  sh["Shield Standard or Advanced"]
  gd["GuardDuty"]
  insp["Inspector"]
  mac["Macie"]
  up["Cognito user pool"]
  ip["Cognito identity pool"]
  q1 -->|yes| waf
  q1 -->|no| q2
  q2 -->|yes| sh
  q2 -->|no| q3
  q3 -->|yes| gd
  q3 -->|no| q4
  q4 -->|yes| insp
  q4 -->|no| q5
  q5 -->|yes| mac
  q5 -->|no| q6
  q6 -->|yes| up
  q6 -->|no| q7
  q7 -->|yes| ip
```

> [!info] How to read this
> Read the exam requirement, then follow the first question that matches. Each service answers one kind of problem.

Simplified: Shield Standard is automatic. Choose Shield Advanced only for its extra capabilities, see [[waf-and-shield]].

Related: [[_index-encryption-and-secrets]] · [[_index-vpc-connectivity]] · [[iam-fundamentals]]
