1. Setting Up a Basic Home Network
The core components of a simple home network are:

Modem: Provided by your Internet Service Provider (ISP). Its job is to bring internet connectivity into your home and convert it into a usable digital signal.

Router: Connected to the modem via an Ethernet cable. This device assigns IP addresses to your devices (DHCP), manages traffic between them, and creates your local network.

Switch (Optional): Used to add more physical Ethernet ports to your network if you have many wired devices.

Wireless Access Point (WAP) (Optional): Often built into the router. Provides Wi-Fi connectivity.

Configuration Process:

Connect a device to the router (via Ethernet or Wi-Fi).

Access the router's admin panel by typing its IP address (e.g., 192.168.1.1) into a web browser.

Critical First Steps:

Change the default administrator username and password.

Set a strong, unique password for your Wi-Fi network.

Personal Implementation:
I use an MTN Homebox, which is an all-in-one "gateway" device that combines the functions of a modem, router, and wireless access point. I configured it by accessing its admin panel via the browser to set a strong admin password and Wi-Fi password.

2. Firewall Fundamentals
A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It acts as a barrier between a trusted internal network and untrusted external networks (like the internet).

Types:

Hardware Firewall: A physical device (often part of a router) that protects the entire network.

Software Firewall: An application installed on an individual device (e.g., Windows Firewall) that protects only that device.

Windows Firewall Rules:

Inbound Rules: Control incoming traffic to your computer from the network or internet. ("You must match the rule to connect to me.")

Outbound Rules: Control outgoing traffic from your computer to the network or internet. ("I must match the rule to be allowed to send data out.")


Rule Configuration:
Firewalls come with predefined rules for common applications and services. Users can also create custom rules to:

Allow or block a specific program.

Allow or block traffic on a specific port.

Create rules based on IP addresses or protocols.

Note: I explored the Windows Firewall interface but did not modify any default rules, as my current personal use case does not require custom configurations and altering them without a need could cause unnecessary connectivity issues.