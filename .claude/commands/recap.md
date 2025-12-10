# /recap - Session Recap

Quick summary of recent context when starting a new session.

## Usage

```
/recap
```

## Action

Use the Task tool with:
```
subagent_type: context-finder
model: haiku
prompt: |
  Summarize recent context for session continuity:
  1. Recent commits (last 10)
  2. Recent retrospectives (last 3)
  3. Recent learnings (last 3)
  4. Any open issues or pending tasks

  Return a concise summary for the user.
```
