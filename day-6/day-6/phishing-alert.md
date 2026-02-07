Summary:
Suspicious phishing email detected targeting user david.wilson@company.com at 09:22 UTC.

Reason for Alert:
An email with the subject "Urgent: Password Expiry Notice" was received from an external sender
spoofing the IT support team. The sender domain was newly registered and contained an embedded link.

Risk Level:
Medium

Investigation Details:
- Targeted User: david.wilson@company.com
- Sender Name: IT Support
- Sender Email: it-support@company-secure.com
- Domain Age: 2 days
- Email Content: Urgent password reset request
- Embedded Link: Present
- Link Clicked: No

Assessment:
The email exhibits multiple phishing indicators including spoofed sender identity, newly registered
domain, urgency in messaging, and embedded link.

Immediate Action:
- No escalation required as the link was not clicked
- Block sender domain at email gateway
- Remove email from other mailboxes if delivered internally
- Educate the user on phishing awareness
