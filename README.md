---
title: Javlin Meetings README
version: 0.1.0
last_updated: 2025-06-12
ai_roles:
  - Forge-Meetings
  - Marketing-Meetings
  - Analytics-Meetings
---

<!-- TOC -->
- [Overview](#overview)
- [Quick Start](#quick-start)
- [Documentation](#documentation)
- [Action Items](#action-items)
<!-- /TOC -->

# Javlin Meetings

## Overview
Turn every call into a living project brain.  
Javlin Meetings transcribes your meetings, extracts decisions & tasks, and links them in a queryable knowledge graph with Slack & Jira integration.

## Quick Start
1. **Clone the repo**  
   ```bash
   git clone git@github.com:your-org/javlin-meetings.git
   cd javlin-meetings
   ```
2. **Install dependencies**  
   ```bash
   npm install
   ```
3. **Configure environment**  
   ```bash
   cp .env.example .env
   # fill in SLACK_CLIENT_ID, SLACK_CLIENT_SECRET, OPENAI_API_KEY, NEO4J_URI, etc.
   ```
4. **Run mock server**  
   ```bash
   npm run mock-server
   ```
5. **Start the app**  
   ```bash
   npm run dev
   ```

## Documentation
- [CHANGELOG.md](CHANGELOG.md)  
- [JAVLIN_MEETINGS_BRAND.md](JAVLIN_MEETINGS_BRAND.md)  
- [JAVLIN_MEETINGS_PRODUCT.md](JAVLIN_MEETINGS_PRODUCT.md)  
- [JAVLIN_MEETINGS_UI_SPEC.md](JAVLIN_MEETINGS_UI_SPEC.md)  
- [JAVLIN_MEETINGS_TASKS.md](JAVLIN_MEETINGS_TASKS.md)  
- [JAVLIN_MEETINGS_ASSETS.md](JAVLIN_MEETINGS_ASSETS.md)  
- [JAVLIN_MEETINGS_IMPLEMENTATION.md](JAVLIN_MEETINGS_IMPLEMENTATION.md)  
- [JAVLIN_MEETINGS_PREP.md](JAVLIN_MEETINGS_PREP.md)  
- [JAVLIN_MEETINGS_SCAFFOLD.md](JAVLIN_MEETINGS_SCAFFOLD.md)  
- [LEGAL_PRELAUNCH_CHECKLIST.md](LEGAL_PRELAUNCH_CHECKLIST.md)  
- [JAVLIN_MEETINGS_CONTENT.md](JAVLIN_MEETINGS_CONTENT.md)  
- [RUNBOOK.md](RUNBOOK.md)

## Action Items
- [ ] Verify environment variables and CI secrets.  
- [ ] Reserve DNS/subdomain if needed.  
- [ ] Populate all docs with content.  