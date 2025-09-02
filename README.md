# Terraform AWS Infrastructure

This project provisions a highly-available VPC and application infrastructure in AWS.

## Components
- VPC with public/private subnets across 2 AZs
- Internet Gateway & NAT Gateway
- Application Load Balancer
- Auto Scaling Group of EC2 instances
- PostgreSQL RDS instance
- Bastion Host for SSH access

## Prerequisites
- Terraform >= 1.0
- AWS CLI configured
- SSH key pair in AWS

## Usage
1. Copy `terraform.tfvars.example` to `terraform.tfvars` and fill values.
2. Run:
```bash
terraform init
terraform plan
terraform apply
```
3. Check outputs with:
```bash
terraform output
```

## Cleanup
```bash
terraform destroy
```
