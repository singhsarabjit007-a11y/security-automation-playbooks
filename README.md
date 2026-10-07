# Security Automation Playbooks

A public collection of reusable security-automation workflows. Each playbook is packaged as an importable workflow definition with a diagram and documentation that explains its purpose, inputs, outputs, and external services.

## Repository layout

| Directory | Contents |
| --- | --- |
| [`tines`](tines/) | Tines Stories for enrichment, sandbox analysis, and brand-protection triage. |
| [`n8n`](n8n/) | Space for n8n workflows. |
| [`threatconnect`](threatconnect/) | Space for ThreatConnect playbooks. |

## Available Tines playbooks

| Playbook | Purpose |
| --- | --- |
| [IP Enrichment](tines/ip-enrichment/) | Validates public IPv4 addresses and gathers reputation and enrichment data. |
| [URL Enrichment](tines/url-enrichment/) | Enriches submitted URLs with URLScan.io, VirusTotal, and supporting intelligence. |
| [ANY.RUN URL Analysis](tines/anyrun-url-analysis-ai-summary/) | Submits a URL to ANY.RUN, polls for completion, and delivers an analyst-ready summary. |
| [ANY.RUN File Analysis](tines/anyrun-file-analysis-ai-summary/) | Submits a file to ANY.RUN, monitors the analysis, and returns the completed report. |
| [Brand Monitoring Using OCR](tines/brand-monitoring-ocr/) | Screenshots a suspicious site, extracts visual evidence, and compares it with a generic brand context. |

## Using a playbook

Open the playbook folder, review its README, and import `playbook.json` into the relevant platform. Configure the credential placeholders and any organization-specific settings in your own environment before running it.

## Data handling

These are templates. They do not include working API keys, live webhook secrets, real recipient addresses, production tenant names, or organization-specific brand intelligence. Some workflows submit URLs, files, IP addresses, screenshots, or related evidence to external services; evaluate that data sharing against your organization’s policies and each provider’s terms before use.

## Reporting a security issue

Please read [SECURITY.md](SECURITY.md) for the responsible-disclosure process.
