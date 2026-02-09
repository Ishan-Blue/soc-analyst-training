Summary:
Suspicious outbound network traffic detected from FIN-LAPTOP-12 associated with user alex.khan@company.com
, indicating possible command-and-control communication.

Reason for Alert:
Repeated outbound connections every 60 seconds to IP 185.203.118.44 over port 443, which is flagged by threat intelligence as a known C2 server.

Risk Level:
High

Assessment:
The consistent beaconing pattern combined with threat intelligence confirmation strongly suggests malware attempting to communicate with a C2 server. Firewall traffic was allowed and the device was not isolated, increasing risk of further compromise.

Immediate Action:
Isolate the affected endpoint, block the destination IP at firewall and EDR level, collect memory and process data, and initiate malware scan.

Escalation:
Yes,escalate to L2 due to confirmed malicious C2 communication and potential endpoint compromise.
