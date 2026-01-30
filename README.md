Secure EC2 Web Server

Overview
This project demonstrates how to deploy and secure a basic web server using Amazon EC2. The goal was to launch a cost-effective compute instance, configure network security, and apply IAM best practices while serving a simple web page.

AWS Services Used
- Amazon EC2
- IAM
- Security Groups
- Amazon Linux 2
- Apache (httpd)

Implementation Summary

- Launched an Amazon Linux 2 EC2 instance
- Selected a low-cost instance type (t2.micro)
- Created a Security Group allowing:
  - HTTP (port 80) from the public internet
  - SSH (port 22) restricted to my IP address
- Attached an IAM role using least-privilege permissions
- Installed and configured Apache via user data
- Deployed a simple HTML page to verify functionality

Security Considerations
  - SSH access restricted to a single IP address
  - IAM role used instead of hardcoded credentials
  - Security Groups used as a virtual firewall

Cost Considerations
  - Used AWS Free Tier–eligible resources
  - No load balancers or autoscaling to minimize cost
  - Designed for simplicity and learning purposes

Key Takeaways
  - Gained hands-on experience launching and configuring EC2 instances
  - Applied network security using Security Groups
  - Used IAM roles to follow AWS security best practices
  - Deployed a functional web server without unnecessary complexity

Possible Future Improvements
  - Add Auto Scaling and Load Balancer
  - Enable monitoring with CloudWatch
  - Automate deployment using Terraform or CloudFormation

More of my work on my portfolio page! https://github.com/JakeNS-Cloud/JakeNS-Portfolio 
