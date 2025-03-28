# Ubuntu Logging & UFW Setup

This step documents the firewall and SSH hardening configuration on the Ubuntu Server for the Network Defense & Detection Lab.


- System updated and upgraded  
- UFW firewall installed and configured  
- SSH access restricted to only the trusted Win11 IP  
- Logging enabled for tracking incoming connections

---

## Commands Used

System Update & Upgrade:  
`sudo apt update && sudo apt upgrade -y`

Install UFW:  
`sudo apt install ufw -y`

Remove default SSH rule:  
`sudo ufw delete allow ssh`

Allow SSH only from Win11 (192.168.0.100):  
`sudo ufw allow from 192.168.0.100 to any port 22`

Enable UFW and turn on verbose logging:  
`sudo ufw enable`  
`sudo ufw status verbose`  
`sudo ufw logging on`

---

## Logs Location

UFW logs are recorded in: `/var/log/ufw.log`  
To monitor in real-time: `sudo tail -f /var/log/ufw.log`

---

## ✅ Result

- Firewall is active  
- SSH access is limited to the admin device only  
- All blocked traffic and attack attempts will be logged and ready for analysis  
