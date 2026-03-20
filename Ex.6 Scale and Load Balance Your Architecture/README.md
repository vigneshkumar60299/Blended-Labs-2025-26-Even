# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : VIGNESH KUMAR S   Reg no : 212223060299  yours   Date :20/03/26

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

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

Describe step-by-step how you performed this experiment in your own words.

1.First, I logged into the Amazon Web Services console.

2.Then I went to the EC2 service and launched a new instance using Amazon Linux.

3.I selected a small instance type (t2.micro) and allowed HTTP access in the security group.

4.After launching, I connected to the instance and installed a web server (Apache).

5.I created a simple web page so that I can identify the instance during testing.

6.Then I created an AMI from this instance so it can be reused later.

7.Next, I created a Launch Template using this AMI with required configurations.

8.After that, I created a Target Group and set HTTP protocol with health checks.

9.Then I went to Elastic Load Balancing and created an Application Load Balancer.

10.I selected multiple Availability Zones to make the system highly available.

11.I attached the Target Group to the Load Balancer.

12.Next, I created an Auto Scaling Group using the Launch Template.

13.I selected multiple Availability Zones again and attached the Load Balancer.

14.I set the minimum, desired, and maximum number of instances.

15.Then I configured scaling policies based on CPU usage (for example, scale when CPU is high).

16.After creating everything, I tested the Load Balancer by opening its DNS in a browser and refreshing multiple times.

17.I observed that different instances handled the requests.

18.Then I generated more traffic to check Auto Scaling, and new instances were created automatically.

19.I also stopped one instance manually to test fault tolerance, and a new instance was launched automatically.

20.Finally, I monitored everything using Amazon CloudWatch.

---

## Output Screenshots 


<img width="1334" height="911" alt="Screenshot 2026-03-20 084148" src="https://github.com/user-attachments/assets/5f946bec-1105-42bf-9163-019cb1471d92" />

<img width="1342" height="863" alt="Screenshot 2026-03-20 085254" src="https://github.com/user-attachments/assets/732f5bbc-9d5e-4770-9839-d7f4796b469a" />

<img width="1336" height="941" alt="Screenshot 2026-03-20 090554" src="https://github.com/user-attachments/assets/00e4a58b-da0c-4f7f-997d-80e2376fb224" />

<img width="1335" height="889" alt="Screenshot 2026-03-20 092950" src="https://github.com/user-attachments/assets/64848780-501c-423e-a064-f6ac0cb293a9" />










---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
