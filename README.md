
<div align="center">

# 🔐 Cybersecurity Lab Environment Setup

**Building an isolated virtual lab for penetration testing and ethical hacking practice**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.2-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Virtualization-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali%20Linux-404040?style=flat-square&labelColor=C00000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Samuel%20Miracle%20-C00000?style=flat-square" />
</p>

## 📌 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using Oracle VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is designed around a private virtual network so that additional virtual machines can be added in future projects and used as targets for authorized security testing.

---

## 🎯 Objectives

The main objectives of this project are to:

- Install and configure Oracle VirtualBox.
- Download and import Kali Linux as a virtual machine.
- Create a private NAT Network for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Identify and verify the IPv4 address assigned to the Kali virtual machine.
- Verify the default gateway and DNS resolution.
- Test internet connectivity and basic network functionality.
- Create a clean virtual machine snapshot for recovery.
- Document the laboratory setup process.
- Prepare the environment for future cybersecurity and penetration-testing projects.

---

## 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for activities such as:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Exploitation practice
- Security-tool experimentation

⚠️ **Important:** This laboratory is intended for educational purposes and authorized security testing. Only test systems that you own or have explicit permission to assess. Do not use the tools or techniques learned in this lab against unauthorized systems.

---

## 🏗️ Lab Architecture

The laboratory uses a Windows host machine running Oracle VirtualBox, with Kali Linux operating as a guest virtual machine.

VirtualBox provides the virtualization environment, while the NAT Network provides connectivity for virtual machines attached to it. A NAT Network can allow attached virtual machines to communicate with one another while providing outbound connectivity.

This setup establishes the foundation for a controlled cybersecurity environment. Additional virtual machines can be connected to the same NAT Network in future projects for practical security exercises.

**Lab components:**

- **Host machine:** Windows 10 (confirm the installed Windows version)
- **Virtualization platform:** Oracle VirtualBox
- **Guest operating system:** Kali Linux
- **Virtual networking:** NAT Network
- **Future expansion:** Additional authorized testing and target virtual machines

---

## ⚙️ Lab Configuration

### 💻 Host Machine Specifications

| 🧩 Component | ⚙️ Configuration |
|---|---|
| 🖥️ Host OS | Windows 10 (verify) |
| 🧠 Host RAM | 8 GB DDR3 |
| 💾 Storage | 297 GB |
| ⚡ Processor | Intel Core i5-4310U |
| 🔢 CPU Cores | 2 |
| 🚀 Base CPU Speed | 2.60 GHz |
| 🎮 Graphics | Integrated Intel HD Graphics |
| 🧰 Hypervisor | Oracle VirtualBox 7.2.14 r174565 |
| 🖼️ GUI Framework | Qt 6.8.0 |
| 🐉 Security OS | Kali Linux 2026.2 (verify the imported image version) |

### 🌐 Virtual Network Configuration

| 🧩 Component | ⚙️ Configuration |
|---|---|
| 🌐 Virtual Network Type | NAT Network |
| 📡 Network Name | NatNetwork (verify in VirtualBox) |
| 🖧 IPv4 Network Prefix | Confirm from the NAT Network settings |
| 🐧 Kali IPv4 Address | Confirm from Kali Linux |
| 🚪 Default Gateway | Confirm from the routing table |
| 🌍 DNS Server | Confirm from the active DNS configuration |
| 🔮 Future VM Range | Determine from the final network configuration |

### 🖥️ Kali Linux Virtual Machine

| 🧩 Component | ⚙️ Configuration |
|---|---|
| 🐉 Operating System | Kali Linux |
| 🧰 Virtualization Platform | Oracle VirtualBox |
| 🧠 Allocated RAM | Confirm from VirtualBox VM settings |
| 🌐 Network Adapter | NAT Network |
| 📡 Attached Network | Confirm the selected NAT Network name |
| 🔌 Adapter Type | Confirm from VirtualBox VM settings |

---

## 🪜 Lab Setup Procedure

### Step 1. Install 7-Zip

7-Zip can be used to extract the Kali Linux virtual-machine package if it is downloaded in a compressed `.7z` archive format.

7-Zip is a file archiving utility that supports the extraction of compressed files and archives.

**Tool:** [7-Zip Official Download Page](https://www.7-zip.org/download.html)

### Step 2. Install Oracle VirtualBox

Oracle VirtualBox was used as the hypervisor for the cybersecurity laboratory.

A hypervisor allows virtual machines to run on a physical computer. In this project, VirtualBox provides the environment in which Kali Linux operates as a guest operating system.

The installed VirtualBox version is **7.2.14 r174565**, with Qt 6.8.0 on Windows.

### Step 3. Create the NAT Network

A dedicated NAT Network was configured in VirtualBox for the cybersecurity laboratory.

A NAT Network allows virtual machines attached to the same virtual network to communicate with one another while using Network Address Translation (NAT) for outbound connectivity.

This setup provides a foundation for adding other virtual machines, including target machines, in future cybersecurity exercises.

#### ⚙️ Network Configuration

Confirm the following settings against the actual configuration in VirtualBox before publishing the final values.

| Setting | Configuration |
|---|---|
| Network Name | NatNetwork (verify) |
| IPv4 Prefix | Confirm from VirtualBox |
| DHCP | Confirm whether enabled |
| IPv6 | Confirm whether enabled or disabled |

#### 📸 Screenshot Evidence

![VirtualBox NAT Network Configuration] 
<img width="1600" height="862" alt="WhatsApp Image 2026-10-29 at 3 53 41 AM (1)" src="https://github.com/user-attachments/assets/a8f6be93-b332-45df-ba62-59209b7b394c" />



### Step 4. Download and Import Kali Linux

Kali Linux was obtained from the official Kali Linux website and imported into Oracle VirtualBox as a virtual machine.

Kali Linux is a Linux distribution designed for penetration testing, digital forensics, security research, and other information-security activities.

After importing the virtual machine, its hardware settings and network adapter were reviewed to prepare it for the laboratory environment.

**Download:** [Official Kali Linux Download Page](https://www.kali.org/get-kali/)

#### 🔌 Virtual Machine Network Settings

The virtual machine's network adapter should use the NAT Network created in Step 3.

Example configuration:

```text
Adapter 1
Attached to: NAT Network
Network:     NatNetwork
Adapter Type:Intel PRO/1000 MT Desktop (82540EM)
```

Verify the network name and adapter type in the actual VirtualBox settings.

#### 🧠 Memory Allocation

The virtual machine's RAM allocation should leave sufficient memory for Windows and other running applications.

My host computer has 8 GB of RAM, so the allocation should be appropriate for the available system resources.

**Actual allocated RAM:** 5095 MB

#### 📸 Screenshot Evidence

![Kali Linux Imported into VirtualBox] 
<img width="1600" height="863" alt="WhatsApp Image 2026-10-29 at 3 53 57 AM (1)" src="https://github.com/user-attachments/assets/b3eb52c8-dade-4d24-b56c-8e0bcc05899c" />



![Kali Linux Virtual Machine Network Settings] 
<img width="790" height="523" alt="WhatsApp Image 2026-10-29 at 3 52 47 AM (1)" src="https://github.com/user-attachments/assets/fbed1628-a3a2-47ae-978b-2423552fd185" />


### Step 5. Configure the Kali Linux Network

The Kali Linux network configuration was checked to establish connectivity through the configured virtual network.

The network settings include the IPv4 address, subnet mask, default gateway, and DNS server. These values determine how the virtual machine communicates with other devices and resolves domain names.
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8

#### 🌐 Network Configuration

Check the network interfaces and assigned IP addresses:

```bash
ip a
```

Display the routing table:

```bash
ip route
```

Check the DNS configuration:

```bash
cat /etc/resolv.conf
```

These commands help identify the active network interface, assigned IPv4 address, subnet information, default route, and configured DNS resolver.

#### 🔎 Network Verification Commands

After identifying the actual gateway, test connectivity to it:

```bash
ping -c 4 <gateway-IP>
```

Replace `<gateway-IP>` with the gateway address shown by `ip route`.

Test outbound connectivity using a public IP address:

```bash
ping -c 4 8.8.8.8
```

Test DNS resolution:

```bash
nslookup networkwalks.com
```

A successful DNS lookup indicates that the domain name resolved to an IP address. A failed ping alone does not necessarily mean the network is unavailable because ICMP traffic may be blocked.

#### 📸 Screenshot Evidence

![Kali Linux Network Configuration] 
<img width="1600" height="863" alt="WhatsApp Image 2026-10-29 at 3 53 07 AM (1)" src="https://github.com/user-attachments/assets/01f37600-2623-40d0-83f5-77a89cf032f2" />



### Step 6. Create a Clean Virtual Machine Snapshot

After the initial configuration and verification steps have been completed, create a clean snapshot in VirtualBox.

A snapshot records the virtual machine's state at a particular point in time. It provides a recovery point that can be used if a future cybersecurity exercise changes the machine's configuration or makes it difficult to use.

#### 📌 Example Snapshot Name

```text
Clean Kali - Network Setup
```

The snapshot should represent the baseline configuration of the laboratory after the initial setup has been verified.

If a future exercise changes or damages the VM configuration, the snapshot can help restore the virtual machine to its saved state.


---

## 🔎 Lab Verification

The following checks can be used to verify the initial laboratory configuration.

| ✅ Test | 🧾 Command | 🎯 Expected Result |
|---|---|---|
| 🌐 Check IP address | `ip a` | The assigned Kali IPv4 address is displayed |
| 🛣️ Check routing table | `ip route` | The expected routes and default route are displayed |
| 📡 Test gateway | `ping -c 4 <gateway-IP>` | Successful replies, |
| 🌍 Test outbound connectivity | `ping -c 4 8.8.8.8` | Successful replies, |
| 🔎 Test DNS resolution | `nslookup networkwalks.com` | The domain resolves successfully |
| 🧰 Verify Nmap | `nmap --version` | The installed Nmap version is displayed |
| 🔄 Verify snapshot | Restore the snapshot and run `ip a` | The saved baseline configuration is restored |

### 📋 Verification Results

Record the actual results from your lab before publishing this section.

| Check | Actual Result |
|---|---|
| Kali IPv4 address | Successfully configured |
| Default gateway | Successfully configured |
| DNS resolution | Successful |
| Internet connectivity | Successful |
| Nmap installation | Installed and verified |
| Snapshot created | Successfully created |
---

## 🐞 Problems Encountered & Solutions

Documenting problems and their solutions is an important part of a cybersecurity lab report.

The following are examples of issues that can occur during setup. Keep only the issues you actually encountered and describe the solution you used.

### Problem 1. Internet Connectivity After Static IP Configuration

Manually configuring IPv4 settings can cause connectivity problems if the IP address, subnet mask, gateway, or DNS configuration does not match the virtual network.

#### Troubleshooting Approach

1. Check the assigned IP address using `ip a`.
2. Check the routing table using `ip route`.
3. Verify that the default gateway matches the configured NAT Network.
4. Check the DNS configuration.
5. Test gateway connectivity and DNS resolution separately.
6. Review the active NetworkManager connection and its settings if the problem persists.

The following command displays the available NetworkManager connections:

```bash
nmcli connection show
```

Identify the actual connection name before making changes. Adjust network settings according to the observed problem rather than applying an unrelated workaround.

### Problem 2. VirtualBox VT-x / Virtualization Error

Virtual machines may fail to start if hardware virtualization is disabled or if the host's virtualization configuration is incompatible with the selected VM settings.

#### Troubleshooting Approach

1. Check whether hardware virtualization is enabled in the system firmware.
2. Restart the computer and enter the BIOS/UEFI settings if necessary.
3. Enable Intel VT-x if it is disabled.
4. Save the configuration and restart the computer.
5. Start the Kali Linux virtual machine again.
6. Review any remaining error messages if the VM still fails to start.

**Documentation note:** Remove or replace this example if you did not encounter this problem during your project.

---

## 💡 What I Learned

Through this project, I developed a better understanding of how to create and configure a virtual environment for cybersecurity practice.

The main concepts covered include:

### 1. NAT vs. NAT Network

A standard NAT adapter and a NAT Network serve different purposes.

A standard NAT adapter generally provides outbound connectivity for an individual virtual machine. A NAT Network can allow multiple attached virtual machines to communicate with one another while also providing outbound connectivity.

This makes a NAT Network useful for building a multi-machine cybersecurity laboratory.

### 2. Virtual Machine Networking

I learned how VirtualBox network adapters connect virtual machines to different network configurations and how these settings affect communication between virtual machines and external networks.

### 3. IPv4 and DNS Configuration

I learned the importance of IPv4 addresses, subnet masks, default gateways, and DNS servers in establishing network connectivity.

I also learned how to use Linux commands to inspect network settings and troubleshoot connectivity problems.

### 4. Virtual Machine Snapshots

A clean snapshot provides a known-good recovery point before performing experimental or potentially disruptive activities.

This helps preserve a working laboratory configuration for future cybersecurity exercises.

### 5. Documentation and Verification

I learned the importance of documenting configuration settings, commands, screenshots, test results, and troubleshooting steps.

Clear documentation makes it easier to reproduce a setup and demonstrate the work completed during a cybersecurity project.

---

## 🔐 Security & Ethical Use

This laboratory is intended for educational purposes and authorized security testing.

All scanning, reconnaissance, and testing activities should be performed only on systems that I own or have explicit permission to assess.

The lab provides a controlled environment for developing practical cybersecurity skills responsibly.

---

## 🔗 Tools & Resources

- 📦 **7-Zip:** https://www.7-zip.org/download.html
- 🖥️ **Oracle VirtualBox:** https://www.virtualbox.org/wiki/Downloads
- 🐉 **Kali Linux:** https://www.kali.org/get-kali/
- 📖 **NetworkWalks Reference Project:** https://github.com/waqaskarimccie/NETWORKWALKS-B082-WK1-PM1-CYBERSECURITY-LAB-SETUP-SAMPLE

---

## 👤 Author

**Samuel Miracle**

Cybersecurity | Ethical Hacking | Penetration Testing

**Program:** NetworkWalks Cybersecurity Internship — Batch B084

🔗 **LinkedIn:** https://www.linkedin.com/in/samuel-miracle-1a7725338/

---

## 📌 Project Information

| Field | Details |
|---|---|
| Program Name | Cybersecurity at NetworkWalks |
| Batch | B084 |
| Week | 01 |
| Project | Cybersecurity & Penetration-Testing Lab Setup |
| Platform | GitHub |
| Virtualization Platform | Oracle VirtualBox |
| Operating System | Kali Linux |

---

<p align="center">
  <b>NetworkWalks Cybersecurity Internship | Batch B084 | Week 01</b>
</p>
