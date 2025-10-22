# ☁ Cloud Internship - Task 2

## 🎯 Objective
To understand how cloud virtual machines (VMs) work by creating, configuring, and connecting to a cloud-based server instance using AWS EC2 (Free Tier).

---

## ⚙ VM Configuration
- *Cloud Provider:* AWS  
- *Instance Name:* cloud-task2  
- *Instance ID:* i-0f2f24063f901684  
- *Instance Type:* t2.micro (Free Tier Eligible)  
- *Operating System:* Ubuntu 22.04 LTS  
- *Region:* ap-east-1a (virginia)  
- *Public IPv4 Address:* 3.7.201.118  
- *Status:* Running (3/3 checks passed)

---

## 🧭 Steps Performed
1. Logged into the AWS Management Console.  
2. Opened *EC2 Dashboard → Launch Instance*.  
3. Selected *Ubuntu 22.04 LTS (Free Tier)* as the AMI.  
4. Chose *t2.micro* instance type.  
5. Created a new *key pair (cloud-task2-key.pem)*.  
6. Configured *Security Group* to allow:
   - SSH (Port 22) from my IP  
   - HTTP (Port 80)  
   - HTTPS (Port 443)
7. Launched the instance and waited until *Status = running*.
8. Connected using *EC2 Instance Connect (browser SSH)*.
9. Verified connection with commands:
   ```bash
   whoami
   uname -a
