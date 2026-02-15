# Lab 01 – Social Engineering Simulation & Defense

## Objective
Simulate a social engineering scenario in a controlled lab to understand:
- How attackers attempt credential capture (pentesting perspective)
- How a SOC team can detect and respond (defensive perspective)

## Environment
- Attacker Machine: Kali Linux (Lab Only)
- Target: Local test server / isolated VM
- Tools: Social-Engineer Toolkit (SET), Wireshark
- Network: Isolated lab (no real users)

## Pentesting Steps
1. Simulated phishing email sent to lab VM
2. Captured HTTP POST requests in a test environment only
3. Analyzed how session data could be exposed if not secured

## SOC / Defensive Steps
1. Monitored network traffic with Wireshark
2. Set up Wazuh rules to detect suspicious connections
3. Logged alerts for simulated credential exfiltration attempts
4. Recommended mitigation:
   - Multi-factor authentication
   - Employee phishing awareness training
   - Encrypted communications (HTTPS)

## Learning Outcome
- Pentester: Learned how social engineering frameworks work safely  
- SOC Analyst: Learned how to detect and respond to simulated attacks


![setl](https://github.com/user-attachments/assets/8ca640ed-f9f2-4526-b870-c91bb75ebf48)
