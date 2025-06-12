---
title: Javlin Meetings Pre-Flight Checklist
version: 0.1.0
last_updated: 2025-06-12
ai_roles:
  - Forge-Meetings
---

<!-- TOC -->
- [Fresh Clone](#fresh-clone)
- [Smoke Tests](#smoke-tests)
- [Secrets & DNS](#secrets--dns)
- [Assets](#assets)
- [Next Steps](#next-steps)
<!-- /TOC -->

# Pre-Flight Checklist

## Fresh Clone
- [ ] git clone & npm install  
- [ ] .env.example docs correct

## Smoke Tests
- [ ] npm run mock-server → 200  
- [ ] npm run dev no JS errors

## Secrets & DNS
- [ ] SLACK_*, OPENAI_* in CI  
- [ ] meetings.javlin.ai DNS & SSL

## Assets
- [ ] logos in assets/logo/  
- [ ] palette in assets/design/  
- [ ] policies in assets/policies/

## Next Steps
- [ ] Schedule sprint reminders  
- [ ] Finalize pilot team list
