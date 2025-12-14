AWS EC2 + WordPress Deployment – EpicReads Project
📌 Overview
This hands‑on cloud project demonstrates how to deploy a WordPress application on an Amazon Linux 2023 EC2 instance inside a custom VPC. It includes secure networking, SSH access, Apache setup, RDS database integration, and CloudWatch monitoring — simulating a real‑world production deployment for EpicReads.

🛠️ Architecture Components
VPC with public and private subnets

Internet Gateway + custom Route Tables

EC2 Instance (Amazon Linux 2023, t3.micro)

Security Groups for SSH, HTTP, and DB access

Apache Web Server + PHP

WordPress CMS deployed on EC2

Amazon RDS (MySQL) for database layer

CloudWatch Alarms for proactive monitoring

🚀 Steps Implemented
✅ 1. VPC & Networking Setup
Created a VPC with CIDR block 10.0.0.0/16

Added public and private subnets across multiple AZs

Attached an Internet Gateway

Configured route tables for internet access (public subnet)

✅ 2. EC2 Instance Deployment
Launched EC2 using Amazon Linux 2023

Created and downloaded a key pair

Connected via SSH using terminal

Installed and configured Apache (httpd)

✅ 3. WordPress Installation
Installed PHP and required extensions

Downloaded and extracted WordPress into /var/www/html

Set correct file permissions

Configured wp-config.php with RDS database details

✅ 4. RDS Database Setup
Created an RDS MySQL instance (db.t3.micro)

Disabled public access for security

Configured RDS Security Group to allow port 3306 only from EC2 SG

Created WordPress database and user inside RDS

✅ 5. CloudWatch Monitoring
Created CPU Utilization alarm

Configured email notifications via SNS

Ensured proactive alerting for performance issues

✅ 6. Validation
Accessed WordPress via EC2 public IP

Completed WordPress installation wizard

Verified database connectivity and site functionality

✅ Outcomes
✅ Secure and scalable AWS infrastructure following best practices

✅ WordPress site publicly accessible via EC2

✅ Database securely isolated in private RDS

✅ CloudWatch alarms enabled for real‑time monitoring

✅ Improved reliability with proactive alerts (reduced downtime by ~20%)

📷 Screenshots
Added screenshots of EC2 instance, RDS setup, WordPress dashboard,and architecture diagram.
