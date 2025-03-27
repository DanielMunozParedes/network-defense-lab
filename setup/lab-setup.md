                 [ Desktop: Kali Linux ]
                 -----------------------
                 - Attacker machine
                 - Tools: Nmap, Hydra, Netcat
                 

                           |
                           |  (Same LAN)
                           |
                 -----------------------
                 |  Laptop: Ubuntu Server  |
                 |-------------------------|
                 | - Target of attacks     |
                 | - UFW + Logs + SSH      |
                 | - Wazuh Agent + Manager |
                 |                         |
                 -------------------------

                           |
                           |
                 ----------------------------
                 | Laptop: Windows 11        |
                 |---------------------------|
                 | - Legit user machine      |
                 | - Connects to Ubuntu via  |
                 |   SSH for admin tasks     |
                 | - Deploys Wazuh, views logs|
                 |                           |
                 ----------------------------
