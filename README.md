# SOC Automation Lab (Homelab)
This project is a fully virtualized Security Operations Center (SOC) home lab designed for hands-on experience planning, designing, and creating a SOC automated environment. It simulates a small corporate environment with centralized monitoring via Wazuh SIEM, a pfSense firewall with Snort IDS/IPS, and multiple endpoints. Lab also includes SOAR implementation (Shuffle).

## 📌 Overview
The lab runs entirely in **VMware Workstation** on a single host machine, using an **isolated host-only network** with pfSense acting as the gateway and WAN interface for simulated internet access.

**Core Features:**
- **Wazuh Manager + Indexer + Dashboard** for SIEM capabilities
- **pfSense Firewall** with Snort IDS/IPS for traffic monitoring and blocking
- **Windows 10 Endpoint** with Sysmon and Wazuh agent for log forwarding
- **Ubuntu Desktop** Wazuh agent for analyst workstation
- **Shuffle** for automation and orchestration
- **TheHive** for incident response case manangement
- **Simulated WAN** for realistic traffic flow

---

## 🖥️ Network Diagram
![Network Diagram](https://github.com/0xTrust-cell/SOC-Automation-Lab/blob/main/Network%20Diagram.pdf)

---

## ⚙️ Lab Architecture

| Component           | Purpose                                            |
|---------------------|----------------------------------------------------|
| **pfSense**         | Firewall, routing, and Snort IDS/IPS               |
| **Ubuntu Server 1** | Wazuh All-in-One (Indexer + Server + Dashboard)    |
| **Ubuntu Server 2** | TheHive + Shuffle for SOAR                         |
| **Windows 10**      | Simulated user endpoint (Sysmon + Wazuh agent)     |
| **Ubuntu Desktop**  | Analyst workstation with Wazuh agent               |

---

## 🔑 Key Skills Demonstrated
- SIEM Deployment & Management (Wazuh)
- IDS/IPS Configuration (Snort)
- Network Security Architecture
- Threat Detection & Incident Response
- Firewall Rules & Segmentation
- Sysmon Log Collection & Analysis
- Security Orchestration, Automation, and Response (SOAR)

---

## 🛠️ Step-by-Step Build Guide
The full setup guide is documented in [`docs/setup-guide.md`](docs/setup-guide.md).

---

## 📂 Repository Structure

