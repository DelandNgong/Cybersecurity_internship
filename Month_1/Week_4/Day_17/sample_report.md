
Incident Report: TiC-2025-09

Date of Report: September 30, 2025
Status: Closed


1. Executive Summary
On September 29, a user's workstation was infected with malware after they opened a malicious email attachment. The incident was contained by isolating the affected machine. The malware was successfully removed, and the user's system was restored. No sensitive data was exfiltrated.

2. Incident Identification
-Incident ID: TiC-2025-09
-Title: Malware Infection via Phishing Email
-Severity: Medium
-Date/Time Discovered: 2025-09-29, 10:15 AM
-Reported By: Meh Kum (User), IT Help Desk

3. Timeline of Events
- 2025-09-29, 09:45 - User (Meh Kum) receives a phishing email titled "Urgent: Invoice Payment Required" and opens the attached file "invoice.pdf.exe".
- 2025-09-29, 10:15 - Antivirus alerts on multiple malware detection. User contacts Help Desk.
- 2025-09-29, 10:25 - Incident Response Team (IRT) is activated. The user's workstation is isolated from the network.
- 2025-09-29, 11:00 - IRT confirms the presence of a trojan malware.
- 2025-09-29, 14:30 - Malware is eradicated, and the system is restored from a clean backup.
- 2025-09-29, 15:00 - Workstation is reconnected to the network after verification.

4. Technical Details
-Attack Vector: Phishing email with a malicious executable attachment disguised as a PDF.
-Malware Type: Trojan
-Indicators of Compromise (IOCs):
  - File: invoice.pdf.exe
  - MD5 Hash: a1b2c3d4e5f678901234567890123456
  - Sender Email: fake.sender@malicious-domain.com
-Affected System: Workstation-PC-12 (User: Meh Kum)

5. Actions Taken
-Containment: Immediately disconnected Workstation-PC-12 from the network.
-Eradication: Ran antivirus scans and manually removed all traces of the malware.
-Recovery: Restored the system from a clean backup taken on September 29.
-Communication: Informed the user and relevant department heads.

6. Root Cause
The primary cause was a user being tricked by a sophisticated phishing email. A contributing factor was the lack of email filtering rules to block executable files attached to emails.

7. Lessons Learned & Recommendations
1. Recommendation: Implement an email filter to automatically block emails with executable attachments (.exe, .scr, etc.).
2. Recommendation: Conduct mandatory phishing awareness training for all employees within the next 30 days.
3. Recommendation: Ensure all workstations have anti-virus software with real-time protection enabled and updated.

Report Prepared By: Ngong Deland Ngong, Cybersecurity Intern
Date: September 30, 2025