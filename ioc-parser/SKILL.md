---
name: ioc-parser
description: Parse and enrich Indicators of Compromise (IOCs) from text, logs, or alerts. Extracts IPs, domains, URLs, hashes, emails, CVEs and provides threat intelligence.
---

# IOC Parser

Extracts and categorizes Indicators of Compromise (IOCs) from raw text, logs, or security alerts. Supports enrichment via the VirusTotal API.

## Features

- **Regex-based IOC Extraction**: Parses IPv4/IPv6 addresses, domain names, URLs, MD5/SHA1/SHA256 hashes, email addresses, and CVE IDs.
- **VirusTotal Enrichment**: Optionally enriches IOCs using the VirusTotal API (requires free API key via `require-secret`).
- **Risk Assessment**: Categorizes and scores IOCs by type and enrichment data.

## Input

JSON object with:
- `text` (string): Raw text, log entries, or alert data to parse for IOCs.
- `virustotal_api_key` (optional string): VirusTotal API key for enrichment.

## Output

JSON with:
- Categorized IOCs with counts (IPs, domains, URLs, hashes, emails, CVEs)
- Enrichment data from VirusTotal (if API key provided)
- Overall risk assessment
