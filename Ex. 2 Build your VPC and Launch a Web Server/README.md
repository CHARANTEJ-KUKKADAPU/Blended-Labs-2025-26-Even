# Build Your VPC and Launch a Web Server (AWS) 

## Author

* **Name**: KUKKADAPU CHARAN TEJ
* **Register Number**: 212224040167
* **Date of Submission**: 27-02-2026

---

## Objective

The objective of this experiment is to understand how to design and configure a basic network infrastructure in AWS using a Virtual Private Cloud (VPC). This lab focuses on creating a VPC with a public subnet, configuring an Internet Gateway and route table, launching an EC2 instance, and hosting a simple web server that can be accessed over the internet.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity

---

## Tools Used

* AWS Management Console
* Amazon VPC
* Amazon EC2
* Internet Gateway
* Route Table
* Security Groups

---

## Tasks Performed

### Task 1: Create a VPC

Create a new Virtual Private Cloud (VPC) with a private IP address range. The VPC acts as a logically isolated network in AWS where all other resources will be deployed.

Students should create a VPC with an appropriate CIDR block (for example, 10.0.0.0/16) and assign a meaningful name.


### Task 2: Create a Public Subnet

Create a subnet inside the VPC to host public resources. Enable auto-assign public IPv4 so that instances launched in this subnet receive a public IP address.

The subnet should use a smaller CIDR range (for example, 10.0.1.0/24).


### Task 3: Create and Attach Internet Gateway

Create an Internet Gateway (IGW) and attach it to the VPC. This allows communication between resources in the VPC and the internet.


### Task 4: Configure Route Table

Create a route table and add a default route (0.0.0.0/0) pointing to the Internet Gateway. Associate this route table with the public subnet.

This step ensures that traffic from the subnet can reach the internet.


### Task 5: Create Security Group

Create a security group to act as a virtual firewall for the EC2 instance. Configure inbound rules to allow:

SSH on port 22

HTTP on port 80


### Task 6: Launch EC2 Instance

Launch an EC2 instance inside the public subnet using Amazon Linux 2 AMI and a suitable instance type (t2.micro).

Attach the previously created security group and key pair.


### Task 7: Configure Web Server

Install and start a web server (Apache HTTPD) on the EC2 instance using user data or manual commands.

Create a simple HTML page and verify that it can be accessed from a web browser using the public IP address of the instance.---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1.Create a VPC with a CIDR block (e.g., 10.0.0.0/16) and a public subnet (e.g., 10.0.1.0/24) with auto-assign public IP enabled.

2.Create and attach an Internet Gateway to the VPC to enable internet connectivity.

3.Configure a Route Table with a default route (0.0.0.0/0) pointing to the Internet Gateway and associate it with the public subnet.

4.Create a Security Group allowing inbound SSH (port 22) and HTTP (port 80), then launch an EC2 instance in the public subnet.

5.Install and start Apache on the EC2 instance, create a simple HTML page, and access it using the instance’s public IP to verify connectivity.

---

## Output Screenshots (Attach 3)

<img width="1919" height="898" alt="Screenshot 2026-02-27 083107" src="https://github.com/user-attachments/assets/144f08be-58ab-43ca-82f5-ee88d6abecf4" />

<img width="1903" height="814" alt="Screenshot 2026-02-27 083330" src="https://github.com/user-attachments/assets/93e5d7ef-1895-4b00-883c-5b5be8c69e7a" />




### Screenshot 1: VPC and Subnet Details

(Insert Screenshot Here)
<img width="1919" height="898" alt="Screenshot 2026-02-27 083107" src="https://github.com/user-attachments/assets/144f08be-58ab-43ca-82f5-ee88d6abecf4" />

---
<img width="1918" height="863" alt="Screenshot 2026-02-14 114753" src="https://github.com/user-attachments/assets/b89e870a-92ef-4f58-b99b-145d317fcf11" />

### Screenshot 2: EC2 Instance Running

(Insert Screenshot Here)

---
<img width="1919" height="872" alt="Screenshot 2026-02-14 115633" src="https://github.com/user-attachments/assets/10340a43-7a94-4d9f-95cb-0a90521396fd" />

### Screenshot 3: Web Server Output in Browser

(Insert Screenshot Here)
<img width="1919" height="855" alt="Screenshot 2026-02-26 105130" src="https://github.com/user-attachments/assets/04c2a8a9-e0fe-4839-82c6-6c37f706b59d" />

---<img width="1919" height="897" alt="Screenshot 2026-02-27 082318" src="https://github.com/user-attachments/assets/d746ce65-7aec-4167-a6c9-cc498d7601ef" />


## Result 

This experiment successfully demonstrated the creation of a custom VPC and deployment of a public-facing web server in AWS. By configuring networking components such as subnets, route tables, and security groups, and by launching an EC2 instance with a web server, the basic architecture of a cloud-hosted application was understood.
