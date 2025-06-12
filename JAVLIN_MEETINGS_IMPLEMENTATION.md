---
title: Javlin Meetings Implementation Guide
version: 0.1.0
last_updated: 2025-06-12
ai_roles:
  - Forge-Meetings
---

<!-- TOC -->
- [Overview](#overview)
- [Env Setup](#env-setup)
- [Deps](#deps)
- [CI/CD](#cicd)
- [Storybook & Lint](#storybook--lint)
- [Mock Server](#mock-server)
- [Next Steps](#next-steps)
<!-- /TOC -->

# Implementation Guide

## Overview
Dev setup, dependencies, CI/CD for Javlin Meetings.

## Env Setup
1. Copy `.env.example` → `.env`  
2. Fill SLACK_*, OPENAI_API_KEY, NEO4J_URI

## Deps
- @slack/bolt  
- openai  
- neo4j-driver  
- react, vite, tailwindcss

## CI/CD
```yaml
# .github/workflows/ci.yml
on: [push,pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3 with: node-version: '18'
      - run: npm install
      - run: npm run lint
      - run: npm test
```

## Storybook & Lint
```js
// .storybook/main.js
stories: ['../src/**/*.stories.jsx']
```

## Mock Server
```bash
npm run mock-server
```

## Next Steps
- Add deploy pipeline to Vercel/AWS  
- Add preview environments
