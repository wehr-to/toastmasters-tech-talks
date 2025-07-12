Title: Practically Detect and Automatically Respond Toward Contain Incidents

Delivery by a practitioner: Clear objective points for technical rehearsal.

* We cannot watch alerts all the time, but we can find and then contain automatically to handle noise.
* We need a way for responding faster to “breaches” that “move fast” without adding unnecessary manual steps.
“Today, I’ll walk through in how to use detection rules, automated response playbooks. Practical tools reduce repetitive manual work.”

* With rule-based, baseline, and correlation-based detection, use EDR, NDR, and SIEM tools.

Examples:

* Find process injection upon each endpoint.
* Note strange migrations for VLANs laterally.
* Flag locations from unexpected off-hours logins.

* Define automated responses following steps tied to clear triggers detected.

Examples:

* Quarantine endpoints.
Rotate secrets for improved security. Act when unusual entry occurs.
Flagged IP addresses get blocked automatically.

* Activity that is legitimate should not be over-blocked at all.
* Alert and partial containment in addition to full containment are actions that are tiered.
Keep those high-impact actions behind a human review until confidence within detections has been established.
You must regularly tune the response playbooks and detection rules.

Cortex XSOAR remains a tool. Its goal involves automation of workflows.
* Use CrowdStrike for both containment and for detection.
* Write in Python scripts that are for account disabling, and for endpoint isolation, and for secret rotation.
* Custom detection tuning uses both Sysmon and also Sigma rules.

* “Today we covered handling false positives, coupled with automated response playbooks, practical detection.”
* “Without burning out on repetitive tasks, automation as well as response workflows help for us to keep up with incidents.”
* “If you're testing of this, start at the time when you automate one response task in your lab so you can see the place where that saves some time and consistency that improves.”

