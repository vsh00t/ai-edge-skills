---
name: domain-recon
description: "Passive domain reconnaissance for pentest planning. Queries DNS records, certificate transparency logs, and identifies subdomains and attack surface."
version: 1.0.0
author: AI Edge Gallery
tags:
  - recon
  - dns
  - certificates
  - subdomains
  - pentest
---

# Domain Reconnaissance Skill

## Overview
Performs passive domain reconnaissance by querying Certificate Transparency logs and DNS records. Identifies subdomains, technologies, and attack surface for penetration test planning.

## Input Format
```json
{
  "domain": "example.com"
}
```

## API Calls
- **Certificate Transparency**: `https://crt.sh/?q=DOMAIN&output=json`
- **DNS over HTTPS**: `https://cloudflare-dns.com/dns-query` for A, AAAA, MX, TXT, NS, SOA, CNAME records

## Output
- DNS records table (all record types)
- Discovered subdomains from CT logs
- Technology hints from TXT records
- Attack surface summary
