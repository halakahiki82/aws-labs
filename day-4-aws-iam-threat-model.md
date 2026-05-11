# Week 1 Day 4 — AWS IAM Misconfiguration Threat Model

## Overview

This document analyzes common AWS IAM security misconfigurations and the associated risks to cloud infrastructure.

The objective was to understand how identity and permission failures contribute to cloud compromise scenarios.

---

# Threat Model Scope

The following IAM-related risks were analyzed:

- Excessive permissions
- Credential leakage
- Shared administrative access
- Lack of least privilege enforcement
- Long-lived access keys
- Wildcard policy usage

---

# Threat Surface

```text
Developer Workstation
        ↓
AWS CLI / SDK
        ↓
IAM Credentials
        ↓
AWS APIs
        ↓
Cloud Resources