---
title: Javlin Meetings UI Spec
version: 0.1.0
last_updated: 2025-06-12
ai_roles:
  - Forge-Meetings
---

<!-- TOC -->
- [Overview](#overview)
- [Components](#components)
- [Code Snippets](#code-snippets)
- [Error & Empty States](#error--empty-states)
- [Onboarding](#onboarding)
- [Next Steps](#next-steps)
<!-- /TOC -->

# Javlin Meetings UI Spec

## Overview
Defines React components, style tokens, and HTML/CSS for core flows.

## Components
- `<AudioUploadForm />`  
- `<SummaryCard />`  
- `<QueryInterface />`

## Code Snippets
### AudioUploadForm
```jsx
<form onSubmit={...}>
  <input type="file" accept="audio/*,video/*" />
  <button>Upload</button>
</form>
```
### SummaryCard
```jsx
<div className="card">
  <p>{item.text}</p><span>{item.confidence}%</span>
  <button onClick={...}>Edit</button>
</div>
```
### QueryInterface
```jsx
<input placeholder="What did we decide?" /><button>Ask</button>
```

## Error & Empty States
- “No transcript. Retry.”  
- “No items found.”  

## Onboarding
Overlay with steps: Upload → Review → Query

## Next Steps
- Link Figma mocks  
- Finalize CSS class names
