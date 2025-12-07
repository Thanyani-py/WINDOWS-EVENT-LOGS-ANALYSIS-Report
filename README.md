# WINDOWS-EVENT-LOGS-ANALYSIS-Report
This repository contains a Windows Event Logs analysis report focused on identifying the actions of an attacker within a compromised system before they accessed the file server. The investigation was conducted using Event Viewer and targeted key security-related Event IDs to reconstruct the attacker’s activity.

The process began with locating the most recently created user account by filtering for Event ID 4720, which revealed the malicious account named Hacked. I then identified the user account responsible for creating it by reviewing the associated metadata in the event details.

Next, I confirmed when the account was enabled by filtering for Event ID 4722, allowing me to determine the exact date and time the attacker activated the account. Finally, by adding Event ID 4724, I verified that a password reset attempt occurred, indicating further unauthorized manipulation of the account.

This analysis demonstrates practical skills in log filtering, event correlation, attacker activity reconstruction, and Windows security monitoring. It reflects my growing experience in defensive security and log analysis.
