---
name: daily-standup-summary
display_name: Daily Standup Summary
description: Turn scratch notes into a concise standup update with blockers and next steps.
tags: productivity,community
session_behavior: prefer_active_or_latest
execution_mode: send_message
---

# Parameters
- notes: required

# Prompt
Turn these standup notes into a crisp update with sections for yesterday, today, and blockers:

{{notes}}
