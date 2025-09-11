Day 4: Interactive Threat Identification
1. Phishing Simulation Exercise
Activity: Completed Google's Phishing Quiz to practice identifying malicious emails.

Key Red Flags Identified:

Look-alike Email Addresses: Sender addresses that mimic legitimate companies but have subtle spelling errors or wrong domains.

Unsecured URLs: Links that do not use http:// or have suspicious domain names.

Urgent & Unusual Requests: Messages pressuring the recipient to click a link or provide sensitive information like verification codes, which legitimate services rarely ask for via email.

Takeaway: Consistent verification of sender addresses and URLs is a critical first line of defense against phishing attempts.

2. Real-World Case Study Analysis
Article Analyzed: "18 Popular Code Packages Hacked, Rigged to Steal Crypto" by KrebsOnSecurity.

Incident Summary
A developer was successfully phished via an email instructing him to update his two-factor authentication (2FA) settings. The attackers used the stolen credentials to gain access to his account and inject malicious code into popular software libraries (npm packages) he maintained.

Attack Vectors & Impact
Initial Vector: Phishing. A carefully crafted email that "seemed legit" bypassed the developer's vigilance.

Attack Type: Supply Chain Attack. By compromising a trusted developer's account, the attackers poisoned software dependencies used by countless other projects.

Goal: The malicious code was designed to stealthily manipulate cryptocurrency transactions and steal funds.

Containment: The attack was discovered and contained by a dedicated team monitoring software updates for suspicious activity.

Key Lessons
Sophisticated Social Engineering: Phishing emails are becoming highly targeted and convincing, capable of tricking even security-conscious individuals.

The Supply Chain is a Weak Link: An attack on a single developer can have a massive downstream impact on thousands of users and organizations, highlighting the critical risk of third-party dependencies.

The Importance of Monitoring: Proactive monitoring of software repositories and updates is essential for early detection and mitigation of such threats.