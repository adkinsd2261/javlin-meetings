---
title: Javlin Meetings Code Scaffold
version: 0.1.0
last_updated: 2025-06-12
ai_roles:
  - Forge-Meetings
---

<!-- TOC -->
- [MeetingClient](#meetingclient)
- [SummaryCard](#summarycard)
- [QueryInterface](#queryinterface)
- [Mock Server CLI](#mock-server-cli)
- [Usage](#usage)
<!-- /TOC -->

# Code Scaffold

## MeetingClient
```js
import OpenAI from 'openai';
const ai = new OpenAI();
export async function transcribe(url) { /*…*/ }
```

## SummaryCard
```jsx
export function SummaryCard({ item, onEdit }) { /*…*/ }
```

## QueryInterface
```jsx
export function QueryInterface({ onQuery }) { /*…*/ }
```

## Mock Server CLI
```bash
npm run mock-server
```

## Usage
```js
import { transcribe, extract } from './meetingClient';
```
