# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: KUKKADAPU CHARAN TEJ
* **Register Number**: 212224040167
* **Date of Submission**: 13-03-26

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

1.Explored Amazon EBS in the EC2 dashboard and reviewed different volume types like gp3, Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

2.Created a new EBS volume with the required size in the same Availability Zone as the EC2 instance.

3.Attached the created EBS volume to the running EC2 instance as an additional block device.

4.Connected to the EC2 instance using SSH, formatted the volume with the ext4 file system, and mounted it to a directory.

5.Stored sample files in the mounted volume and verified that the data remained available after rebooting the EC2 instance.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1919" height="974" alt="Screenshot 2026-03-13 150316" src="https://github.com/user-attachments/assets/a1864a42-0f27-4d88-a0d3-2006327adf49" />


---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1919" height="971" alt="Screenshot 2026-03-13 150522" src="https://github.com/user-attachments/assets/a4597946-5072-47c4-affa-9851c0eb9ac4" />


---

### Screenshot 3: Mounted Volume with Data

<img width="1919" height="1021" alt="Screenshot 2026-03-13 150903" src="https://github.com/user-attachments/assets/6f6d5dd6-ca9e-4db2-b066-802569cc8164" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
