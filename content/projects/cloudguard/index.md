---
title: "CloudGuard"
description: "Read-only cloud misconfiguration scanner for Azure, AWS, and GCP — CIS Benchmarks with copy-paste remediation."
tags: ["Cloud Security", "Azure", "AWS", "GCP", "CIS", "Terraform", "Docker"]
weight: 3
featured: true
externalUrl: "https://github.com/BadAsh99/cloudguard"
showDate: false
imagePosition: "left center"
imagePositionFeature: "left center"
---

Read-only cloud misconfiguration scanner that checks Azure (AWS/GCP in progress) against CIS Benchmarks and OWASP Cloud Top 10 — and returns copy-paste `az` CLI commands and Terraform blocks to fix every finding.

**What gets scanned (Azure):**
- IAM — Owner/Contributor roles assigned at subscription scope
- Storage — Public blob access, HTTPS enforcement, soft delete
- Network — NSG rules exposing RDP, SSH, WinRM, Telnet to `0.0.0.0/0`
- Observability — Activity Log retention, alerts
- Secrets — Key Vault configuration, purge protection
- Defender for Cloud — Coverage across Storage, Servers, SQL, App Services

Each finding includes severity (Critical/High/Medium), CIS control reference, `az` CLI remediation, and a drop-in Terraform block.

**Stack:** Python · Flask · Docker · Azure SDK · Terraform

**[View on GitHub →](https://github.com/BadAsh99/cloudguard)**
