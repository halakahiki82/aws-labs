# Week 1 Day 4 — AWS IAM Architecture & Security Analysis

## Overview

This exercise focused on understanding AWS Identity and Access Management (IAM) architecture and the security implications of identity-based cloud access control.

The objective was to analyze how AWS authenticates users, authorizes actions, and enforces permissions across cloud resources.

---

# Core Concept

AWS IAM controls:
- Identity authentication
- Authorization
- API access
- Resource permissions
- Temporary and long-lived credentials

IAM acts as the foundational security boundary for AWS environments.

---

# IAM Architecture Model

```text
IAM User / Role
        ↓
IAM Policy
        ↓
Allowed AWS Actions
        ↓
AWS Resources