Lab Report: Network Configuration & Firewall Rules in Cisco Packet Tracer
Objective
To design a basic network topology, configure IP addressing, and implement basic firewall rules to control traffic flow.

Lab Environment
Tool Used: Cisco Packet Tracer

Devices: Routers, Switches, PCs

Part 1: Basic Network Setup and IP Configuration
Topology 1: Segmented Network
I created a network to simulate two separate subnets connected by a router.

Layout:

One router.

Two switches, each connected to a different router interface.

Two PCs connected to each switch (total of 4 PCs).

Configuration:

Assigned IP addresses to all devices (PCs and router interfaces).

Each switch and its connected PCs formed a separate subnet, with the router's interface acting as the default gateway for that subnet.

Verification:

Successfully tested connectivity between devices within the same subnet and across different subnets via the router. This confirmed correct IP addressing and routing.

Topology 2: Simple Network for Firewall Test
I created a simpler network to focus on firewall rules.

Layout:

One router.

One switch connected to the router.

Two PCs (PC1 and PC2) connected to the switch.

Configuration:

Assigned IP addresses from the same subnet to both PCs and the router interface. Verified connectivity with a successful ping.

Part 2: Implementing and Testing Firewall Rules
Action Taken on PC1:
I configured two inbound firewall rules on PC1:

Rule 1: DENY all ICMP traffic.

Rule 2: ALLOW all IP traffic.

Results and Analysis:
Ping Test (ICMP): When attempting to ping PC2 from PC1, the request failed. This is the expected result because the DENY ICMP rule explicitly blocked the ping packets, which use the ICMP protocol.

IP Address Lookup: I was still able to search for and find PC2's IP address from PC1. This worked because the ALLOW IP rule permitted general IP communication, which includes the address resolution protocols (like ARP) that operate at a lower layer than the specific ICMP block.

Conclusion:
This lab successfully demonstrated:

The ability to design and configure a functional multi-subnet network.

The practical effect of firewall rules: a specific deny rule (ICMP) overrides a general allow rule (IP).

How different network protocols (IP vs. ICMP) can be controlled independently by a firewall.

Next Steps
If connectivity permits, I will supplement this virtual lab by examining the security settings on my physical home router (MTN Homebox) to compare real-world device configuration with the simulated experience.