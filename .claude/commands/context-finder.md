# /context-finder - Search History & Context

Fast search through git history, retrospectives, issues, and codebase.

## Usage

```
/context-finder              # No args = recent context summary
/context-finder [query]      # Search for specific topic
```

## Behavior

### No Arguments (Default)
When called without arguments, automatically gather:
1. Recent commits (last 10)
2. Latest retrospectives (last 3)
3. Latest learnings (last 3)
4. Open issues or pending tasks

### With Arguments
Search across all sources for the specific query.

## Action

Use the Task tool with:
```
subagent_type: context-finder
model: haiku
prompt: [query or default summary request]
```

ARGUMENTS: $ARGUMENTS
