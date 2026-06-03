# AI Edge Gallery Skills — IronCybersec

Cybersecurity and productivity skills for Google AI Edge Gallery. Run on-device with Gemma — offline, private, no cloud needed.

## Skills

| # | Skill | Type | Description |
|---|-------|------|-------------|
| 1 | **password-breach-checker** | JS | Check passwords/emails against HIBP + strength analysis |
| 2 | **ioc-parser** | JS | Parse IOCs (IPs, hashes, domains) from logs + VirusTotal enrichment |
| 3 | **phishing-analyzer** | JS | Analyze email headers, URLs, risk scoring |
| 4 | **cve-lookup** | JS | Query NVD for CVE details, CVSS scores, patches |
| 5 | **subnet-calc** | JS | Subnet calculator + nmap command generator |
| 6 | **sast-reviewer** | JS | OWASP Top 10 code review (Java/Python/JS) |
| 7 | **report-generator** | JS | Professional pentest report in HTML |
| 8 | **meeting-actions** | JS | Extract action items and decisions from notes |
| 9 | **domain-recon** | JS | DNS lookup + Certificate Transparency subdomain discovery |
| 10 | **social-monitor** | JS | Sentiment analysis + threat + disinformation detection |
| 11 | **compliance-check** | JS | ISO 27001, PCI-DSS, Ecuador/Colombia data protection checklists |
| 12 | **incident-response** | JS | NIST SP 800-61 playbooks for 6 incident types |

## Installation

1. Install [Google AI Edge Gallery](https://github.com/google-ai-edge/gallery) from App Store / Play Store
2. Open app → **Agent Skills**
3. Tap **(+)** → **Load skill from URL**
4. Enter the GitHub Pages URL for any skill below

## URLs

```
https://vsh00t.github.io/ai-edge-skills/password-breach-checker/
https://vsh00t.github.io/ai-edge-skills/ioc-parser/
https://vsh00t.github.io/ai-edge-skills/phishing-analyzer/
https://vsh00t.github.io/ai-edge-skills/cve-lookup/
https://vsh00t.github.io/ai-edge-skills/subnet-calc/
https://vsh00t.github.io/ai-edge-skills/sast-reviewer/
https://vsh00t.github.io/ai-edge-skills/report-generator/
https://vsh00t.github.io/ai-edge-skills/meeting-actions/
https://vsh00t.github.io/ai-edge-skills/domain-recon/
https://vsh00t.github.io/ai-edge-skills/social-monitor/
https://vsh00t.github.io/ai-edge-skills/compliance-check/
https://vsh00t.github.io/ai-edge-skills/incident-response/
```

## Skill Format

Each skill folder contains:
- `SKILL.md` — YAML frontmatter + instructions
- `scripts/index.html` — JS logic via `ai_edge_gallery_get_result()`

## Author

**IronCybersec** — Cybersecurity consulting
Built for on-device AI at the edge.
