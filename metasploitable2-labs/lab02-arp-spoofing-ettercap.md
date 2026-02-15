Lab 02 – ARP Spoofing (Man-in-the-Middle) Simulation

## Objective
Simulate an ARP spoofing attack in a controlled lab environment to understand how Man-in-the-Middle (MITM) attacks work.

## Environment
- Attacker: Kali Linux
- Target: Metasploitable 2
- Tools Used: Ettercap, Wireshark
- Network Type: NAT / Host-only lab network

## Enumeration
- Identified target IP address
- Verified connectivity using ping
- Confirmed ARP table entries

## Attack Execution
- Enabled IP forwarding on attacker machine
- Launched Ettercap in ARP spoofing mode
- Targeted victim and gateway IP addresses

Example command used:
ettercap -T -q -i eth0 -M arp:remote /TARGET-IP/ /GATEWAY-IP/


## Traffic Analysis
- Captured packets using Wireshark
- Observed intercepted traffic between victim and gateway
- Verified successful MITM position

## Post-Attack Verification
- Confirmed traffic interception
- Checked ARP tables for poisoning evidence

## Mitigation
- Use static ARP entries
- Enable Dynamic ARP Inspection (DAI)
- Use encrypted protocols (HTTPS, SSH)


- Implement network segmentation![etter](https://github.com/user-attachments/assets/b59c9790-b3fe-48a4-8e1f-ba045f67eb93)
![etter3](https://github.com/user-attachments/assets/d73ac965-5965-499a-a02b-8fda846f81e0)
![etter2](https://github.com/user-attachments/assets/861bdf04-2345-4945-b29b-58f2ee9da2e7)
