# networkwalks-B083-week1-cybersecurity-lab-setup
cybersecurity-lab-setup


# 🔐 Cybersecurity Lab Environment Setup

> A hands-on cybersecurity laboratory built using **Kali Linux** and **VirtualBox** for learning networking, reconnaissance, vulnerability assessment, penetration testing, and security tools in a controlled environment.

---

## 📌 Project Overview

This project documents the setup and configuration of my personal **Cybersecurity & Penetration Testing Lab** using VirtualBox and Kali Linux.

The main purpose of this lab is to create a **safe and controlled virtual environment** where cybersecurity concepts and security tools can be practiced without affecting real-world systems.

The lab can later be expanded by adding vulnerable target machines, Windows/Linux systems, web applications, and other security-testing environments.

---

## 🎯 Objectives

The main objectives of this project are:

- 🖥️ Install and configure VirtualBox
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
