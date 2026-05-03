# VPN Remote Access Lab (Cloud-Based)

## Overview
This project demonstrates how I simulated secure remote access using a cloud-hosted virtual machine and a VPN client. The goal was to validate how network traffic can be securely routed and how IP masking works in a controlled environment.

---

## What I Did

- Provisioned a Windows virtual machine in Microsoft Azure
- Enabled RDP (port 3389) for remote administrative access
- Installed and configured ProtonVPN on the virtual machine
- Connected to a remote VPN server (Netherlands)
- Verified IP address change using external IP lookup tools
- Simulated secure remote access from a cloud-based system

---

## Key Concepts Demonstrated

- Virtual Machine provisioning (Azure)
- Remote Desktop Protocol (RDP)
- VPN tunneling and encrypted traffic routing
- IP masking and geolocation changes
- Network security and remote access control

---

## Architecture Flow

Local Machine → Azure VM (RDP) → VPN Tunnel → Internet

---



## 1. Virtual Machine Provisioning (Azure)
<img src="https://github.com/user-attachments/assets/45776008-5107-411d-b353-0fb7b76d269b" width="519" />

Provisioned a Windows 11 Virtual Machine in Azure, configuring region, security settings (Trusted Launch, vTPM, Secure Boot), and enabling RDP access to simulate a secure remote environment for VPN connectivity testing.

### 2. VPN Connected (Remote Region)
<img src="https://github.com/user-attachments/assets/925af320-adcc-4cef-ba31-e9b8a9dc2d46"  width="800" />

Connected to a remote VPN server (Netherlands) from the Azure VM to simulate secure access from a different geographic location.



### 3. IP Address Verification
<img src="https://github.com/user-attachments/assets/2bdca7f1-cd67-4817-8e83-e416f14bd323" width="400"  />

---

## Notes

The public IP address initially resolved to a Microsoft-owned location (Washington), which may differ from the VM deployment region due to cloud provider IP allocation.

After connecting to the VPN, the IP address reflected the VPN server location (Netherlands), confirming successful VPN tunneling and traffic redirection.

---

## Outcome

This lab demonstrates how secure remote access can be implemented using VPN tunneling from a cloud-hosted system, helping protect network traffic and mask public IP addresses.

---

## Skills Gained

- Cloud Infrastructure (Azure)
- Networking Fundamentals
- Secure Remote Access
- VPN Configuration
