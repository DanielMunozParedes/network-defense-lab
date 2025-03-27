# Network Defense & Detection Lab

This project simulates real-world network-based attacks within a self-hosted lab environment and implements defensive monitoring and detection logic to identify, analyze, and document malicious activity.

It is part of a broader cybersecurity portfolio focused on developing practical, hands-on skills in detection engineering, log analysis, and system monitoring.

---

## Objectives

- Simulate common network threats (port scans, brute-force attempts, unauthorized connections)
- Monitor network activity and system logs
- Detect threats using log-based analysis and detection rules
- Document attack scenarios and incident responses
- Automate aspects of log filtering and detection logic

---

## Lab Architecture

| Component | Description |
|----------|-------------|
| Kali Linux | Simulates attacker activity (Nmap, Hydra, Netcat) |
| Ubuntu Server | Target system for logging and detection |
| Wazuh (optional) | SIEM/log management and alert generation |
| Tools | UFW, syslog, tcpdump, Wireshark, Python, Bash |

### Architecture Diagram: [`architecture/lab-diagram.png`](architecture/lab-diagram.png)

---

## Attack Scenarios Simulated

| Attack Type | Tool Used | Target | Detection Method |
|-------------|-----------|--------|------------------|
| SYN Port Scan | Nmap | Ubuntu Server | UFW logs + Wazuh |
| SSH Brute Force | Hydra | SSH Service | Auth log + alert rule |
| Netcat Reverse Shell | Netcat | Open port listener | Connection log + custom logic |

---

## Repository Structure

| Folder | Purpose |
|--------|---------|
| `architecture/` | Network layout and topology diagrams |
| `setup/` | Setup notes and lab configuration steps |
| `logs/` | Collected log files (UFW, syslog, auth.log, PCAPs) |
| `detection-rules/` | Custom detection rules (e.g., Wazuh, Logstash) |
| `scripts/` | Python/Bash scripts for filtering and automation |
| `incident-report/` | Written analysis of simulated attacks |
| `screenshots/` | Screenshots of alerts, dashboards, and CLI output |
| `tools-used.md` | List of tools, commands, and references used |

---

## Project Status

| Task | Status |
|------|--------|
| Lab environment setup | ⬜️ In Progress |
| Port scan simulation | ⬜️ In Progress |
| Logging & capture | ⬜️ In Progress |
| Detection rule creation | ⬜️ Not started |
| Incident reporting | ⬜️ Not started |
| Automation script | ⬜️ Not started |

---

##  Tools & Technologies

- Linux (Ubuntu Server, Kali Linux)
- UFW / Syslog
- Wireshark / tcpdump
- Python / Bash
- Wazuh (maybe?)
- Git / GitHub for documentation

---

## Skills Demonstrated

- Network-level threat detection
- Log analysis and parsing
- SIEM rule writing (manual or automated)
- System configuration and hardening
- Incident response documentation
- Scripting for detection automation

---

## 📌 Tags

`Blue Team` `Detection Engineering` `Log Analysis` `Linux Security` `SIEM` `Network Monitoring` `Incident Response`

