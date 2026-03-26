---
title: "Firewise AI"
description: "GenAI-powered PAN-OS security posture validator — upload a firewall config, ask natural language questions, get AI-generated audit analysis."
tags: ["PAN-OS", "Palo Alto Networks", "GenAI", "Streamlit", "Security Audit"]
weight: 4
externalUrl: "https://github.com/BadAsh99/firewise-ai"
showDate: false
imagePosition: "left center"
imagePositionFeature: "left center"
---

Upload a PAN-OS XML firewall config. Ask natural language questions about your security posture. Get AI-generated analysis backed by real configuration context — without parsing thousands of lines of XML manually.

**Example questions:**
- "Are any security zones missing egress rules?"
- "Which policies allow any-to-any traffic?"
- "Does this config comply with CIS PAN-OS Benchmark recommendations?"
- "Is the management interface exposed to untrusted zones?"

**Why it exists:** Security engineers inherit undocumented firewall configs constantly. Firewise turns a multi-hour manual audit into a 10-minute AI-assisted review — with dual model support (Gemini + GPT-4) and a full CSV export for audit records.

**Stack:** Python · Streamlit · Google Gemini · OpenAI GPT-4 · xmltodict

**[View on GitHub →](https://github.com/BadAsh99/firewise-ai)**
