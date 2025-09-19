# AWS IAM, S3, EC2 Hands-On

This repository documents my hands-on exercises in AWS, focusing on **Identity and Access Management (IAM)**, **Amazon S3**, and **Amazon EC2**.  

## 📌 What I Practiced
- Creating IAM users with different levels of access
- Writing **custom IAM policies**
- Restricting access by **region** and **resource type**
- Using **IAM Policy Simulator** to test permissions before applying
- Enforcing **least privilege** with S3 read-only and EC2 restrictions

## 👤 IAM Users
- **DemoUser** → S3 access (read-only)  
- **DemoUser1** → Fine-grained EC2 + S3 access  

## 📜 Policies
1. **S3 Read-Only with Region Restriction**  
   - File: `IAM/DemoUser1S3ReadOnly.json`  
   - Grants read-only S3 access, restricted to `us-east-1`.  

2. **EC2 Restriction Policy**  
   - File: `IAM/EC2MicroUSEast1.json`  
   - Allows launching EC2 instances but only a specific type (`t2.micro`) in `us-east-1`.  
   - Tested via Policy Simulator (EC2 blocked in free tier).  

## 🪣 S3
- Created a bucket `demouser1-test-bucket`  
- Attached policy restricting **read-only access**  

## 🖥️ EC2
- Created a **restricted policy** for EC2 instance launch.  
- Verified using **Policy Simulator**.  

## 📖 Notes
- EC2 tests simulated due to Free Tier limitations  
- Hands-on reinforced key AWS concepts:
  - IAM users, policies, and permissions boundaries
  - Region-specific access control
  - Testing before deploying policies

---

### 🔗 Next Steps
I will continue adding more exercises as I progress through **AWS Cloud Practitioner** and **Solutions Architect Associate** preparation.
