# Week 1 Day 2 — AWS vs Azure Virtual Machine Architecture Comparison

## Overview

This exercise focuses on comparing how two major cloud providers (AWS and Azure) implement the same core concept: virtual machines.

No resources were deployed. The goal was to understand architectural and conceptual differences between cloud platforms.

---

## Core Concept

A Virtual Machine in cloud environments provides:
- Compute (CPU/RAM)
- Operating system environment
- Network connectivity
- Storage integration
- Identity-based access control

---

## AWS Implementation (EC2)

AWS uses a modular, component-based model:

- Compute: EC2 instance
- Image: AMI (Amazon Machine Image)
- Networking: VPC + Subnet
- Firewall: Security Groups
- Identity: Key Pair (SSH authentication)
- Storage: EBS volumes

### Key characteristic:
AWS requires explicit configuration of each infrastructure layer.

---

## Azure Implementation (Virtual Machines)

Azure uses a more grouped resource model:

- Compute: Virtual Machine
- Image: Azure VM Image
- Networking: Virtual Network (VNet)
- Firewall: Network Security Group (NSG)
- Identity: SSH key or password authentication
- Storage: Managed Disks
- Resource organization: Resource Groups

### Key characteristic:
Azure encourages bundled deployment through Resource Groups.

---

## Architectural Differences

| Layer | AWS | Azure |
|------|-----|------|
| Compute | EC2 | Virtual Machine |
| Network | VPC | VNet |
| Firewall | Security Group (instance-level) | NSG (subnet or VM level) |
| Resource grouping | Service-based | Resource Group-based |
| Default posture | Highly explicit configuration | More integrated defaults |

---

## Security Perspective (Important)

- AWS provides more granular control but increases configuration complexity
- Azure abstracts more infrastructure, reducing setup friction but potentially hiding network relationships

---

## Key Takeaways

- Both AWS and Azure provide functionally equivalent virtual machine services
- The primary difference is architectural philosophy, not capability
- AWS emphasizes modular infrastructure composition
- Azure emphasizes resource grouping and abstraction

---

## Outcome

Gained conceptual understanding of cross-cloud virtual machine architecture and foundational differences in infrastructure design patterns between AWS and Azure.