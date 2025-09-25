Day 14: Wireshark Analysis & CS50 Introduction
1. Hands-On Wireshark: Analyzing Sample Captures
Today involved analyzing pre-captured traffic files to understand specific protocols without network noise.

A. ARP (Address Resolution Protocol) Analysis
Objective: To observe how devices on a local network find each other's MAC addresses.

Packet Analysis:

Frame 1: ARP Request (Broadcast)

Time: 0.000000 seconds

Source: Device with IP 192.168.30.26 and MAC 10:e7:c6:09:f7:?? (likely the router)

Destination: Broadcast to the entire network (FF:FF:FF:FF:FF:FF)

Message (literally): "Who has the IP address 192.168.30.3? Please tell me your MAC address."

Frame Length: 42 bytes.

Protocol: ARP over Ethernet.

Frame 2: ARP Reply (Unicast)

Time: 0.001112 seconds

Source: Device with IP 192.168.30.3 and MAC 10:8f:fe:95:97:00

Destination: Directly to the requester (10:e7:c6:09:f7:??)

Message (literally): "I have the IP 192.168.30.3. My MAC address is 10:8f:fe:95:97:00."

Frame Length: 60 bytes.

Key Takeaway: ARP is a fundamental local network protocol that maps IP addresses to physical MAC addresses. The request is a broadcast (shouted to everyone), and the reply is a unicast (spoken directly back to the asker).

B. IPv4 & ICMP Analysis (Ping)
Objective: To observe the Internet Control Message Protocol (ICMP) used by the ping command.

Packet Analysis:

Scenario: A series of Echo (ping) Requests and Echo Replies.

Protocol: ICMP, which runs on top of IPv4.

How it works:

The source device sends an ICMP Echo Request packet to a target IP address.

If the target device is online and reachable, it responds with an ICMP Echo Reply.

Purpose: Used to test connectivity and latency between two network devices.

Key Takeaway: ICMP is a core diagnostic tool. Unlike TCP, it is connectionless (no handshake), making it fast for simple queries like checking if a host is "alive."

2. CS50's Introduction to Cybersecurity - Assignment 0
Activity: Completed Assignment 0 of the CS50 cybersecurity course on edX.

Focus: This assignment typically serves as an introduction to core security mindset concepts, such as:

Identifying threats in realistic scenarios (e.g., phishing emails, social engineering).

Understanding the importance of verification and skepticism.

Securing accounts (such as using passwords, mfa etc)

Applying the CIA Triad (Confidentiality, Integrity, Availability) to simple cases.

Benefit: This provided a structured, academic reinforcement of the fundamental principles covered in the first two weeks of my internship.

3. Summary
Day 14 was dedicated to deepening practical skills through targeted protocol analysis with Wireshark (ARP, ICMP) and strengthening foundational knowledge through a formal course assignment. This combination of open-ended exploration and guided learning is solidifying my understanding of how networks communicate.