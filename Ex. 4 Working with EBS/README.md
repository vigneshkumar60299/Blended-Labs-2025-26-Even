# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: VIGNESHKUMAR S
* **Register Number**: 212223060299
* **Date of Submission**: 13/03/2026

---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)



1. 1. Login to AWS Management Console

2. Open Amazon EC2 dashboard

3. Launch a new EC2 instance or select an existing one

4. Navigate to “Volumes” under Elastic Block Store

5. Click on “Create Volume”

6. Choose volume type, size, and availability zone (same as the instance)

7. Click “Create Volume”

8. Select the created volume and click “Attach Volume”

9. Choose the EC2 instance and assign a device name

10. Connect to the EC2 instance

11. Check that the new volume is available in the system

12. Format the attached volume with a file system

13. Create a directory for mounting the volume

14. Mount the volume to the created directory

15. Verify that the volume is successfully mounted

16. Store some data in the mounted volume

17. Reboot the EC2 instance

18. Reconnect to the instance after reboot

19. Check whether the volume is still attached

20. Mount the volume again if it is not mounted automatically

21. Verify that the previously stored data is still available

22. Confirm that data persists even after reboot


---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="593" height="607" alt="image" src="https://github.com/user-attachments/assets/8183f511-5d4a-4f13-93f0-b96d400a6571" />

---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/f4790a21-4882-4456-b2ee-d7ed3ddb3ad1" />

<img width="1919" height="807" alt="image" src="https://github.com/user-attachments/assets/2858aea3-abd7-447d-a490-a84d4f6f7464" />


---

### Screenshot 3: Mounted Volume with Data

<img width="1918" height="1039" alt="image" src="https://github.com/user-attachments/assets/81355c31-dbef-4a2f-8566-a6e2ffaf9880" />

<img width="1908" height="1032" alt="image" src="https://github.com/user-attachments/assets/d4b0b695-096d-4c81-8deb-da9c51fc2fe9" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
