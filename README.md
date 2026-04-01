# Hosting-a-Website-on-Azure-Virtual-Machine-Nginx-Deployment-
A hands-on cloud infrastructure project demonstrating VM provisioning, secure access, and web server deployment using Microsoft Azure.
 Overview

This project showcases the deployment of a Linux-based virtual machine on Microsoft Azure, followed by the installation and configuration of an Nginx web server to host a live website accessible via a public IP address.

It reflects foundational skills in cloud infrastructure provisioning, remote server management, and web hosting—key competencies in Cloud and DevOps engineering.

 Objectives:
 
Provision a Linux Virtual Machine in Azure

Configure networking and public access

Establish secure SSH connectivity

Install and configure Nginx

Deploy and verify a live web server

Tech Stack:

Category	Technology

Cloud Platform	Microsoft Azure

Compute	Azure Virtual Machine (Linux)

Access	SSH (PowerShell / MobaXterm)

Web Server	Nginx

OS Package Manager	APT

 Deployment Workflow:
 
1️⃣ Provision Virtual Machine

Navigate to Azure Portal

Create a new Virtual Machine

Configure:

Region & Resource Group

Image (Ubuntu Linux)

Authentication (Username & Password/SSH)

Configure networking (ensure port 80 (HTTP) is open)

Validate and deploy:

2️⃣ Connect via SSH

Option A: PowerShell

ssh username@public-ip

Option B: MobaXterm

Create new SSH session

Input:


Public IP

Username

Authenticate to access VM:

3️⃣ Install & Configure Nginx

# Update system
sudo apt update && sudo apt upgrade -y

# Install Nginx
sudo apt install nginx -y

# Start and enable service
sudo systemctl start nginx
sudo systemctl enable nginx

4️⃣ Verify Deployment
Open browser

Enter: http://<your-public-ip>

Confirm Nginx default page is displayed

Key Outcomes

✔️ Successfully deployed a cloud-based VM

✔️ Established secure remote access via SSH

✔️ Installed and configured Nginx web server

✔️ Hosted a live web page accessible over the internet
