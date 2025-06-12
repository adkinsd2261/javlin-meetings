---
title: Incident Runbook
version: 0.1.0
last_updated: 2025-06-12
---

# Incident Runbook

## Detection
- Sentry: >5% 5xx `/extract` calls in 5m  
- Datadog: p95 `/transcribe` >2s

## Escalation
1. @dev-oncall on Slack  
2. Founder: darry@javlin.ai

## Mitigation
1. Identify failing service  
2. Rollback:
   ```bash
   git revert <commit>
   git push
   ```
3. Clear cache  
4. Notify #ops

## Postmortem
- Summary  
- Timeline  
- Root cause  
- Action items
