# Brainwave Matrix Intern - E-Commerce Website Deployment

This repository contains the code for a **static e-commerce website** deployed on AWS as part of the Brainwave Matrix Solutions internship program.

## 🌟 Project Overview
- A simple **HTML/CSS-based e-commerce website**.
- Hosted on **AWS EC2** (with Apache or Nginx).
- Includes **images, styles, and basic functionality**.
- Part of the **Brainwave Matrix Internship Program**.

## 🚀 Deployment Steps
### **1. Setting Up the Project**
1. Clone this repository:
   ```sh
   git clone https://github.com/your-username/Brainwave_Matrix_Intern.git
   ```
2. Navigate to the project folder:
   ```sh
   cd Brainwave_Matrix_Intern
   ```
3. Ensure all files (`index.html`, `style.css`, `images/`) are present.

### **2. Hosting on AWS EC2**
#### **Step 1: Launch an EC2 Instance**
1. Go to **AWS Console** → Navigate to **EC2**.
2. Click **Launch Instance**.
3. **Choose Amazon Linux 2 or Ubuntu as the AMI**.
4. **Select Instance Type:** t2.micro (Free Tier eligible).
5. **Configure Security Group:** Allow **HTTP (Port 80)** and **SSH (Port 22)**.
6. **Create/Select a Key Pair** → **Launch the Instance**.

#### **Step 2: Connect to the EC2 Instance**
```sh
ssh -i your-key.pem ec2-user@your-ec2-public-ip
```
_(For Ubuntu, use `ubuntu@your-ec2-public-ip`)_.

#### **Step 3: Install Apache/Nginx**
##### **Apache (Recommended)**
```sh
sudo apt update -y
sudo apt install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
``

#### **Step 5: Access Your Website**
- Open a browser and go to:
  ```
  http://your-ec2-public-ip
  ```
- Your static website should be visible! 🎉


---

### 🎯 **Internship Goal**
This project is a demonstration of deploying a static website on **AWS EC2 instance**. By completing this, we enhance our understanding of **cloud hosting, deployment automation, and best DevOps practices**.

---

🔹 **Created by:** Ranjit H Dhole  
🔹 **Intern at:** Brainwave Matrix Solutions Pvt Ltd  
🔹 **Date:** March 2025
