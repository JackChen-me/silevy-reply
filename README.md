# silevy-reply

A Claude Code skill for drafting cross-platform replies and comments. Auto-routes to platform-specific rules for GitHub, Reddit, Twitter/X, Hacker News, and more.

## What it does

When you need to reply to an issue, PR, Reddit comment, tweet, or any online discussion, this skill:

1. **Routes** to the right platform ruleset based on your input
2. **Analyzes** context (your turf vs. someone else's, cold DM, etc.)
3. **Drafts** a reply that sounds human, not AI
4. **Checks** before sending: intent, facts, tone, style

## Platform support

| Platform | Trigger |
|----------|---------|
| GitHub Issues/PRs | Paste issue/PR number or link |
| Reddit | Paste comment text or screenshot |
| Twitter/X | Paste tweet content |
| HN / Discord / Forums | Auto-applies general principles |

## Key principles

- **High information density.** No filler sentences.
- **Have an opinion.** Don't just describe.
- **Lead with the conclusion.** No preamble.
- **Short.** 2-5 sentences unless deep technical discussion.
- **Sound human.** Contractions, casual tone, no AI-speak.

## Anti-AI-smell checklist

The skill maintains a detailed blocklist of phrases and patterns that scream "AI-generated", including:

- Em dashes in body text
- "Great question" / "Great catch"
- "Feel free to..." / "Happy to discuss further"
- Thank > Answer > Invite three-part structure
- Addressing every single point in a reply

## Installation

Two versions available:

- `skill.md` -- English
- `skill-zh.md` -- Chinese (中文版)

```bash
# macOS / Linux
mkdir -p ~/.claude/skills/silevy-reply

# English version
cp skill.md ~/.claude/skills/silevy-reply/skill.md

# Or Chinese version (中文版)
cp skill-zh.md ~/.claude/skills/silevy-reply/skill.md
```

Then use it in Claude Code by typing `/silevy-reply` followed by the content you want to reply to.

## Examples

**GitHub issue reply:**
```
/silevy-reply #72
```

**Reddit comment analysis:**
```
/silevy-reply [paste reddit comments]
```

**Draft a tweet reply:**
```
/silevy-reply [paste tweet]
```

## License

MIT
