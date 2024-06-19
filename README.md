Multi-Tier Architecture on AWS using Terraform

Deploy a scalable and resilient multi-tier architecture on AWS using Terraform.

🚀 Project Overview

This project allows us to deploy a highly available, scalable, and secure multi-tier architecture on Amazon Web Services (AWS) using Terraform. 

The architecture consists of the following three tiers:

Web Tier: This tier handles incoming user requests and can be horizontally scaled for increased capacity. It typically includes web servers and a load balancer for distributing traffic.

Application Tier: Application servers run our business logic and interact with the database tier. They can also be horizontally scaled to meet demand.

Database Tier: The database stores and manages our application data. In this architecture, we use Amazon RDS for a managed database service.

📌 Architecture Diagram
multi-tier-architecture

![278309947-14aeb752-ba87-4f51-87d5-bcf3000ee455](https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/assets/119873299/aef368e2-7f50-497f-abbe-85e0d17c4135)


🚦 Getting Started
Prerequisites
Before you get started, make sure you have the following prerequisites in place:

Terraform installed.

AWS IAM credentials configured.

Git for cloning the repository.

📋 Table of Contents

Features

Web Tier

Application Tier

Database Tier

Terraform Configuration

✨ Features

High Availability: The architecture is designed for fault tolerance and redundancy.

Scalability: Easily scale the web and application tiers to handle varying workloads.

Security: Security groups and network ACLs are configured to ensure a secure environment.

🌟 Web Tier

The Web Tier is the entry point for incoming user requests. It typically includes:

Load Balancer: Distributes traffic across multiple web servers.

Auto Scaling: Automatically adjusts the number of web servers based on traffic.

Security Groups: Controls incoming and outgoing traffic to the web servers.

Web Tier Configuration

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/alb-web-sg.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/alb-web.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/asg-web.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/alb-web-sg.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/asg-web-sg.tf


Application Tier

The Application Tier hosts the application servers responsible for running business logic and interacting with the database tier. 

Key components include:

Application Servers: These run your application code and can be horizontally scaled.

Load Balancer: Distributes traffic to the application servers.

Auto Scaling: Automatically adjusts the number of web servers based on traffic.

Security Groups: Controls incoming and outgoing traffic to the application servers.

Application Tier Configuration

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/lauch-template-app.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/alb-app.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/asg-app.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/alb-app-sg.tf

https://github.com/nasrisuhaira/multi-tier-architecture-using-terraform/blob/main/asg-app-sg.tf

Database Tier

The Database Tier stores and manages our application data. We use Amazon RDS for a managed database service. Key components include:

Amazon RDS: A managed database service for MySQL/PostgreSQL/SQL Server databases.

Security Groups: Control incoming and outgoing traffic to the database.

Database Tier Configuration



