# /context-finder - Search History & Context

Fast search through git history, retrospectives, issues, and codebase using the context-finder subagent.

## Usage

```
/context-finder              # No args = recent context summary
/context-finder [query]      # Search for specific topic
```

## Behavior

### No Arguments (Default)
When called without arguments, automatically gather:
1. **Recent context issues** - `gh issue list` filtered by "context:" prefix
2. **Latest retrospectives** - Most recent 3 files in `retrospectives/`
3. **Latest learnings** - Most recent 3 files in `learnings/`
4. **Recent commits** - Last 10 commits with timestamps

### With Arguments
Search across all sources for the specific query.

## Examples

```
/context-finder                        # Recent context summary
/context-finder voice notification     # Search specific topic
/context-finder workshop requests      # Find workshop context
```

## Action

Use the Task tool with:
```
subagent_type: context-finder
model: haiku
prompt: [query or default summary request]
```

ARGUMENTS: $ARGUMENTS
