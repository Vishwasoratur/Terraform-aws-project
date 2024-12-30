# Terraform-aws-project
Terraform project to provision AWS infrastructure with a VPC, two subnets, EC2 web servers, an Application Load Balancer, security groups, and an S3 bucket for scalable web hosting.
# Terraform AWS Web Infrastructure

This project provisions a simple, scalable, and fault-tolerant web application infrastructure on AWS using Terraform.

## Features

- **VPC and Subnets**: 
  - Creates a custom VPC with two subnets in different availability zones (`us-east-1a` and `us-east-1b`) for high availability.

- **EC2 Instances**: 
  - Deploys two EC2 instances as web servers using custom user data scripts.

- **Application Load Balancer**: 
  - Distributes traffic across EC2 instances with a health check mechanism.

- **Security Groups**: 
  - Configures rules to allow HTTP (port 80) and SSH (port 22) traffic.

- **S3 Bucket**: 
  - Provisions an S3 bucket for future use (e.g., asset storage or logging).

## Prerequisites

- Terraform installed on your local machine.
- AWS CLI configured with the necessary access keys.
- User data scripts (`userdata.sh` and `userdata1.sh`) ready in the project directory
