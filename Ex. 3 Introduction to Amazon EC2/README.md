# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**:VIGNESH KUMAR S
* **Register Number**: 212223060299
* **Date of Submission**: 12/03/26

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. Login to AWS Management Console

2.Open Amazon EC2 dashboard

3.Click on Launch Instance

4.Choose an AMI (Amazon Machine Image) such as Amazon Linux or Ubuntu

5.Select an instance type such as t2.micro

6.Configure instance details (network, number of instances, etc.)

7.Add storage and tags if required

8.Configure security group to allow SSH (port 22) or HTTP (port 80)

9.Create and download key pair (.pem file)

10.Click Launch Instance

11.Wait until instance state becomes running

12.Select the instance and click Connect

13.Connect using SSH command

14.Access the instance terminal

15.Go to monitoring tab to check CPU usage and status checks

16.Use CloudWatch to observe performance metrics

17.Stop the instance when not in use

18.Start the instance again when needed

19.Terminate the instance when it is no longer required

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1261" height="763" alt="image" src="https://github.com/user-attachments/assets/c1ccd531-c1e8-423d-a923-b9d519b1aed0" />


---

### Screenshot 2: SSH Connection to Instance

<img width="1269" height="834" alt="image" src="https://github.com/user-attachments/assets/6339eb6d-b779-4a27-ada8-9bd2c71998ad" />


---

### Screenshot 3: Instance Monitoring / Status

<img width="1262" height="828" alt="image" src="https://github.com/user-attachments/assets/f57482aa-b707-4397-8c80-8d4231963ba0" />

---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
