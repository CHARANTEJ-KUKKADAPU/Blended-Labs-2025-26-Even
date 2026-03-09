# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: KUKKADAPU CHARAN TEJ
* **Register Number**: 212224040167
* **Date of Submission**:  27-02-26

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

1.Launch an Amazon EC2 instance named Web Server in the US East (N. Virginia) region using Amazon Linux 2023 AMI and t2.micro instance type.

2.Configure networking by selecting Lab VPC, creating a Web Server security group, and initially removing all inbound rules.

3.Enable termination protection, add a User Data script to install and start the Apache (httpd) web server, and launch the instance.

4.Monitor the instance using Status checks, Monitoring (CloudWatch metrics), System Log, and Instance Screenshot in the EC2 console.

5.Allow HTTP access by adding an inbound rule for port 80, then stop the instance to resize it to t2.small and increase the EBS volume from 8 GiB to 10 GiB, and start the instance again.

## Output Screenshots (Attach 3)

<img width="1919" height="927" alt="Screenshot 2026-02-27 084711" src="https://github.com/user-attachments/assets/c53a1714-33fb-4f6b-8e7f-a13edbca95ce" />
<img width="1919" height="975" alt="Screenshot 2026-02-27 083347" src="https://github.com/user-attachments/assets/9dc8e713-4f36-42b7-9031-dcf0a03870da" />

<img width="1919" height="878" alt="Screenshot 2026-02-27 084307" src="https://github.com/user-attachments/assets/19783a53-70c4-4b05-963a-64b358a04db8" />


### Screenshot 1: EC2 Dashboard / Instance List

<img width="1919" height="898" alt="Screenshot 2026-02-27 083107" src="https://github.com/user-attachments/assets/0a194b72-f9b8-4ecc-b574-1a6ad8d6430a" />


### Screenshot 2: SSH Connection to Instance
<img width="1919" height="975" alt="Screenshot 2026-02-27 083347" src="https://github.com/user-attachments/assets/60d4b1c4-dec4-4fd0-8df2-f2a508a4f5ce" />


### Screenshot 3: Instance Monitoring / Status

<img width="1919" height="927" alt="Screenshot 2026-02-27 084711" src="https://github.com/user-attachments/assets/74b9541e-6d65-4408-a758-0c031c42182d" />


## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
