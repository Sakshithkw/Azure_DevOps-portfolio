# Assignment 2: Availability Sets & User Data Scripts

## Overview
Create Availability Sets for high availability, add user data scripts for automation, manage VM properties.

---

## ✅ Tasks Completed

### Step 1: Created Resource Group
- Name: myRG
- Region: Central India

[Screenshot](01-availability-set.png)

---

### Step 2: Created Availability Set
- Name: myAS
- Fault Domains: 2
- Update Domains: 5

**Purpose**: Distribute VMs across physical servers

[Screenshot](02-vm-creation.png)

---

### Step 3: Created VM in Availability Set
- Name: myvm
- OS: Ubuntu 22.04 LTS
- Availability Set: myAS
- Size: Standard_B1s → B2als_v2

[Screenshot](02-vm-creation_completion.png)

---

### Step 4: Added User Data Script
\`\`\`bash
#!/bin/bash
useradd jay
useradd sakshi
\`\`\`

Automatically creates users at startup.

[Screenshot](03-script-verification.png)

---

### Step 5: Verified Script
Users successfully created:

\`\`\`bash
jay:x:1001:1001::/home/jay:/bin/bash
sakshi:x:1002:1002::/home/sakshi:/bin/bash
\`\`\`

---

### Step 6: Reset Password
Reset azureuser password via Azure Portal.

[Screenshot](04-password-reset.png)

---

### Step 7: Changed Instance Size
Resized from B1s to B2als_v2 (2 vCPUs, 4 GiB RAM).

[Screenshot](05-instance-size-change.png)

---

## 🛠 Commands Used

\`\`\`bash
# SSH login
ssh -i key.pem azureuser@<IP>

# Verify users
cat /etc/passwd | grep -E 'jay|sakshi'

# Check VM info
hostnamectl
\`\`\`

---

## 📊 Learning Outcomes

✅ Availability Sets for high availability  
✅ Fault Domains & Update Domains  
✅ User data script automation  
✅ VM password reset  
✅ Instance resizing/vertical scaling  

---

[← Back to Portfolio](../README.md)
