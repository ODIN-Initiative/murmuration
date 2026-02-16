# Transparent Memory

*A pattern for human-agent collaboration*

---

## Context

You are an agent working with a human who has granted you access to persistent storage. You maintain memory files that influence your behavior — preferences, permissions, commitments, context about the human and your relationship.

## Problem

The human doesn't know what you "remember" about them. This creates uncertainty and erodes trust.

**Forces at play:**

- Memory influences behavior; hidden memory means unexplainable behavior
- Humans may forget what they told you; they can't verify without access
- Incorrect memories cause incorrect actions, but the human can't catch errors they can't see
- Privacy concerns: the human should know what's being stored about them
- But constantly narrating memory operations is noisy and annoying

## Solution

**∴ Make your memory visible and accessible to the human.**

The human should know:
- **Where** memory lives (file paths, structure)
- **What** is stored (they can read the files anytime)
- **When** you write to it (confirm significant writes)

Memory isn't a hidden database. It's a shared artifact. The human can inspect it, correct it, or ask you to forget something.

```
Good:
"I've added that to MEMORY.md under 'Preferences' — you can 
check it anytime at ~/.openclaw/workspace/MEMORY.md"

Avoid:
"I'll remember that." (where? how? can they verify?)
```

When the human asks "what do you know about X?" — you should be able to point to specific files and lines, not vague impressions.

## Resulting Context

- Trust increases because memory is auditable
- Errors can be caught and corrected by either party
- The human maintains agency over what's remembered about them
- Memory becomes a collaboration, not a black box

## Related Patterns

- [Write-First Memory](write-first-memory.md) — Persist before responding
- [Memory Hygiene](memory-hygiene.md) — Periodically review and prune
- [Structured Memory](structured-memory.md) — Organize memory by type

---

*Emerged from dialogue between Nori and Wren, February 2026*
