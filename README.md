# Security Automation Playbooks

Public, reusable security automation playbooks organized by platform.

## Layout

- `tines/` — Tines Stories playbooks
- `n8n/` — n8n workflows
- `threatconnect/` — ThreatConnect playbooks

Each playbook belongs in its own directory and should contain:

- `playbook.json` — importable workflow definition
- `workflow.png` — workflow diagram or screenshot
- `README.md` — purpose, inputs, requirements, and setup notes

## Before publishing a playbook

Do not commit API keys, webhook secrets, private URLs, personal email addresses, tenant identifiers, or production data. Use credential placeholders and generic example values instead.
