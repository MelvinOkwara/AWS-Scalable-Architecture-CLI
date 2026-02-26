# AWS Scalable Architecture via CLI

This project demonstrates a highly available, scalable web infrastructure built using the AWS CLI.

## Project Steps

### 1. Network Foundation (VPC & Subnets)
![VPC Setup](./01-vpc-subnet-identification.png)

### 2. Security Configuration
![Security Groups](./02-security-groups-creation.png)

### 3. Instance Bootstrapping
![User Data Script](./03-web-server-provisioning-script.png)

### 4. Launch Template
![Launch Template](./04-ec2-launch-template.png)

### 5. Target Group Setup
![Target Group](./05-target-group-arn-setup.png)

### 6. Load Balancer Setup
![Load Balancer](./06-application-load-balancer-creation.png)

### 7. Auto Scaling Group (ASG)
![Auto Scaling Group](./07-auto-scaling-group-initialization.png)

### 8. Scaling Policies
![Scaling Policy](./08-cpu-scaling-policy-configuration.png)

### 9. Content Delivery (CloudFront)
![CloudFront](./09-cloudfront-global-cdn-deployment.png)

### 10. Final Verification
![Final Output](./10-live-verification-cdn-url.png)