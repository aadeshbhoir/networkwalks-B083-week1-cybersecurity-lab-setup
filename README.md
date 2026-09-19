# networkwalks-B083-week1-cybersecurity-lab-setup
cybersecurity-lab-setup

# 🔐 Cybersecurity Testing Lab Setup

### WEEK 01 — Cybersecurity & Pentesting Lab Environment

> A virtual cybersecurity testing environment built using **Kali Linux** and **Oracle VirtualBox** for learning, security testing, and future penetration-testing labs.

---

## 📌 Project Overview

The objective of this project was to create a basic **cybersecurity testing laboratory** using Kali Linux running inside Oracle VirtualBox.

The lab provides an isolated virtual environment where cybersecurity tools, networking concepts, and security-testing techniques can be practiced safely.

---

## 🎯 Objectives

- Set up a Kali Linux virtual machine.
- Configure Oracle VirtualBox networking.
- Create a **NAT Network** for the cybersecurity lab.
- Configure the `10.0.0.0/24` network.
- Verify Internet connectivity.
- Test basic network connectivity from Kali Linux.
- Create a VirtualBox snapshot for recovery.
- Document the complete lab setup.

---

## ⚙️ Lab Environment

| Component | Configuration |
|---|---|
| 💻 Virtualization Platform | Oracle VirtualBox |
| 🐉 Testing Machine | Kali Linux |
| 🌐 Network Type | NAT Network |
| 📡 Network | `10.0.0.0/24` |
| 🌍 Internet Access | Enabled |
| 💾 VM Snapshot | `week1` |
| 🖥️ Host OS | Windows |

---

## 🏗️ Lab Architecture

```text
                    🌐 Internet
                        │
                        │
                ┌───────▼────────┐
                │  NAT Network   │
                │  10.0.0.0/24   │
                └───────┬────────┘
                        │
                ┌───────▼────────┐
                │  Oracle        │
                │  VirtualBox    │
                └───────┬────────┘
                        │
                ┌───────▼────────┐
                │   Kali Linux   │
                │ Cybersecurity  │
                │ Testing VM     │
                └────────────────┘
