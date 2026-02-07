Summary:
Suspicious outbound network traffic detected from endpoint FIN-LAPTOP-23 at 22:18 UTC.

Reason for Alert:
The device initiated multiple outbound connections to a known malicious IP address over port 443.
The IP is associated with command-and-control (C2) infrastructure based on threat intelligence feeds.

Risk Level:
High

Investigation Details:
- Source Device: FIN-LAPTOP-23
- Source User: emma.johnson@company.com
- Destination IP: 91.215.85.17
- Destination Port: 443
- Traffic Pattern: Repeated beaconing behavior at regular intervals
- Device Behavior: Abnormal compared to baseline activity

Assessment:
The observed traffic pattern is consistent with possible malware infection attempting to communicate
with an external command-and-control server.

Immediate Action:
- Isolate the affected endpoint from the network
- Escalate incident to L2 SOC for malware investigation
- Initiate endpoint scan via EDR
- Block destination IP at firewall
- Review recent user activity and downloads

