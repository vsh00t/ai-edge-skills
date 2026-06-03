---
name: phishing-analyzer
description: Analyze suspicious emails for phishing indicators. Parses email headers, extracts URLs, checks sender reputation, and provides a risk score.
---

# Phishing Analyzer

Analyzes suspicious emails for phishing indicators by parsing headers, extracting and examining URLs, checking for social engineering techniques, and computing a risk score.

## Features

- **Header Parsing**: Extracts and analyzes Received, From, Reply-To, Message-ID, SPF/DKIM/DMARC authentication results.
- **URL Analysis**: Detects suspicious TLDs, IP-based URLs, URL shorteners, and potential homograph attacks.
- **Content Analysis**: Checks for urgency language, generic greetings, mismatched From/Reply-To addresses.
- **Base64 Decoder**: Decodes Base64-encoded email body content.
- **Risk Scoring**: Computes a 0-100 risk score with breakdown by category.

## Input

JSON object with:
- `email_raw` (string): Raw email content including headers and body.
- Or `headers` (object) + `body` (string): Pre-parsed headers and body.

## Output

JSON with:
- Risk score (0-100) with category breakdown
- Header analysis (authentication results, sender analysis)
- URL analysis findings
- Content analysis findings
- Recommendations
