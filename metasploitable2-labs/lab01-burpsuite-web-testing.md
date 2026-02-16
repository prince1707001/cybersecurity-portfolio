# Lab 01 – Web Application Security Testing using Burp Suite

## Objective
Perform web application security testing in a controlled lab environment using Burp Suite to identify common vulnerabilities.

## Environment
- Attacker: Kali Linux
- Target: Intentionally vulnerable lab application (local VM)
- Tool: Burp Suite Community Edition
- Network: Isolated lab network

## Testing Performed

### 1. Intercepting HTTP Requests
- Configured browser proxy to route traffic through Burp
- Intercepted login request
- Analyzed HTTP headers and parameters

### 2. Parameter Manipulation
- Modified request parameters in Repeater
- Tested for input validation weaknesses

### 3. SQL Injection Testing
- Observed server response behavior
- Identified lack of input sanitization

### 4. Session Handling Analysis
- Reviewed session cookies
- Checked for Secure and HttpOnly flags

## Findings
- Improper input validation
- Weak session configuration
- Potential SQL injection vulnerability

## Defensive Recommendations
- Implement server-side validation
- Use prepared statements
- Enforce Secure and HttpOnly cookies
- Apply Web Application Firewall (WAF)

