# Lab 01 – Cryptography, Hashing, and Password Security

## Objective
Understand password security by testing cryptography and hashing techniques in a controlled environment, and observe how SOC tools can detect weak practices.

## Environment
- Lab Machine: Kali Linux
- Tool: Pentbox
- Monitoring: Wazuh (SOC)
- Network: Isolated lab environment

## Pentesting Perspective
1. Used Pentbox to simulate password cracking attacks on test accounts
2. Explored different hash types (MD5, SHA1, SHA256) and their weaknesses
3. Tested password policies (length, complexity)
4. Observed which passwords are easily cracked

## SOC / Defensive Perspective
1. Monitored login attempts using Wazuh
2. Created alerts for repeated failed login attempts
3. Analyzed hash storage and recommended best practices

## Key Takeaways
- Weak passwords and outdated hash functions are vulnerable
- SOC can detect brute force and suspicious authentication attempts
- Strong password policies + salted hashes are essential

## Screenshots
- Pentbox password test interface
- Hash cracking output
- Wazuh alert for repeated login attempts

![cryp](https://github.com/user-attachments/assets/6f8fee74-63f7-4abe-81df-e2659764d934)
