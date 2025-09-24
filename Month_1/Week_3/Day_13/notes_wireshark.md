Day 13: Introduction to Wireshark & Network Traffic Analysis
1. What is Wireshark?
Wireshark is a network protocol analyzer (a "packet sniffer"). It captures data packets traveling through a network interface, allowing you to inspect their contents in detail. It is an essential tool for:

Network Troubleshooting: Identifying why connections are failing.

Security Analysis: Detecting malicious activity on a network.

Learning: Understanding how network protocols actually work.

2. Wireshark Interface Breakdown
The interface is divided into three main panes that show the encapsulation of data according to the OSI model.

Packet List Pane (Top)
A summary of all captured packets. Key columns:

No.: The packet number in the capture.

Time: When the packet was captured relative to the start.

Source: The IP address of the sender.

Destination: The IP address of the receiver.

Protocol: The application-layer protocol (e.g., DNS, TCP, HTTP).

Info: A brief description of the packet's purpose.

Packet Details Pane (Bottom left)
Shows the selected packet broken down by protocol layers (like peeling an onion).

Frame: The raw data as captured from the network.

Ethernet II (Data Link Layer): Contains the source and destination MAC addresses for the local network segment.

Internet Protocol Version 4 (Network Layer): Contains the source and destination IP addresses for routing across networks.

Transmission Control Protocol (Transport Layer): Manages the connection between applications using port numbers.

Application Protocol (e.g., DNS): The actual content of the message.

Packet Bytes Pane (Bottom right)
The raw data of the packet in hexadecimal and ASCII. Used for advanced analysis.

3. Key Network Protocols Observed
DNS (Domain Name System) - The Internet's Phonebook
Purpose: Translates human-readable domain names (e.g., web.whatsapp.com) into machine-readable IP addresses (e.g., 157.240.1.53).

How it works: Your computer sends a DNS Query to a DNS server (like 8.8.8.8). The server replies with a DNS Response containing the IP address.

Wireshark Filter: dns

TCP (Transmission Control Protocol) - The Reliable Messenger
Purpose: Establishes a reliable, connection-oriented session between two applications. Ensures data arrives completely and in order.

The Three-Way Handshake: The process to establish a TCP connection:

SYN (Synchronize): The client sends a packet with the SYN flag set to initiate a connection.

SYN-ACK (Synchronize-Acknowledge): The server acknowledges the request (ACK) and agrees to synchronize (SYN).

ACK (Acknowledge): The client acknowledges the server's response. The connection is now ESTABLISHED.

Wireshark Filter: tcp

Google Public DNS (8.8.8.8)
A free, global DNS resolution service provided by Google. Many systems use it as a fast and reliable alternative to an ISP's default DNS servers.

4. Hands-On Lab: Analyzing a DNS Query
Scenario:
I captured traffic while my computer needed to find the IP address for WhatsApp's web service.

Observation in Wireshark:
After applying the dns filter, I observed a clear conversation:

DNS Query:

Source: My Local IP

Destination: 8.8.8.8

Protocol: DNS

Info: Standard query A web.whatsapp.com

Translation: "Hey Google DNS, what is the IP address for 'web.whatsapp.com'?"

DNS Response:

Source: 8.8.8.8

Destination: My Local IP

Protocol: DNS

Info: Standard query response A 157.240.1.53

Translation: "The IP address for 'web.whatsapp.com' is 157.240.1.53."

Key Takeaway from the Lab:
This simple capture demonstrates the critical first step of almost all internet activity: the DNS lookup. Before any secure connection (HTTPS) can be established, the destination must first be found via DNS.

5. Essential Wireshark Tips
Use Filters: They are crucial for reducing noise. Examples:

ip.addr == 192.168.1.105 (Show all traffic to/from my IP)

dns (Show only DNS packets)

tcp.port == 80 (Show traffic using HTTP port 80)