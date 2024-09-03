# Terraform AWS Infrastructure Setup

## Introduction

This Terraform script sets up a basic AWS infrastructure environment with:

- A Virtual Private Cloud (VPC) with public and private subnets.
- Internet and NAT Gateways for internet access.
- Security Groups for web servers.
- EC2 instances running a basic web server.
- An Application Load Balancer (ALB) to distribute traffic.
- An RDS MySQL database instance.

## Prerequisites

Before you begin, ensure you have the following:

- [Terraform](https://www.terraform.io/downloads.html) installed.
- An AWS account with appropriate permissions.
- AWS credentials configured. You can set these up using environment variables or the AWS CLI.

### Configure AWS Credentials

You can configure your AWS credentials using environment variables:

```bash
export AWS_ACCESS_KEY_ID=<your-access-key-id>
export AWS_SECRET_ACCESS_KEY=<your-secret-access-key>
