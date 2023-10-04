**Components Answer Key**
Web server: The web server is responsible for serving the website's HTML, CSS, and JavaScript files to users.
IAM roles: IAM roles are used to grant user permissions to access and manage AWS resources.
Regions: AWS regions are isolated locations around the world where AWS infrastructure is hosted.
Billing: AWS billing provides a detailed overview of your AWS usage and costs.
Security groups: Security groups act as a firewall for your AWS resources, controlling incoming and outgoing traffic.
Databases: AWS offers a variety of database services, including relational databases, NoSQL databases, and in-memory databases.
Load balancers: Load balancers distribute traffic across multiple instances of a resource, such as web servers or database servers.

The following is a logical architecture for a website stored in AWS:

The web server is hosted in an AWS EC2 instance.
The IAM role for the web server has the permissions necessary to access the website's files and resources.
The website's files are stored in an Amazon S3 bucket.
The Amazon S3 bucket is configured to deliver the static files to the web server using CloudFront.
The database server is hosted in an AWS RDS instance.
The IAM role for the database server has the permissions necessary to access the database.
The web server and database server are located in the same AWS region.
A load balancer is used to distribute traffic between the web servers.
A security group is used to control access to the web servers and database server.

Explanation of Components:

- Web server: The web server is responsible for serving the website's HTML, CSS, and JavaScript files to users. The web server can be hosted on an AWS EC2 instance, or you can use a managed web hosting service like AWS Elastic Beanstalk.
- IAM roles: IAM roles are used to grant user permissions to access and manage AWS resources. For example, you can create an IAM role for the web server that has the permissions necessary to access the website's files and resources.
- Regions: AWS regions are isolated locations around the world where AWS infrastructure is hosted. When you create an AWS resource, you must choose a region. You can choose to place your resources in the same region, or you can distribute them across multiple - regions.
- Billing: AWS billing provides a detailed overview of your AWS usage and costs. You can use AWS billing to track your costs and optimize your AWS usage.
- Security groups: Security groups act as a firewall for your AWS resources, controlling incoming and outgoing traffic. For example, you can create a security group for the web server that allows inbound traffic from all sources on port 80.
- Databases: AWS offers a variety of database services, including relational databases, NoSQL databases, and in-memory databases. For example, you can use Amazon RDS to host a relational database like MySQL or PostgreSQL.
- Load balancers: Load balancers distribute traffic across multiple instances of a resource, such as web servers or database servers. For example, you can use an AWS load balancer to distribute traffic across multiple web servers.
Benefits of Using AWS for Your Website:

The benefits to using AWS 
Scalability: AWS is highly scalable, so you can easily scale your website up or down as needed.
Reliability: AWS is very reliable, with a high uptime percentage.
Security: AWS offers a variety of security features to help protect your website from attacks.
Cost-effectiveness: AWS is very cost-effective, and you only pay for the resources that you use.
Availability: With AWS availability zones, if one zone goes offline, another will take its place without any downtime.
Availability: With AWS availability zones (AZs), there will be no downtime if one AZ fails.
Flexibility: You have many options when it comes to choosing what services fit best for your needs.
AWS Global Infrastructure: AWS operates over more than 100+ data centers across multiple geographic areas. This allows you to deploy applications closer to
Elasticity: If demand changes over time, AWS allows you to add more instances without having to worry about scaling back.
