# i2i-Academy--ntroductionToCloud-1
AWS EC2 instance setup and network connectivity verification for i2i Academy Cloud Homework 1

# AWS EC2 Instance Provisioning & Network Verification

This repository contains the technical implementation details for the first cloud infrastructure assignment within the i2i Academy training program. The project focuses on deploying a virtual machine using Amazon Web Services (AWS), configuring network security firewalls, establishing secure remote access, and performing basic Linux file operations.

---

## Infrastructure Specifications

| Parameter | Configuration Details |
-----------   ----------------------
| **Cloud Provider** | Amazon Web Services (AWS) |
| **Compute Service** | Amazon EC2 (Elastic Compute Cloud) |
| **Instance Type** | `t3.micro` (Free Tier Eligible) |
| **Operating System** | Linux Ubuntu Server (LTS) |
| **Public IP Address** | `51.21.254.24` |
| **Local Environment** | Windows Command Prompt (CMD) |

---

## Implementation Steps

### 1. Virtual Machine Deployment
* Provisioned an Ubuntu Server instance via the AWS EC2 Management Console using the `t3.micro` architecture.
* Generated an RSA cryptographic key pair named `i2i-key.pem` for secure public-key authentication and downloaded it to the local system.

### 2. Network Connectivity Validation (Ping Test)
* Configured the instance's AWS Security Group to allow inbound **All ICMP - IPv4** traffic from any source (`0.0.0.0/0`).
* Executed an ICMP network diagnostics check from the local machine:
```bash
ping 51.21.254.24
