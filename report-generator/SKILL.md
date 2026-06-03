name	report-generator
description	Generate professional cybersecurity pentest and audit reports. Structures findings with severity ratings, observations, and recommendations in HTML format.
# Report Generator Skill

## Overview
Generates professional cybersecurity penetration test and audit reports from raw findings data. Produces HTML-formatted reports with severity color coding, executive summaries, and detailed findings.

## Input Format
Provide raw findings as JSON with the following structure:
```json
{
  "findings": [
    {
      "title": "Finding title",
      "description": "Detailed description",
      "severity": "Critical|High|Medium|Low|Info",
      "component": "Affected component/system",
      "observation": "What was observed",
      "recommendation": "Remediation recommendation"
    }
  ],
  "metadata": {
    "project": "Project name",
    "client": "Client name",
    "date": "Assessment date",
    "assessor": "Assessor name"
  }
}
```

## Output
- Professional HTML report with color-coded severity ratings
- Executive summary table with finding counts
- Detailed findings with observations and recommendations
- Risk rating matrix

## Severity Colors
- Critical: Red (#dc3545)
- High: Orange (#fd7e14)
- Medium: Yellow (#ffc107)
- Low: Blue (#0d6efd)
- Info: Gray (#6c757d)