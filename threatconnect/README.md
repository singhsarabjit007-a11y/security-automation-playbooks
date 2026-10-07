# ThreatConnect Playbooks

Resilient ThreatConnect playbook templates for common enrichment, sandboxing, and phishing-intake workflows. Each template has validation gates, clearer operational logging, and explicit failure paths where supported by its integrated application.

## Included playbooks

Each playbook has its own directory with a local README and importable file.

- [ATD Malware Detonation](atd/)
- [Hash Intelligence via Email](email-hash/)
- [IPQS IP Reputation](ip-reputation/)
- [IPQS URL Reputation](url-reputation/)
- [Phishing Intake](phishing/)
- [VirusTotal Intelligence Search](virustotal/)
- [VMRay Submission and IOC Collection](vmray/)

## Validation and configuration

All included PBX files were parsed as JSON and checked for unresolved workflow job references. Each PBXZ package was opened and its embedded playbook was parsed successfully.

Before import, update organization-specific configuration: API keys, owners, mailbox settings, integration endpoints, email recipients, and security policy values. Review all imported playbooks in a non-production organization before enabling them in production.
