# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: VIGNESH KUMAR S
* **Register Number**:212223060299
* **Date of Submission**: 20/03/2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)


1. 1. Open AWS Management Console and go to EC2 service.

2. Click on “Launch Instance” and choose an operating system like Amazon Linux or Ubuntu.

3. Select instance type (t2.micro) and keep other settings as default.

4. Configure storage if required.

5. In security group, allow SSH (port 22) and database port (like 3306 for MySQL).

6. Launch the instance and download the key pair.

7. Connect to the EC2 instance using SSH from your system.

8. Update the system packages to the latest version.

9. Install a database management system such as MySQL.

10. Start the database service and enable it to run automatically.

11. Secure the database by setting root password and basic configuration.

12. Log in to the database server.

13. Create a new database.

14. Create a user and assign permissions to access the database.

15. Create a sample table in the database.

16. Insert some records into the table to test.

17. Configure database settings to allow remote access if needed.

18. Ensure the required port is open in the security group.

19. Test the database connection from another system or client.

20. Verify that data can be accessed successfully.



---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1333" height="907" alt="Screenshot 2026-03-20 102324" src="https://github.com/user-attachments/assets/9f72a32c-bbdc-45d5-8e8e-ec9665ee20c4" />


---

### Screenshot 2: Database Service Running

<img width="1919" height="1046" alt="image" src="https://github.com/user-attachments/assets/46c15788-082a-477e-bbb5-5262249b1cdd" />


---

### Screenshot 3: Sample Database and Table

<img width="1230" height="945" alt="Screenshot 2026-03-20 105041" src="https://github.com/user-attachments/assets/40e7b040-fad5-4778-bbf5-0360ede0a15d" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
