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


![](https://github.com/jahidhsn-rng/networkwalks-B084D-week1-cybersecurity-lab-setup/blob/103a8cdfa3bbe98898ad4153210c43da8fde0b57/NAT%20network.PNG)

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

## 🔹 Step 4. Import Kali Linux

The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.

The VM network adapter was configured as follows:

```text
Adapter 1
Attached to: NAT Network
Network:     NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop
```

The VM was allocated:

```text
RAM: 2048 MB
```
![](https://github.com/jahidhsn-rng/networkwalks-B084D-week1-cybersecurity-lab-setup/blob/bd3e6e752b6f1af66f0dc8fffbc9d37aac2f2daf/kali%20snapp.PNG)

A shared folder was also configured for transferring required files between the host operating system and the Kali VM.

---

---

## 🔹 Step 5: Configure the Kali Linux Network

**Network Configuration**

- IP Address: 10.0.0.2
- Subnet Mask: 255.255.255.0
- Gateway: 10.0.0.1
- DNS: 8.8.8.8

Using a fixed IP address simplifies lab documentation and makes it easier to identify and access the Kali Linux machine during future practical exercises.

---

## 🔹 Step 6. Create a Baseline VM Snapshot

Once the initial setup and configuration were completed, a snapshot of the Kali Linux virtual machine was saved in VirtualBox.

Example snapshot name:
```text
Kali Linux - Initial Network Setup
```
This snapshot serves as a backup of the virtual machine in its original configured state.

If any future lab activity causes configuration errors or system issues, the virtual machine can easily be restored to this saved snapshot.

---


---

## 🛡️ LAB VERIFICATION & VALIDATION

The following tests were performed to verify the Kali Linux virtual machine configuration, network connectivity, and installed tools.

| 🔧 Verification Test | 💻 Command / Action | 🎯 Expected Outcome |
|:---|:---|:---|
| 🖥️ IP Configuration | `ip a` | Displays the assigned Kali Linux IP address |
| 🔗 Gateway Connectivity | `ping 10.0.0.1` | Successful ping replies received |
| 🌐 Internet Connectivity | `ping 8.8.8.8` | External network connection confirmed |
| 🔍 DNS Resolution | `nslookup networkwalks.com` | Domain name resolves successfully |
| ⚙️ Nmap Verification | `nmap --version` | Installed Nmap version displayed |
| 💾 Snapshot Recovery | Restore snapshot and run `ip a` | Original VM configuration restored |

---

### ✅ Verification Checklist

- [ ] Kali Linux IP address configured correctly
- [ ] Gateway connectivity verified
- [ ] Internet access confirmed
- [ ] DNS resolution working
- [ ] Nmap installed and functioning
- [ ] Virtual machine snapshot successfully restored

**📌 Result:** The lab environment is ready for the next phase once all verification checks pass.

---


---

# 🛠️ Troubleshooting & Issues Resolved

Documenting technical challenges and their corresponding solutions is an essential part of maintaining a reliable and reproducible laboratory environment.

## ⚠️ Issue 01: Network Connectivity After Static IP Configuration

**Problem:**

Following the manual configuration of IPv4 network settings, Internet connectivity was interrupted due to potential compatibility or configuration issues involving Kali Linux and NetworkManager.

**Solution:**

The following NetworkManager command was used as a troubleshooting measure:

```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
```

After applying the configuration, the network connection was restarted and connectivity was tested again.

> **Note:** Network connection names may vary across systems. Use `nmcli connection show` to identify the correct connection name before executing the command.

---

## ⚠️ Issue 02: VirtualBox Hardware Virtualization Error

**Problem:**

The Kali Linux virtual machine initially failed to start because hardware virtualization (Intel VT-x) was disabled in the system BIOS/UEFI firmware.

**Resolution Steps:**

1. Restarted the host computer.
2. Entered the BIOS/UEFI configuration menu.
3. Located and enabled Intel VT-x (hardware virtualization).
4. Saved the updated firmware settings.
5. Restarted the system.
6. Launched the Kali Linux virtual machine again.

**Outcome:**

The virtualization issue was resolved, and the Kali Linux virtual machine started successfully.

---

# 📚 Key Learnings & Technical Takeaways

Throughout this project, I gained practical experience in configuring virtualized environments and establishing a foundation for cybersecurity laboratory exercises.

The key technical concepts covered include:

### 01. 🌐 NAT vs. NAT Network

I learned the functional differences between VirtualBox NAT and NAT Network configurations.

Unlike standard NAT, NAT Network allows multiple virtual machines connected to the same virtual network to communicate with one another while providing network address translation for external connectivity.

This configuration is particularly useful when developing multi-machine cybersecurity testing environments.

### 02. 🔌 Virtual Machine Networking

I gained a better understanding of how VirtualBox network adapters connect virtual machines to different network environments.

I also explored how network adapter configurations influence connectivity and communication between virtual machines and external networks.

### 03. 📡 Static IP Address Configuration

I developed practical experience configuring and verifying IPv4 network parameters in Kali Linux, including:

- IP addresses
- Subnet masks
- Default gateways
- DNS servers

I also learned the importance of maintaining consistent network configurations throughout laboratory exercises.

### 04. 💾 Virtual Machine Snapshots & Recovery

I learned the importance of creating a clean baseline snapshot before conducting experimental or potentially disruptive activities.

Snapshots provide a reliable recovery point, allowing the virtual machine to return to a previously saved configuration when troubleshooting or performing future cybersecurity exercises.

### 05. 📝 Technical Documentation

I recognized the importance of maintaining structured and detailed technical documentation.

Recording commands, network configurations, screenshots, troubleshooting procedures, and their corresponding solutions improves reproducibility and makes technical projects easier to understand, maintain, and review.

---

# 🔐 Security & Ethical Considerations

This laboratory environment was developed exclusively for educational purposes, cybersecurity training, and authorized testing.

All experiments and security-related activities should be performed only within systems and networks for which proper authorization has been obtained.

**⚖️ Responsible Learning. Ethical Testing. Continuous Improvement.**

---


---

# 🔗 Tools, Platforms & Resources

The following tools and platforms were used during the laboratory setup and configuration process.

| 🧰 Tool / Platform | 🔗 Official Resource |
|:---|:---|
| 📦 WinRAR | [Official Download Page](https://www.win-rar.com/download.html) |
| 🖥️ Oracle VirtualBox | [Official Download Page](https://www.virtualbox.org/wiki/Downloads) |
| 🐉 Kali Linux | [Official Download Page](https://www.kali.org/get-kali/) |

---

## 👨‍💻 Author & Contact

# Jahid Hassan

Cybersecurity Enthusiast | Aspiring Security Professional


🔗 **LinkedIn Profile:** [Connect with me on LinkedIn](https://www.linkedin.com/in/jahid-hassan-rng57/)

---

## 📋 Project Information

| **Project Details** | **Description** |
|:---|:---|
| 🎓 Program | Cybersecurity at networkWalks |
| 📅 Week | 01 |
| 🛡️ Project Title | Cybersecurity & Penetration Testing Lab Setup |
| 💻 Platform | GitHub |
| 👨‍💻 Author | Jahid Hassan |
| 🏷️ Batch | B084 |

---

**⭐ Thank you for visiting this repository!**

Feel free to explore the project, review the configurations, and connect with me on LinkedIn.

---
