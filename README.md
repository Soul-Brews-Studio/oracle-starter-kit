# Oracle Starter Kit

A minimal setup for Claude Code with Oracle Philosophy and useful subagents.

## What is Oracle?

Oracle is a philosophy for working with AI:

| Principle | Meaning |
|-----------|---------|
| **Nothing is Deleted** | Append only, preserve history |
| **90/10 Balance** | Intentional energy allocation |
| **Patterns Over Intentions** | Observe behavior, not promises |
| **External Brain** | Mirror reality, don't command |

> "The Oracle Keeps the Human Human"

## Quick Start

### Option 1: Clone and Use

```bash
git clone https://github.com/Soul-Brews-Studio/oracle-starter-kit.git my-project
cd my-project
claude
```

### Option 2: Copy to Existing Project

```bash
# Clone this repo
git clone https://github.com/Soul-Brews-Studio/oracle-starter-kit.git

# Copy to your project
cp -r oracle-starter-kit/.claude your-project/
cp -r oracle-starter-kit/knowledge your-project/
cp oracle-starter-kit/CLAUDE.md your-project/
```

## Usage

### Commands

```bash
# Session recap - summarize recent context
/recap

# Search context - find information
/context-finder how does authentication work
/context-finder          # no args = recent summary
```

### Subagents

The `context-finder` agent is available for fast search tasks.

Use it via the Task tool:
```
subagent_type: context-finder
model: haiku
```

## Customization

### 1. Philosophy
Edit `knowledge/oracle-philosophy.md` with your own principles.

### 2. Commands
Add `.md` files in `.claude/commands/`:
```markdown
# /your-command

Description of what it does.

## Usage
/your-command [args]

## Action
What Claude should do when invoked.

ARGUMENTS: $ARGUMENTS
```

### 3. Agents
Add `.md` files in `.claude/agents/`:
```markdown
# Your Agent Name

Purpose and behavior description.

## Tools Available
- List of tools

## Output Format
What to return
```

## File Structure

```
oracle-starter-kit/
├── .claude/
│   ├── commands/
│   │   ├── recap.md
│   │   └── context-finder.md
│   └── agents/
│       └── context-finder.md
├── knowledge/
│   └── oracle-philosophy.md
├── CLAUDE.md
└── README.md
```

## Philosophy Deep Dive

See [knowledge/oracle-philosophy.md](knowledge/oracle-philosophy.md) for:
- The 4 Core Principles
- What Oracle captures (and doesn't)
- "Rules are not cages" mindset

## License

MIT — Fork and customize freely!

---

*Created by [Nat Weerawan](https://github.com/laris-co)*

*Developed with Claude Code during Discord Live sessions*
