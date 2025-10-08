Day 23: Introduction to Ethical Hacking

1. What is Ethical Hacking?
Ethical hacking involves legally exploiting systems, networks, or applications to discover vulnerabilities with the owner's explicit permission. The goal is to identify and fix security weaknesses before malicious attackers can exploit them.

Key Principle: Performing the same actions as a malicious hacker, but with authorization and for a defensive purpose. Without permission, it is illegal and considered a cybercrime.

2. The Importance of Ethical Hacking
- Proactive Defense: Finds and fixes security holes *before* they are exploited by attackers.
- Protects Data: Helps prevent data breaches and theft of sensitive information.
- Improves Security Posture: Provides a real-world assessment of an organization's security controls.
- Meets Compliance: Many regulations and standards require periodic security testing.

3. The 5 Phases of Ethical Hacking

Phase 1: Reconnaissance (Information Gathering)
- Goal: To passively gather intelligence about the target and create a blueprint.
- Activities: Collecting information on IP addresses, domain details, network structure, and employees.
- Tools: 'recon-ng', 'Maltego' (for mapping relationships), public records, social media.

Phase 2: Active Scanning
- Goal: To actively probe the target for vulnerabilities and weak points.
- Activities: Scanning for open ports, running services, and potential vulnerabilities.
- Tools: 'Nmap' (network scanning), 'Wireshark' (traffic analysis), 'Aircrack-ng' (wireless network testing).

Phase 3: Gaining Access
- Goal: To exploit identified vulnerabilities to gain entry into the target system.
- Activities: Using exploits to breach systems, such as exploiting a software bug or weak password.
- Tools: Exploit frameworks like 'Metasploit', password cracking tools like 'John the Ripper'.

Phase 4: Maintaining Access
- Goal: To ensure continued access to the compromised system.
- Activities: Installing backdoors or rootkits to create a persistent presence.
- Purpose: Demonstrates the potential for long-term damage if a real attacker gains access.

Phase 5: Covering Tracks
- Goal: To remove all evidence of the testing activities.
- Activities: Clearing logs, deleting created files, and uninstalling tools.
- Purpose: Shows the organization what evidence would be left behind in a real attack and tests their detection capabilities.
