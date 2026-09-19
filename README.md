# networkwalks-B083-week1-cybersecurity-lab-setup
cybersecurity-lab-setup

# 🔐 Cybersecurity Lab Environment Setup

> A hands-on cybersecurity laboratory built using **Kali Linux** and **Oracle VirtualBox** for learning networking, reconnaissance, vulnerability assessment, penetration testing, and security tools in a controlled environment.

---

## 📌 Project Overview

This project documents the setup and configuration of my personal **Cybersecurity & Penetration Testing Lab** using Oracle VirtualBox and Kali Linux.

The main purpose of this lab is to create a **safe and controlled virtual environment** where cybersecurity concepts, networking, and security tools can be practiced without affecting real-world systems.

This laboratory can later be expanded by adding vulnerable target machines, Windows/Linux systems, web applications, and other security-testing environments.

---

## 🎯 Objectives

The main objectives of this project are:

- 🖥️ Install and configure Oracle VirtualBox
- 🐉 Install and configure Kali Linux
- 🌐 Create a dedicated virtual network
- 🔧 Configure Kali Linux networking
- 📡 Verify network connectivity
- 🔍 Verify basic cybersecurity tools
- 💾 Create a clean VM snapshot
- 📝 Document the complete lab setup
- 🚀 Prepare the environment for future cybersecurity projects

---

## 🛡️ Purpose of the Lab

This laboratory is designed for **cybersecurity education and authorized security testing**.

The environment can be used for:

- 🔎 Network reconnaissance
- 📡 Network scanning
- 🔐 Security testing
- 🧪 Vulnerability assessment
- 🌐 Web security testing
- 📦 Packet analysis
- 🛠️ Security-tool experimentation
- 💻 Penetration-testing practice

> ⚠️ **Ethical Use**
>
> All testing must be performed only on systems that you own or have explicit permission to test.
> Never use these tools against unauthorized systems or networks.

---

# 🏗️ Lab Architecture

The current laboratory consists of a host computer running VirtualBox with Kali Linux as the primary cybersecurity machine.

```text
                 ┌──────────────────────┐
                 │     Host Computer    │
                 │      Windows OS      │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │      VirtualBox      │
                 │     Hypervisor       │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │     Virtual Network  │
                 │     NAT Network      │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │      Kali Linux      │
                 │   Security Machine   │
                 └──────────────────────┘

```


# 🧠 What I Learned

## 1. Virtualization

I learned how VirtualBox can be used to create isolated virtual machines for cybersecurity practice.

---

## 2. Virtual Networking

I learned how virtual network adapters and NAT Networks allow virtual machines to communicate in a controlled environment.

---

## 3. IP Addressing

I learned how to identify and configure:

- IPv4 addresses
- Subnet masks
- Default gateways
- DNS servers
- Network routes

---

## 4. Network Troubleshooting

I learned how to troubleshoot connectivity step-by-step:

```text
Network Interface
       ↓
   IP Address
       ↓
    Routing
       ↓
    Gateway
       ↓
    Internet
       ↓
      DNS
```



# 🪜 Lab Setup Procedure

## Step 1. Install 7-Zip

7-Zip was installed to extract the Kali Linux virtual-machine package, which may be distributed as a `.7z` archive.

**Tool:** 7-Zip

---

## Step 2. Install VirtualBox

VirtualBox was installed as the hypervisor.

---

## Step 3. Create the NAT Network

A dedicated NAT Network was created in VirtualBox.

Configuration:
Network Name: NatNetwork
IPv4 Prefix:  10.0.0.0/24
DHCP:         Enabled
IPv6:         Disabled


A **NAT Network** was selected because multiple virtual machines connected to the same NAT Network can communicate with one another while also having outbound network connectivity.

This will allow future attacker and target VMs to communicate within the lab.


---

## Step 4. Import Kali Linux

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

A shared folder was also configured for transferring required files between the host operating system and the Kali VM.



---

## Step 5. Configure the Kali Linux Network

The Kali Linux network configuration was checked and configured with a consistent IPv4 address.

Example configuration:

```text
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8
```

A consistent IP address makes it easier to document the lab and reference the Kali machine in future exercises.



---

## Step 6. Create a Clean VM Snapshot

After completing the initial configuration, a VirtualBox snapshot was created.

Example snapshot name:

```text
Clean Kali - Network Setup
```

The snapshot represents the clean baseline of the laboratory.

If a future exercise changes or damages the VM configuration, the machine can be restored to this baseline.


---



# 🔗 Tools & Resources

- **7-Zip:** [https://7-zip.org/download.html](https://7-zip.org/download.html)
- **VirtualBox:** [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
- **Kali Linux:** [https://kali.org/get-kali](https://kali.org/get-kali)

---




## 📌 Project Information
Program Name: Cybersecurity at Networkwalks | Week: 01 | Project: Cybersecurity & Pentesting Lab Setup | Repository: GitHub

