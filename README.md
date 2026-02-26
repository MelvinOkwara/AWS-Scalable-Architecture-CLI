# AWS Scalable Architecture via CLI

This project demonstrates the creation of a highly available, scalable web infrastructure using the AWS CLI. It includes a VPC, Auto Scaling Group, Application Load Balancer, and CloudFront Distribution.

## Project Steps

### 1. Network Foundation (VPC & Subnets)
Fetching the Default VPC and identifying two Subnets in different Availability Zones for High Availability.
![VPC Setup](./1-vpc-subnets.png)

### 2. Security Configuration
Creating Security Groups for the Load Balancer (allowing HTTP 80) and the EC2 Instances.
![Security Groups](./2-security-groups.png)

### 3. Instance Bootstrapping
Writing the `userdata.sh` script to automate the installation of Apache and the creation of a dynamic landing page.
![User Data Script](./3-userdata.png)

### 4. Launch Template
Defining the EC2 configuration, including the Amazon Linux AMI, Instance Type, and the base64-encoded UserData.
![Launch Template](./4-launch-template.png)

### 5. Target Group Setup
Creating the Target Group to manage health checks and traffic routing for the EC2 instances.
![Target Group](./5-target-group.png)

### 6. Auto Scaling Group (ASG)
Deploying the ASG across multiple subnets to ensure the application scales automatically based on demand.
![Auto Scaling Group](./7-asg-creation.png)

### 7. Scaling Policies
Implementing a Target Tracking Scaling Policy based on Average CPU Utilization (50%).
![Scaling Policy](./8-scaling-policy.png)

### 8. Content Delivery (CloudFront)
Configuring CloudFront to cache content and reduce latency for global users.
![CloudFront](./9-cloudfront-config.png)

### 9. Final Verification
Accessing the application via the CloudFront URL. The page displays the unique Instance ID, proving the Load Balancer is distributing traffic.
![Final Output](./10-final-output.png)
