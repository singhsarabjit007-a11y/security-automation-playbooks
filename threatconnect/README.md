# ThreatConnect Playbooks

Resilient ThreatConnect playbook templates for common enrichment, sandboxing, and phishing-intake workflows. Each template has validation gates, clearer operational logging, and explicit failure paths where supported by its integrated application.

## Included playbooks

| Playbook | Purpose |
| --- | --- |
| `Resilient Hash Intelligence via Email.pbx` | Extracts MD5, SHA-1, and SHA-256 values from email, queries ThreatConnect owners, and returns results to the sender. |
| `Resilient ATD Malware Detonation.pbx` | Submits a tagged malware document to McAfee/Trellix ATD and stores severity-mapped File indicators. |
| `Resilient IPQS Reputation Enrichment.pbxz` | Enriches IP-address indicators using IPQualityScore reputation data. |
| `Resilient IPQS URL Reputation Enrichment.pbxz` | Enriches URL indicators using IPQualityScore reputation data. |
| `Resilient Phishing Intake Playbook.pbx` | Validates, password-protects, and stores submitted phishing-email attachments. |
| `Resilient VirusTotal Intelligence Search.pbx` | Runs a validated, paginated VirusTotal Intelligence search and creates File indicators. |
| `Resilient VMRay Submission and Results.pbx` | Submits samples to VMRay and ingests its IOC output after the asynchronous analysis completes. |

## Validation and configuration

All included PBX files were parsed as JSON and checked for unresolved workflow job references. Each PBXZ package was opened and its embedded playbook was parsed successfully.

Before import, update organization-specific configuration: API keys, owners, mailbox settings, integration endpoints, email recipients, and security policy values. Review all imported playbooks in a non-production organization before enabling them in production.
