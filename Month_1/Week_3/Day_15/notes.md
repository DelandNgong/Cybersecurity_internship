Day 15. Mini Packet Tracer project.
1. Project Objective
To design a segmented network and implement strict firewall rules to completely isolate a specific host, preventing both basic discovery (ping) and all other IP communication.

2. Network Design and Configuration
Topology Created:
1 Router: Acting as the core gateway and firewall.

2 Switches: Connecting devices within their respective segments.

5 PCs:

Segment 1 (Switch0): PC0 and PC1

Segment 2 (Switch1): PC2, PC3, and PC4

IP Addressing Scheme:
A subnetting strategy was implemented to logically separate the two network segments.

Segment 1

PC0: 192.168.1.10

PC1: 192.168.1.11

Router Interface: 192.168.1.1

Segment 2

PC2: 192.168.2.10

PC3: 192.168.2.11

PC4 (The "Secret" Host): 192.168.2.12

Router Interface: 192.168.2.1

Initial Connectivity Test:
Before applying firewall rules, connectivity was verified. PCs within the same segment could communicate, and the router successfully routed traffic between the two subnets.

3. Firewall Rule Implementation: Host Isolation
The goal was to make PC4 unreachable from any other device on the network.

Security Policy Enforced:
Rule 1: Deny ICMP (Internet Control Message Protocol) traffic to PC4.

Rule 2: Deny all other IP traffic to PC4.

4. Results and Verification
After applying the firewall rules, tests were conducted:

Ping Test (ICMP): Attempts to ping PC4 from any other PC (PC0, PC1, PC2, PC3) failed. The ICMP Echo Requests were blocked by the router.

Connection Test (IP): Attempts to access PC4  searching by IP, attempting a connection also failed because all general IP traffic was denied.

Conclusion: PC4 was successfully isolated from the rest of the network. It could not be discovered or communicated with, effectively making it "invisible" and secure from unauthorized access.

5. Key Learnings
Network Segmentation: Dividing a network into subnets is the first step toward implementing granular security controls.

Firewall Rule Specificity: The combination of a specific protocol deny (icmp) followed by a broad protocol deny (ip) is an effective way to block all access to a host.