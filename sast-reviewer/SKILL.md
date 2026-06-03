name	sast-reviewer
description	Static Application Security Testing (SAST) code reviewer. Analyzes code snippets for security vulnerabilities following OWASP Top 10. Supports Java/Spring, Python, JavaScript.
# SAST Code Reviewer

Static Application Security Testing tool that analyzes code snippets for security vulnerabilities aligned with the OWASP Top 10. Supports Java/Spring, Python, and JavaScript.

## Features

- **OWASP Top 10 Coverage**: Detects SQL Injection, XSS, Deserialization, Hardcoded credentials, Path traversal, Command injection, SSRF, Insecure crypto, XXE, and Security misconfiguration.
- **Multi-language Support**: Language-specific detection rules for Java/Spring, Python, and JavaScript.
- **Detailed Findings**: Each finding includes severity, line number, OWASP category, description, and remediation advice.
- **Summary Report**: Aggregated counts by severity level.

## Input

JSON object with:
- `code` (string): Source code snippet to analyze.
- `language` (string): Programming language — "java", "python", or "javascript".

## Output

JSON with:
- List of findings (each with severity, line, category, description, remediation)
- Summary count by severity (Critical, High, Medium, Low)
- Overall risk assessment