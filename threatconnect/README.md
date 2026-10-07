# ThreatConnect Playbooks

Resilient ThreatConnect playbook templates for common enrichment, sandboxing, and phishing-intake workflows. Each template has validation gates, clearer operational logging, and explicit failure paths where supported by its integrated application.

## Included playbooks

Each playbook has its own directory with a local README and importable file.

- [ATD Malware Detonation](atd-malware-detonation/)
- [Hash Intelligence via Email](hash-intelligence-email/)
- [IPQS IP Reputation](ipqs-ip-reputation/)
- [IPQS URL Reputation](ipqs-url-reputation/)
- [Phishing Intake](phishing-intake/)
- [VirusTotal Intelligence Search](virustotal-intelligence-search/)
- [VMRay Submission and IOC Collection](vmray-submission-ioc-collection/)

## Validation and configuration

All included PBX files were parsed as JSON and checked for unresolved workflow job references. Each PBXZ package was opened and its embedded playbook was parsed successfully.

Before import, update organization-specific configuration: API keys, owners, mailbox settings, integration endpoints, email recipients, and security policy values. Review all imported playbooks in a non-production organization before enabling them in production.
