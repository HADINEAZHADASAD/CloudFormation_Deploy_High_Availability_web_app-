# CloudFormation_Deploy_High_Availability_web_app-

In the Udagram project, I utilized CloudFormation to deploy highly available web servers for a web application. The deployment process involves creating and configuring the necessary infrastructure components and deploying the application itself. The script follows a sequential order, starting with the networking components, then proceeding to the server setup, security roles, and software installation.

By utilizing CloudFormation, the entire deployment process can be automated and easily reproducible. This approach ensures consistency and reduces manual configuration errors. Here is an overview of the deployment script:

Networking Components:

Creation of Virtual Private Cloud (VPC)
Configuration of subnets across multiple availability zones
Configuration of an internet gateway for external connectivity
Configuration of route tables and associations
Server Setup:

Creation of Auto Scaling Groups (ASG) for high availability
Configuration of load balancers to distribute traffic across instances
Launch configuration for server instances
Configuration of instance security groups for inbound and outbound traffic rules
Configuration of health checks for load balancers
Security Roles:

Creation of IAM roles and policies for EC2 instances
Configuration of IAM roles and policies for load balancers
Assignment of appropriate permissions to the roles
Software Deployment:

Configuration of user data scripts for EC2 instances to install and configure required software (e.g., web servers, database, etc.)
Deployment of the Udagram application code to the instances
