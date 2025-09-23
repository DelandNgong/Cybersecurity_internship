Day 2: Deep Dive into the CIA Triad

#Core Principle
The CIA Triad (Confidentiality, Integrity, Availability) forms the foundation of cybersecurity. Most attacks aim to exploit one or more of these principles.

1. Confidentiality
Goal: Protect information from unauthorized access.
-Least Privilege Principle: Access is granted on a strict need-to-know basis.
#Implementation:
-Classification: Categorizing data to determine access levels.
-Access Control: Mechanisms like Identification, Authentication, and Authorization.
-Encryption: Converting plaintext to ciphertext, rendering data useless to unauthorized parties even if accessed.

2. Integrity
Goal: Ensure data is accurate, trustworthy, and unaltered.
-Prevention of Tampering: Policies and controls to prevent unauthorized modification of data (in transit or at rest).
#Implementation:
-Access Control: Restricting write/modify permissions.
-Hashing: Generating a unique digital fingerprint (hash) for data. Any change to the data alters this hash, alerting us to tampering.

3. Availability
Goal: Ensure information and systems are accessible when needed by authorized users.
-Maintaining Uptime: Mitigating disruptions to service.
#Implementation:
-Redundancy: Backup systems to take over if primary ones fail.
-Backups: Copies of data to restore after an incident.
-Common Threats: Denial-of-Service (DoS/DDoS) attacks, system-crashing malware.


#Balancing the Triad & Real-World Observations

#Prioritization in Practice
The priority of each principle depends on the system's purpose:
-Public Services: Prioritize Availability (e.g., a public news website).
-Financial Systems: Prioritize Integrity (e.g., banking databases).
-Classified Communications: Prioritize Confidentiality (e.g., government secrets).

#Key Takeaways from Attack Analysis
-Primary Target: Confidentiality is the most frequently targeted principle in recent attacks (e.g., data breaches, leaks).
-Least Targeted: Integrity attacks (direct data tampering) are less common but highly damaging.
-Root Cause: Most successful attacks are not due to advanced "genius" hacking but often stem from:
  -Simple human errors.
  -Weak security links (e.g., poor password hygiene).
  -Inadequate security processes and configurations.

#Emerging Challenges
The classic CIA model is tested by modern threats like:
-Insider Threats: Authorized users violating trust.
-IoT Interconnectedness: The vast amount of data and access points creates a massive attack surface that is difficult to secure completely.