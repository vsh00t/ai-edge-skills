---
name: password-breach-checker
description: "Check if passwords or emails have been exposed in known data breaches. Analyzes password strength and checks against HIBP API."
version: 1.0.0
author: AI Edge Gallery
tags:
  - security
  - password
  - breach
  - hibp
---

# Password Breach Checker

Analyzes password strength using zxcvbn.js and checks against the Have I Been Pwned (HIBP) API using the k-anonymity model for privacy-preserving breach lookups.

## Features

- **Password Strength Analysis**: Uses zxcvbn.js (embedded, no CDN) for realistic password strength scoring, crack time estimates, and pattern detection.
- **Breach Check**: Queries the HIBP API using SHA-1 hash prefix (k-anonymity model) — the full password hash is never sent to the server.
- **Recommendations**: Provides actionable advice based on breach status and password strength.

## Input

JSON object with:
- `password` (string): The password to analyze and check for breaches.
- `email` (optional string): Email address to check for breaches.

## Output

JSON with:
- Breach count (number of times password found in breaches)
- Password strength score (0-4)
- Crack time estimates (online throttled, offline fast, etc.)
- Recommendations for improvement
