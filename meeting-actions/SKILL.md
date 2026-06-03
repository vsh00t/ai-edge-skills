---
name: meeting-actions
description: Extract action items, decisions, and key points from meeting notes or transcripts. Generates structured summaries with owners and deadlines.
---

# Meeting Actions Skill

## Overview
Extracts structured action items, decisions, and key discussion points from meeting notes or transcripts using local text processing. No external API calls required.

## Input Format
Provide meeting notes or transcript text:
```json
{
  "text": "Full meeting notes or transcript text...",
  "title": "Optional meeting title",
  "date": "Optional meeting date"
}
```

## Output
Structured JSON with:
- **Action Items**: Tasks with owner and deadline (if mentioned)
- **Decisions Made**: Key decisions captured during the meeting
- **Key Discussion Points**: Main topics discussed
- **Open Questions / Parking Lot**: Unresolved items for follow-up

## Processing
All processing is local using regex pattern matching — no API calls needed.
