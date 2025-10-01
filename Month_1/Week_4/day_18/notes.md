Day 18: Incident Response Case Study Analysis
Objective
To analyze real-world cybersecurity incidents and understand how Incident Response (IR) teams apply the IR lifecycle in different scenarios, from detection to lessons learned.

Case Study 1: Business Email Compromise (BEC) & Payment Fraud
Source: "Cyber Security Incident Response - How SOC Responds, See LIVE" by BlackPerl (https://youtu.be/IqxQktruIwk?si=o4Lq3aQqUEdk7TmE)

Incident Summary
A sophisticated Business Email Compromise (BEC) attack led to a successful financial fraud. Attackers impersonated a trusted third-party vendor to redirect invoice payments to accounts they controlled.

Attack Chain & IR Response
Initial Reconnaissance & Weaponization:

Attackers sent a fake phishing email to test the target. This email was reported by an employee, raising the first alert.

Establishing Foothold & Persistence:

Using credentials likely obtained from a previous breach or phishing attack, the attackers gained legitimate login access to a trusted user's or admin's email account.

Actions on Objectives (The Fraud):

From the compromised account, the attackers sent legitimate-looking emails requesting a change in payment details for an upcoming invoice.

The finance team, trusting the email's source, processed the payment, sending the funds directly to the attacker's bank account.

Incident Response Actions:

The IR team worked backwards from the alert, analyzing logs to establish a timeline of events from the initial breach to the fraudulent transaction.

Focus was on identifying the source of compromise and containing the account access.

Key Takeaway
This case highlights that even a single set of compromised credentials can bypass many technical defenses. It underscores the critical need for multi-factor authentication (MFA) and out-of-band verification (e.g., a phone call) for any financial transaction changes.

Case Study 2: Web Application Attack on Government Services
Source: "Cyber Security Incident Response - An Island State Case Study" - Vanuatu Government (https://conference.apnic.net/52/assets/files/APBS588/cyber-security-incident-response-an-island-state-case-study.pdf)

Incident Summary
Attackers compromised a government web application by uploading malicious code with admin privileges, leading to a significant disruption of public services.

Attack Chain & IR Response
Initial Access:

Attackers gained administrative-level access to the web application's backend.

Impact:

Deployed malicious code that disrupted multiple critical government services, causing widespread outages.

Incident Response Lifecycle in Action:

Detection & Analysis: Identified the unauthorized code and the point of entry.

Containment: Isolated the affected web servers to prevent the disruption from spreading.

Eradication: Removed the malicious code from the system.

Recovery: Restored services from clean backups and brought systems back online.

Lessons Learned: The report detailed the need for stronger access controls, regular vulnerability patching, and improved monitoring for web applications.

Key Takeaway
This case demonstrates a direct attack on system availability (CIA Triad). It shows the importance of robust access management (principle of least privilege) and having a tested recovery plan to restore operations quickly after an attack.

Overall Conclusion from Day 18
No two incidents are the same: Attack vectors range from social engineering (BEC) to technical exploitation (web app hack).

The IR lifecycle is universal: Despite different attacks, the core phases of Preparation, Detection, Containment, Eradication, Recovery, and Lessons Learned were clearly applicable in both cases.

Proactive measures are crucial: MFA, employee training, strict access controls, and backups are repeatedly identified as key defensive layers that could prevent or mitigate attacks.