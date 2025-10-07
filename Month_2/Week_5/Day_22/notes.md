 Day 22: Introduction to Nmap & Initial Network Scanning

1. What is Nmap?
Nmap (Network Mapper) is a free, open-source tool used for network discovery and security auditing. It helps discover devices on a network, find open ports, and identify services running on those ports.

2. Basic Nmap Scan & Results
Performed a basic Nmap scan on my local router/gateway using the command: nmap -T4 -A -v 192.168.100.1

3. Scan Results Analysis
- Scanned 1000 common ports
- 994 ports were closed (normal and good - means services not accessible)
- 6 ports showed interesting states:

PORT 21/TCP (FTP)
- State: Filtered
- Meaning: Port is likely blocked by a firewall
- Note: FTP is insecure file transfer protocol

PORT 22/TCP (SSH)
- State: Open
- Meaning: Secure Shell service is running
- Note: Used for remote administration, common attack target

PORT 23/TCP (TELNET)
- State: Filtered
- Meaning: Port blocked by firewall
- Note: Telnet is insecure (sends passwords in plain text)

PORT 53/TCP (DOMAIN)
- State: Open
- Meaning: DNS service running
- Note: Normal for router to handle DNS queries

PORT 80/TCP (HTTP)
- State: Open
- Meaning: Web service running
- Note: http is not secure, https is.

PORT 5080/TCP
- State: Open
- Service: Unknown (Nmap guessed "onscreen")
- Note: Could be additional admin interface or service

4. Key Learning
This was a network discovery scan showing what services are running, not a vulnerability assessment.

The scan successfully identified open "doors" on the network but didn't test the strength of the "locks."
