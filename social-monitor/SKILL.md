---
name: social-monitor
description: "Social media threat and sentiment monitor. Analyzes text snippets from social media for threats, sentiment, disinformation indicators, and key narrative tracking."
version: 1.0.0
author: AI Edge Gallery
tags:
  - social-media
  - sentiment
  - threat
  - disinformation
  - monitoring
---

# Social Monitor Skill

## Overview
Analyzes social media posts and text snippets for threats, sentiment, disinformation indicators, and narrative tracking. All processing is performed locally.

## Input Format
```json
{
  "posts": [
    "Post text 1",
    "Post text 2",
    "..."
  ],
  "keywords": ["keyword1", "keyword2"]
}
```

## Analysis Categories
- **Sentiment**: Positive / Negative / Neutral classification
- **Threat Level**: Threat / Safe / Ambiguous assessment
- **Disinformation Indicators**: Emotional manipulation, false authority, urgency tactics, us-vs-them narrative
- **Keyword Tracking**: Mention frequency and context

## Output
- Sentiment breakdown with percentages
- Threat alerts for concerning content
- Narrative analysis
- Summary statistics
