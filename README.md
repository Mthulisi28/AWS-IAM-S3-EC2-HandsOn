# AWS IAM, S3, EC2 Hands-On

This repository documents my hands-on exercises in AWS, focusing on:

- Creating IAM users and custom policies
- Restricting access with read-only S3 policies
- Fine-grained EC2 policies (specific instance type + region)
- Using IAM Policy Simulator to test permissions

## IAM Users

- DemoUser: read-only S3 access
- DemoUser1: fine-grained EC2 + S3 permissions

## Policies Included

- `DemoUser1S3ReadOnly.json`: Read-only access to a specific bucket, restricted to us-east-1
- `EC2MicroUSEast1.json`: EC2 access only for t2.micro in us-east-1

## Notes

- EC2 tests simulated due to Free Tier limitations
- Policy Simulator used for multi-service access testing
