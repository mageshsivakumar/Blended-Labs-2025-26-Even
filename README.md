# Lab 6 – Scale and Load Balance Your Architecture

## Author
* **Name**: MAGESH S
* **Register Number**: 212224040180
---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

- Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

- Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

- Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

- Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

- Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

- Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

- Students test the setup by generating traffic and observing automatic scaling and load distribution.

---


## Output Screenshots 

### Created LoadBalancer

<img width="1920" height="967" alt="image" src="https://github.com/user-attachments/assets/30bcd1d3-d987-4d74-8107-4e3a64acadc3" />

### Created LabConfig

<img width="1920" height="967" alt="image" src="https://github.com/user-attachments/assets/6da7573d-c81b-4621-91aa-e419be44821b" />

### Dynamic Scaling Policy created

<img width="1920" height="967" alt="image" src="https://github.com/user-attachments/assets/d09eafcc-42ca-43e2-8b6d-de4b226b63f7" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
