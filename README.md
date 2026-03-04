### ui-reviewer

A senior UX/UI designer agent that reviews any website's UI and UX. It takes screenshots on desktop and mobile, then delivers a full analysis covering layout, navigation, accessibility, conversion, and more.

## Installation

Agents live in `~/.claude/agents/`. Copy any agent file there and it's instantly available in all your Claude Code sessions.

**Install all agents:**

```bash
curl -o ~/.claude/agents/ui-reviewer.md \
  https://raw.githubusercontent.com/deekshashekar/claude-agents/main/ui-reviewer.md
```

**Or clone and symlink:**

```bash
git clone https://github.com/deekshashekar/claude-agents.git
ln -s $(pwd)/claude-agents/ui-reviewer.md ~/.claude/agents/ui-reviewer.md
```

## Usage

Once installed, open any Claude Code session and ask:

```
Review https://yourwebsite.com
```

The agent will automatically:

1. Take full-page desktop screenshots of each section
2. Resize to 375x812 (iPhone) and repeat
3. Analyze narrative, layout, IA, navigation, social proof, accessibility, and mobile responsiveness
4. Deliver a prioritized list of recommendations and quick wins

## Requirements

- [Claude Code](https://claude.ai/code) installed
- Playwright MCP server configured (for browser automation)
