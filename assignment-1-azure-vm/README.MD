# Assignment 1: Azure VM Deployment & Web Hosting

## Overview
Deploy a Linux virtual machine on Azure, install Apache web server, and host a custom website.

---

## ✅ Tasks Completed

### Step 1: Created Resource Group
- Name: RG-Practice-VM
- Region: Central India

[Screenshot](01-resource-group-created.png)

---

### Step 2: Created Virtual Machine
- Name: PracticeVM
- OS: Ubuntu 22.04 LTS
- Public IP: Enabled
- NSG Rules: SSH (22) + HTTP (80)

[Screenshot](02-vm-overview.png)

---

### Step 3: SSH Connection
Connected via SSH using PEM key authentication.

[Screenshot](03-ssh-login-success.png)

---

### Step 4: Installed Apache
Installed and configured Apache2 web server.

[Screenshot](04-apache-status.png)

---

### Step 5: Created Website
Deployed custom HTML website.

[Screenshot](05-html-code.png)

---

### Step 6: Website Live
Website accessible via public IP.

[Screenshot](06-website-live.png)

---

## 🛠 Commands Used

\`\`\`bash
# Update system
sudo apt update && sudo apt upgrade -y

# Install Apache
sudo apt install apache2 -y

# Start Apache
sudo systemctl start apache2
sudo systemctl enable apache2

# Create website
cd /var/www/html
sudo nano index.html
\`\`\`

---

## 📊 Learning Outcomes

✅ Azure Portal navigation  
✅ VM provisioning  
✅ SSH authentication  
✅ Linux package management  
✅ Web server configuration  

---

[← Back to Portfolio](../README.md)
