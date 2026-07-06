# Assignment 3: Custom VM Images

## Objective
Create a custom VM image in Azure from a configured virtual machine and use it to deploy new VMs.

## Steps Performed
1. Created and configured a base VM with required software/settings
2. Generalized the VM using sysprep (Windows) / waagent -deprovision (Linux)
3. Stopped/deallocated the VM
4. Captured the VM as a custom image via Azure Portal
5. Deployed a new VM using the custom image

## Screenshots
![Step 1](./screenshot1.png)
![Step 2](./screenshot2.png)

## Key Learnings
- Custom images help standardize and speed up VM deployment
- Generalizing a VM removes machine-specific info before imaging

## Tools/Services Used
Azure Portal, Azure VM, Custom Images
