<div align="center">

  # 🛡️ Cybersecurity & Ethical Hacking Lab

**Designing a secure virtual environment for hands-on security testing, network analysis, and ethical hacking experiments**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-CyberSecurity-8B0000?style=flat-square&labelColor=111111&logo=hackthebox&logoColor=white" />
  <img src="https://img.shields.io/badge/Hypervisor-VirtualBox%207.0-0070C0?style=flat-square&labelColor=111111&logo=virtualbox&logoColor=white" />
  <img src="https://img.shields.io/badge/OS-Kali%20Linux%202026.3-557C94?style=flat-square&labelColor=111111&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-Linux-FCC624?style=flat-square&labelColor=111111&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-238F89?style=flat-square&labelColor=111111&logo=cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/Focus-Penetration%20Testing-C00000?style=flat-square&labelColor=111111&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Technology-Virtualization-6A5ACD?style=flat-square&labelColor=111111" />
  <img src="https://img.shields.io/badge/Tools-Network%20Analysis-238F89?style=flat-square&labelColor=111111" />
  <img src="https://img.shields.io/badge/Practice-Ethical%20Hacking-E87500?style=flat-square&labelColor=111111" />
  <img src="https://img.shields.io/badge/Lab-Environment-404040?style=flat-square&labelColor=8B0000" />
     <img src="https://img.shields.io/badge/Jahid%20Hassan-C00000?style=flat-square" />
</p>

---

# 📌 About This Project

This project involves building a dedicated virtual lab for cybersecurity research and ethical penetration testing using Oracle VirtualBox and Kali Linux.
The goal is to establish an isolated and manageable testing environment for exploring security tools, performing network discovery, conducting reconnaissance, identifying potential vulnerabilities, and practicing various security assessment techniques.
A private virtual network is used to maintain separation from external systems while allowing future expansion with additional virtual machines that can serve as controlled targets for authorized penetration-testing exercises.

# 🎯 Project Goals & Objectives

This project aims to establish a secure and isolated virtual cybersecurity environment by completing the following tasks:  

     
- 🖥️ Install and configure Oracle VirtualBox as the virtualization platform.   
- 🐉 Set up Kali Linux as a guest virtual machine.     
- 🌐 Create and configure a dedicated NAT Network for the lab environment.     
- 🔗 Establish stable network connectivity between virtual machines.      
- 📍 Assign a static IP address to the Kali Linux virtual machine.      
- 🔍 Verify network connectivity, default gateway access, and DNS resolution.      
- 💾 Create a baseline virtual machine snapshot for backup and recovery.         
- 📝 Document the installation, configuration, and verification procedures.        
- 🚀 Prepare the lab infrastructure for future penetration testing and cybersecurity projects.

---


# 🛡️ Lab Purpose & Applications

The purpose of this lab is to provide a dedicated, isolated, and secure environment for developing practical cybersecurity skills and performing authorized security assessments.

The environment can be utilized for a variety of hands-on security exercises, including:

- **🔎 Network Reconnaissance –** Discovering hosts and gathering network information.   
- **🌐 Port Scanning –** Identifying open ports and running network services.  
- **🛠️ Vulnerability Assessment –** Detecting and analyzing potential security weaknesses.  
- **📡 Packet Analysis –** Capturing and inspecting network traffic.  
- **🔐 Web Security Testing –** Exploring common web application security issues.  
- **💻 Exploitation Practice –** Learning exploitation techniques in controlled lab scenarios.  
- **⚙️ Security Tool Experimentation –** Installing, configuring, and testing various cybersecurity tools.


**⚠️Disclaimer:** All activities are intended for educational purposes and authorized testing within the isolated lab environment.

---

## 🏗️ Lab Architecture

![image alt](https://github.com/jahidhsn-rng/networkwalks-B084D-week1-cybersecurity-lab-setup/blob/c7af2cf9e1b6e044277d67ac75d24fe9891a945a/vm%20box.PNG)


Additional virtual machines can be integrated into the existing isolated network in future projects to expand the lab environment and support more advanced cybersecurity testing scenarios.

---

  
## ⚡ Lab Configuration

| 🔹 Component | 🔸 Configuration |
|:---|:---|
| 💻 Host OS | Windows 10 home |
| 🧠 Host RAM | 16 GB |
| 🚀 Processor | Intel Core i5 |
| 🖥️ Hypervisor | VirtualBox 7.0 |
| 🐉 Security OS | Kali Linux 2026.3 |
| 💾 Kali RAM | 2048 MB |
| 🌐 Virtual Network | NAT Network |
| 📡 Network Address | `10.0.0.0/24` |
| 🎯 Kali IP Address | `10.0.0.2/24` |
| 🔗 Default Gateway | `10.0.0.1` |
| 🛜 DNS Server | `8.8.8.8` |
| 🧩 Future VM Range | `10.0.0.3 – 10.0.0.99` |

---


# 🪜 Lab Setup Procedure

## 🔹 Step 1: Install Win-rar

Install **Win-rar** to extract the Kali Linux virtual machine package, which is commonly provided in `.zip` archive format.

- 🧰 **Tool:** Win-rar
- 📦 **Purpose:** Extract the Kali Linux VM archive.

---

## 🔹 Step 2: Install Oracle VirtualBox

Install **Oracle VirtualBox** to create and manage the virtual machines required for the cybersecurity lab.

- 🖥️ **Tool:** Oracle VirtualBox 7.0
- ⚙️ **Purpose:** Provide the virtualization platform for running Kali Linux.

---

## 🔹 Step 3: Configure the NAT Network

Create a dedicated **NAT Network** in Oracle VirtualBox to provide network connectivity for the cybersecurity lab while keeping the virtual environment separated from the host network.

![]()

### ⚙️ Network Configuration

| 🔧 Parameter | 📡 Configuration |
|:---|:---|
| 🏷️ Network Name | `NatNetwork` |
| 🌐 IPv4 Prefix | `10.0.0.0/24` |
| 🔄 DHCP Server | Enabled |
| 🚫 IPv6 | Disabled |
| 🔗 Network Type | NAT Network |

### 🎯 Purpose

- Establish a private virtual network for the lab.
- Enable internet connectivity for connected virtual machines.
- Allow communication between machines on the same NAT Network.
- Provide DHCP-based IP address assignment.

---
