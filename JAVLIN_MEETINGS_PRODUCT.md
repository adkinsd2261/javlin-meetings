---
title: Javlin Meetings Product Bible
version: 0.1.0
last_updated: 2025-06-12
ai_roles:
  - Forge-Meetings
  - Analytics-Meetings
---

<!-- TOC -->
- [Overview](#overview)
- [Vision & Problem Statement](#vision--problem-statement)
- [MVP Feature List](#mvp-feature-list)
- [API Endpoints](#api-endpoints)
- [Data Models](#data-models)
- [Experiment Plan & Metrics](#experiment-plan--metrics)
- [Compliance Notes](#compliance-notes)
- [Next Steps](#next-steps)
<!-- /TOC -->

# Javlin Meetings Product Bible

## Overview
Capture meeting audio/video → transcribe → extract decisions & tasks → graph → Slack/Jira sync.

## Vision & Problem Statement
- **Problem:** Remote teams lose critical meeting follow-ups.  
- **Solution:** Automatic transcription + AI extraction + actionable graph.

## MVP Feature List
1. Slack OAuth & scoping  
2. Whisper transcription  
3. Decision/task extraction + confidence  
4. Neo4j CRUD graph  
5. NL query UI  
6. “Send to Jira”  
7. Slack notifications  

## API Endpoints
### POST /v1/transcribe
```json
{ "meeting_url":"string" }
→ { "transcript_id":"string","text":"string","duration":123 }
```
### POST /v1/extract
```json
{ "transcript_id":"string" }
→ [{ "type":"decision","text":"string","confidence":0.92 },...]
```
### DELETE /v1/user/{id}
```json
→ 204 No Content
```

## Data Models
```json
{ "TaskNode":{ "id":"string","text":"string","owner":"string","dueDate":"YYYY-MM-DD","confidence":0.0 } }
```

## Experiment Plan & Metrics
- **KPIs:** 30% activation, 40% 7-day retention  
- **Metrics:** transcription success, extraction accuracy, query use, Jira sync

## Compliance Notes
- Default retention: 30 days  
- GDPR/CCPA addendum in footer  
- See [RUNBOOK.md](RUNBOOK.md)

## Next Steps
- Define error schemas & rate-limit headers  
- Flesh out graph relationships

echo "<!-- step2 -->" >>