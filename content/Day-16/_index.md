---
title: Capstone Project 
weight: 116
---

## System Architecture Capstone & Goals
1. Research and Development 
2. System Architecture and Design 
3. Technical Writing 
4. Logical Architecture 

## Logical Architecture Features 
1. Load Balancers Architecture (Web Front-End)
2. Virtual Machines with Packer Images 
3. Chef Server Configuration 
4. CI/CD using Jenkins  
5. CI/CD using GitLab
6. Firewall or DMZ Zones or VPC/VPN Access 
7. Database Redundancy
8. Docker Production Server Deployment  
9. External Network Operating System Builds
10. Intranet and Internet Access 
11. Role based access to Production, Developer, Testing Servers 
12. Load Balancers Architecture (Database) with one of the following
    1.  Google Firebase 
    2.  MySQL 
    3.  MongoDB

## Capstone: Website Architecture Design Logical Architecture
Create a fictious company name (and logo optionally). Add the logo or the first letter of the Company name to the document that will be the technical application design. Using [Draw.io](https://www.draw.io) or similar tool to design the following logical architecture for a website stored in AWS. Use icons for each component and remember the takeaways from the topics we covered on how to create a presentation. Add the logical design to the document once you have completed architecture. Below are the components you design should include: 

**Logical Architecture Components**
1. Web Server 
2. Application server failover  
3. IAM roles
4. Regions
5. Security groups
6. Databases redundancy 
7. Load balancers
8. S3 for static images 
9. Intranet access (internal webpages)
10. Internet access (public webpages) 
11. Firewalls & DMZ for public and private access 
12. VPN - employee only
13. Client Machine(s)

**Bonus** - Token based authentication for access to the companies’ network. What is it and why should companies use it?   

**Project: Logical Architecture for a Website Stored in AWS**
Create visual representation of the logical architecture and all the components. We are not expecting extensive knowledge on Amason that required VPC with subnets, route tables, internet gateway and NAT Gateway but a complete understanding of a web applications dataflow and design. Create a document that can answer the following questions.  

[Choosing an AWS database service](https://aws.amazon.com/getting-started/decision-guides/databases-on-aws-how-to-choose/)

## Resources 
1. [Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
2. [Amazon Machine Images](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html)
3. Front-End We & Mobile on AWS 
4. [Amazon Machine Images (AMI's)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html)
5. [Regions & Zones](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html) 
6. [Security in Amazon ec2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security.html)
7. [IAM Roles for Amazon ec2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-roles-for-amazon-ec2.html)
8. [Storage](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Storage.html)
9. [Amazon VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
10. [Relational Database User Guide](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html)
11. [Virtual Machine (VM) Redundancy](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/disaster-recovery-resiliency.html) 
12. [RDS Redundancy](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/disaster-recovery-resiliency.html)

## Platform Profile Questions
Create a document that answers the following questions
- Who is your target audience for the platform? 
- Which personas do you think where used to create the technical documentation? 
- What are some of the key features or capabilities of this solution offered to these audiences?
- Web purpose does the web server have in the design?
- What is an EC2 instance?
- What conditions would qualify an S3 storage solution vs Database storage? 
- What is the role of the database?  
- What are the necessary Identity Access Management (IAM) roles for database access? 
- Why do we need a load balancer? 
- Why are Security Groups important? 
- What is a Virtual Private Network and why would you use one?
- What is a RSA Token and how is it used 
- What is a firewall and what purpose does it have in an organization? 
  - How is access filtered by firewalls? 


