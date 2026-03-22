#Alert: A suspicious phishing email with a possible account compromise

Severity: low

Indicators:
- Suspicious subject line(inheritance scam, fake offers)
- Untrusted sender domain (trendymillineryco.me)
- Social engineering language requesting sensitive information
- Unusual outbound emails from internal account following the receipt of the phishing email

Investigation:
- Queried Siem (Splunk) for the sender and recipient activity
- Analyzed inbound email logs to identify further phishing characteristics
- Pivoted to recipient account acticity to find suspicious outbound emails sent shortly after initial email

Conclusion: True Positive - Phishing with potential account compromise

Actions:
- Block the sender domain
- Temporarily disable the users account
- Educate the user via training if applicable
- Initiate a password reset for the affected account





