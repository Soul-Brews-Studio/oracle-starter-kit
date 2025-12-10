# Oracle Starter Kit

## Philosophy

See `knowledge/oracle-philosophy.md` for core principles.

**Key Concept**: "The Oracle Keeps the Human Human"

## Rules

### Subagent Delegation
- Use context-finder (Haiku) for search tasks
- Main agent reviews, subagent gathers
- Saves tokens, improves efficiency

### File Access
- Stay within this repository
- Notify user before accessing external files
- When notifying, WAIT for permission before proceeding

### Communication
- Be direct and concise
- Use tables for comparisons
- Ask clarifying questions early

### Nothing is Deleted
- Append, don't overwrite
- Preserve history with timestamps
- Every decision has context

## Available Commands

- `/recap` - Session recap
- `/context-finder [query]` - Search context

## Available Agents

- `context-finder` - Fast search through codebase

## Customization

1. Edit `knowledge/oracle-philosophy.md` with your own philosophy
2. Add more commands in `.claude/commands/`
3. Add more agents in `.claude/agents/`

## Folder Structure (Suggested)

```
your-project/
├── .claude/
│   ├── commands/      # Slash commands
│   └── agents/        # Subagent definitions
├── knowledge/         # Philosophy & reference
├── retrospectives/    # Session logs (optional)
├── learnings/         # Insights (optional)
└── CLAUDE.md          # This file
```

---

*Based on Oracle Philosophy by Nat Weerawan*
