# 🔒 Secure AWS Three-Tier Web Application

This project demonstrates how to deploy a **secure and scalable three-tier architecture** on AWS.  
The design separates the web, application, and database layers across public and private subnets for maximum security.

---

## 🏗 Architecture Overview
![Architecture Diagram: <img width="1536" height="1024" alt="VPC → Public_OR_Private Subnets → ALB → EC2 → RDS" src="https://github.com/user-attachments/assets/3f25ac3c-48cd-46f4-91cd-3ed57ecd14f4" />


### Layers
- **Presentation Layer (Web Tier):** Amazon EC2 behind an Application Load Balancer (ALB).  
- **Application Layer:** EC2 instances in private subnets handle business logic.  
- **Data Layer:** Amazon RDS database in private subnets with restricted access.

---

## ⚙️ Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/PitchGates/secure-aws-three-tier-wep-app.git
   cd secure-aws-three-tier-wep-app
2. Create a VPC with public and private subnets.
3. Deploy EC2 instances for each tier using CloudFormation or Terraform.
4. Configure ALB in public subnet to forward traffic to private EC2s.
5. Deploy RDS in private subnet; allow access only from App Tier.
6. Secure all layers using Security Groups and IAM Roles.

## Tools and Services Used
1. Amazon VPC
2. Elastic Load Balancer (ALB)
3. Amazon EC2
4. Amazon RDS
5. IAM Roles and Policies
6. Terraform / CloudFormation

## Security Highlights
- Private subnets for sensitive workloads.
- Bastion Host for SSH access to private instances.
- IAM least-privilege roles.
- Encrypted database connections and at-rest data.

## Deployment Options
Terraform: Use main.tf for IaC deployment.
CloudFormation: Use provided YAML template for stack creation.
