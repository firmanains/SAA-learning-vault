---
title: Decoupling (index)
aliases: [decoupling index, SQS SNS EventBridge]
tags: [aws, saa-c03, domain/resilient]
exam: SAA-C03
exam_domains: ["Domain 2: Design Resilient Architectures"]
verified_on: 2026-11-08
status: verified
---

# Decoupling (index)

This topic was too large for one note. It maps to exam task statement 2.1 (design scalable and loosely coupled architectures). SQS, SNS and EventBridge are in the exam guide's in-scope services list under Application Integration.[^1]

- [[sqs]] — queues, standard vs FIFO, visibility timeout, dead-letter queues.
- [[sns-and-fan-out]] — topics, subscribers, filter policies, the SNS + SQS fan-out pattern.
- [[eventbridge]] — event buses, rules, targets, Scheduler.

```mermaid
flowchart TD
  q1{"One consumer must buffer and process work at its own pace?"}
  q2{"One message must reach many consumers or notify people?"}
  q3{"React to AWS, SaaS or app events, or run on a schedule?"}
  sqs["SQS queue"]
  fan["SNS topic + one SQS queue per consumer"]
  eb["EventBridge rule or Scheduler"]
  fifo["FIFO queue if order matters"]
  q1 -->|yes| sqs
  sqs --> fifo
  q1 -->|no| q2
  q2 -->|yes| fan
  q2 -->|no| q3
  q3 -->|yes| eb
```

> [!info] How to read this
> Read the requirement and follow the first question that matches. Fan-out combines two services: SNS delivers, SQS buffers.

Simplified: this is a first-pass guide. Details such as high fan-out (SNS) versus content routing (EventBridge) are in [[eventbridge]].

Related: [[elastic-load-balancing]] · [[ec2-auto-scaling]]

[^1]: SAA-C03 exam guide, in-scope services appendix — https://d1.awsstatic.com/training-and-certification/docs-sa-assoc/AWS-Certified-Solutions-Architect-Associate_Exam-Guide.pdf (cached in `_exam-guide.md`, accessed 2026-11-08)
