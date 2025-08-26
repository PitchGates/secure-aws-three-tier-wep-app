# Secure AWS Three-Tier Web Application

## 📌 Project Status
🚧 **Active Development** - This project is currently in the planning and initial implementation phase. Last updated: 2025-08-26.

## 🎯 Objective
To build a secure, highly available three-tier web application on AWS that demonstrates core cloud architecture and security principles.

## 🏗️ Planned Architecture
-   **Networking:** Multi-AZ VPC with public and private subnets, Internet Gateway, NAT Gateway.
-   **Compute:** EC2 instances in an Auto Scaling Group for the web tier.
-   **Load Balancing:** Application Load Balancer (ALB) to distribute traffic.
-   **Database:** Amazon RDS (PostgreSQL) in private subnets for the data tier.
-   **Security:** Security Groups, NACLs, and AWS WAF rules.

## 🔧 Tech Stack
-   **Cloud Provider:** AWS
-   **Infrastructure as Code:** Terraform / AWS CloudFormation
-   **Scripting:** Python (Boto3) / Bash
-   **Monitoring:** AWS CloudWatch

## ✅ Next Steps
-   [ ] Draft initial Terraform configuration for the VPC.
-   [ ] Configure public and private subnets and route tables.
-   [ ] Deploy and configure the Application Load Balancer.
-   [ ] Implement security best practices for IAM and S3.

## 📂 Repository Structure
