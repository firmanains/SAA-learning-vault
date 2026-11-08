---
title: Monitoring and audit (index)
aliases: [monitoring index, CloudWatch CloudTrail Config]
tags: [aws, saa-c03, domain/resilient]
exam: SAA-C03
exam_domains: ["Domain 2: Design Resilient Architectures"]
verified_on: 2026-11-08
status: verified
---

# Monitoring and audit (index)

This topic was too large for one note. CloudWatch, CloudTrail and AWS Config are all in the exam guide's in-scope list under Management and Governance.[^1]

- [[cloudwatch]] — metrics, alarms, alarm actions, logs and metric filters.
- [[cloudtrail]] — API activity events, event history, trails, log file integrity.
- [[aws-config]] — configuration history, Config rules, conformance packs, aggregators.

```mermaid
flowchart TD
  q1{"Who made an API call, and when?"}
  q2{"What was the resource configuration, or does it follow a rule?"}
  q3{"Metric, threshold, alarm or application log?"}
  ct["CloudTrail"]
  cfg["AWS Config"]
  cw["CloudWatch"]
  q1 -->|yes| ct
  q1 -->|no| q2
  q2 -->|yes| cfg
  q2 -->|no| q3
  q3 -->|yes| cw
```

> [!info] How to read this
> Match the question word: "who" is CloudTrail, "what was the configuration" or "is it compliant" is Config, "how is it performing" or "alert me" is CloudWatch.

Simplified: real designs use all three together. Each note's comparison table lists the differences.

Related: [[ec2-auto-scaling]] · [[sns-and-fan-out]] · [[eventbridge]]

[^1]: SAA-C03 exam guide, in-scope services appendix — https://d1.awsstatic.com/training-and-certification/docs-sa-assoc/AWS-Certified-Solutions-Architect-Associate_Exam-Guide.pdf (cached in `_exam-guide.md`, accessed 2026-11-08)
