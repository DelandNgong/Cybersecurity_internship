Day 13: Wireshark DNS Traffic Analysis
What I Studied Today
The main focus was on practical DNS analysis using Wireshark. I learned how to capture and interpret the DNS queries my computer makes in real-time. I also reviewed the definitions and roles of other key networking protocols for context.

Wireshark Navigation - Key Points
Display Filter is Essential: The most important tool for this task. I used the filter dns to isolate only DNS traffic from the capture.

Reading the Panels:

Packet List (Top): Gives a quick overview. The Info column summarizes the DNS conversation.

Packet Details (Bottom Left): Allows me to drill down into the layers of a packet - Frame, Ethernet, IP, UDP, and finally the DNS section with the query/response details.

Byte View (Bottom Right): Shows the raw data; less frequently used for initial analysis.

Protocols Involved & Their Definitions
Protocols in my DNS Capture:

DNS (Domain Name System): The core protocol being analyzed. It translates domain names (like web.whatsapp.com) into IP addresses.

UDP (User Datagram Protocol): DNS primarily uses UDP port 53 for its fast, connectionless queries. It's simpler than TCP but doesn't guarantee delivery.

IP (Internet Protocol): The fundamental protocol for routing packets across networks. It uses IP addresses (like 192.168.100.16 and 8.8.8.8) to get data from source to destination.

Ethernet: The dominant protocol for local area networks (LANs). It handles the physical transmission of data frames between devices on the same network segment.

Other Key Protocols:

ARP (Address Resolution Protocol): Used to map an IP address to a physical MAC address on a local network. For example, my computer would use ARP to find the MAC address of the router before sending the DNS packet to it. This happens before the DNS query in the capture.

TCP (Transmission Control Protocol): A connection-oriented protocol that ensures reliable, ordered delivery of data. It's used by protocols that require high reliability, like HTTP/S, SSH, and FTP. DNS can use TCP for large responses or zone transfers.

HTTP/HTTPS (Hypertext Transfer Protocol/Secure): The protocols used for loading websites. HTTPS is the encrypted version. A DNS query is the first step to accessing a website; once the IP is known, my browser would then establish a TCP connection and send an HTTP/HTTPS request to that IP. This happens after the DNS response.

Analysis of My Capture

After opening a capture on wireshark, I got an influx of network traffic , iformation which did not make sense at firs. Then I opened whatsapp in my browser, came back and stoped the capture. I filtered the traffic using dns (as seen on my screenshot or wireshark capture file), the i could see the request from my ip to google's 8.8.8.8, the a couple of responses later on. This was an exciting step for to start making sense out of what was going one.

Conclusion
This session was a practical application of using Wireshark for monitoring network data, and get security related information.