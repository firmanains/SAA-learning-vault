---
title: Encryption and secrets (index)
aliases: [encryption index]
tags: [aws, saa-c03, domain/secure]
exam: SAA-C03
exam_domains: ["Domain 1: Design Secure Architectures"]
verified_on: 2026-11-08
status: verified
---

# Encryption and secrets (index)

This topic was too large for one note. It maps to exam task statements 1.3 (data security controls: KMS, ACM/TLS, key rotation, certificate renewal) and 1.2 (credentials security, Secrets Manager).

- [[kms-and-cloudhsm]] — KMS keys, envelope encryption, key policies, rotation, and when CloudHSM is needed instead.
- [[acm-certificates]] — public and private TLS certificates, Region rules, and renewal.
- [[secrets-manager-vs-parameter-store]] — secrets with rotation vs configuration values.

Quick pick:
- Need a key to encrypt data → KMS.
- Need a dedicated, single-tenant HSM → CloudHSM.
- Need a TLS certificate on a load balancer or CloudFront → ACM.
- Need a rotating database password → Secrets Manager.
- Need cheap configuration storage → Parameter Store.

Related: [[iam-fundamentals]] · [[vpc-fundamentals]]
