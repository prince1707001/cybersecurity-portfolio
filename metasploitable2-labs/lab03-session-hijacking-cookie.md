# Lab 03 – Session Hijacking via Cookie Manipulation

## Objective
Demonstrate session hijacking by capturing and reusing a valid session cookie in a controlled lab environment.

## Environment
- Attacker: Kali Linux
- Target: Metasploitable 2 Web Application
- Tools: Wireshark, EditThisCookie (Browser Extension)
- Network: Host-only / NAT Lab Network

## Attack Scenario
A victim user logs into a web application over an insecure connection.  
The attacker captures the session cookie and reuses it to gain unauthorized access.

## Traffic Capture
- Started Wireshark on attacker machine
- Applied HTTP filter to capture web traffic
- Identified session cookie in HTTP headers

## Cookie Extraction
- Located session cookie value from captured packets
- Copied cookie name and value

## Session Hijacking
- Opened browser with EditThisCookie plugin
- Injected captured session cookie
- Refreshed page and gained access as authenticated user

## Result
- Successfully accessed user account without credentials
- Confirmed session hijacking vulnerability

## Mitigation
- Enforce HTTPS (TLS)
- Set Secure and HttpOnly cookie flags
- Implement session expiration and regeneration
- Use HSTS
-
-
- ![seshij2](https://github.com/user-attachments/assets/7a11d980-df9a-40b4-9cd2-c8bec6e934dc)
![seshij](https://github.com/user-attachments/assets/13f6f121-fcde-48d1-9231-84fae1ca4f87)
