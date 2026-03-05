Security Operations Center (SOC) Incident Report Template

Incident ID:
Alert Name:
Date:
Time (UTC):
Severity: Low / Medium / High / Critical
Status: Open / Contained / Escalated / Closed
Analyst:

1. Executive Summary

Provide a concise 3–5 sentence summary describing:
What triggered the alert
What activity was observed
Whether compromise occurred
Final outcome

Example structure:
On [date], the SOC received an alert for [alert type]. Investigation revealed [brief finding]. The activity was classified as [malicious/suspicious/benign]. Appropriate containment actions were taken and the incident was [status].

2. Alert Details
Field	Value
Data Source	(Firewall / EDR / SIEM / Email Gateway / Proxy)
Detection Rule	
Source IP	
Source Hostname	
Source User	
Destination IP	
Destination Domain	
Destination Port	
Application	
Protocol	
Action Taken	(Blocked / Allowed / Detected)
3. Timeline of Events
Time	Event
HH:MM	Initial alert generated
HH:MM	Analyst began triage
HH:MM	Additional activity observed
HH:MM	Containment actions initiated
HH:MM	Incident resolved

Focus on clarity and chronological flow.

4. Indicators of Compromise (IOCs)
List technical artifacts identified during investigation.
Network Indicators
IP Address:
Domain:
URL:
Port:

Host-Based Indicators
File Hash (SHA256):
File Name:
Process Name:
Registry Key:
Command Line:

Email Indicators (if applicable)
Sender:
Reply-To:
Subject:
Attachment Name:
Embedded Link:

5. Investigation & Analysis
Document your investigative reasoning.
Include:
Log review findings
Correlated alerts
EDR telemetry analysis
Authentication log review
DNS lookups
Process tree analysis
User activity validation

Explain:
What was suspicious?
What ruled out false positives?
What evidence confirmed or denied compromise?

6. MITRE ATT&CK Mapping

Map observed behavior to the MITRE ATT&CK.
Example:
Initial Access – Phishing (T1566)
Execution – User Execution (T1204)
Command and Control – Web Protocols (T1071.001)
Credential Access – Input Capture (T1056)

7. Impact Assessment
   
Assess:
Was data accessed or exfiltrated?
Were credentials compromised?
Was lateral movement observed?
Were additional systems affected?
State clearly:
No evidence of compromise observed
or
Confirmed account compromise

8. Containment & Remediation
Immediate Actions
Blocked IP/domain
Isolated endpoint
Disabled user account
Forced password reset
Revoked sessions
Malware removed
Long-Term Recommendations
Patch vulnerable systems
Improve detection rule
Enable MFA
User awareness training
Threat hunting for related IOCs

9. Root Cause Analysis

Describe:
How the incident originated
Control gaps identified
Whether existing security controls worked as intended
Example:
The firewall successfully blocked the outbound request; however, the user was exposed to phishing content prior to enforcement.

10. Lessons Learned
What worked well?
What could be improved?
Detection gaps?
Process improvements?

11. Analyst Reflection 

This section is excellent for GitHub and interviews.
Highlight:
Investigative methodology
Cross-log correlation
Risk evaluation skills
ATT&CK mapping knowledge

Undertanding of containment priorities
