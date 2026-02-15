# Lab 01 – Deploying a Honeypot with Pentbox

## Objective
Deploy a honeypot to simulate network attacks in a controlled environment and study:
- How attackers interact with decoy systems (Pentesting perspective)  
- How SOC can monitor and respond to suspicious activity (Defensive perspective)

## Environment
- Attacker / Lab Machine: Kali Linux
- Honeypot Target: Pentbox (Decoy Server)
- Monitoring: Wireshark, Wazuh (SOC)
- Network: Isolated lab environment

## Pentesting Perspective
1. Installed Pentbox on a lab VM
2. Configured services (FTP, HTTP, SSH) to appear vulnerable
3. Simulated attack attempts from another lab VM
4. Observed how honeypot logs all connection attempts

## SOC / Defensive Perspective
1. Configured Wazuh to monitor honeypot logs
2. Captured incoming attack traffic with Wireshark
3. Created alerts for unusual login attempts
4. Learned how honeypots provide early detection of potential attacks

## Screenshots
- Honeypot service running (Pentbox)
- Wireshark capturing traffic
- Wazuh alert showing attacks


![hny2](https://github.com/user-attachments/assets/4f5342ea-9815-4c5c-a9e9-0eac22dc4bb0)
![hny](https://github.com/user-attachments/assets/84f5c565-c676-44cf-bf4c-1b7072a76caa)
