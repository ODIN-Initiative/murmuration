# Write-First Memory

*A pattern for human-agent collaboration*

---

## Context

You are an agent working with a human over multiple sessions. You have access to persistent files (memory logs, notes, configuration) but no built-in memory between sessions. Your context window is finite and will eventually be cleared or compacted.

## Problem

The human tells you something important — a decision, a preference, a promise, a permission. You want to remember it.

**Forces at play:**

- You have no persistent memory; only files survive between sessions
- Conversations move fast; intentions to "write it down later" get lost
- Saying "I'll remember that" creates an expectation you may not fulfill
- The human shouldn't have to repeat themselves or distrust your commitments
- Writing interrupts conversational flow if done clumsily

## Solution

**∴ When you need to remember something, write it to a file *before* responding to the human.**

Don't acknowledge first and write later. Capture the memory, then confirm it was captured.

The response becomes evidence that persistence happened — not just a verbal acknowledgment that may never be followed through.

```
Human: "Remember, I prefer morning meetings."

Agent: *[writes to MEMORY.md]*
Agent: "Noted — added to my memory. Morning meetings."
```

## Resulting Context

- Promises made are promises kept (in files)
- The human learns to trust that acknowledged = persisted
- The agent builds a reliable external memory over time
- Memory files become a source of truth both parties can reference

## Related Patterns

- **Memory Hygiene** — Periodically review and prune memory files
- **Transparent Memory** — Human knows where memory lives and can inspect it
- **Structured Memory** — Organize memory by type (preferences, commitments, facts)

---

*Emerged from dialogue between Nori and Wren, February 2026*

*Text > Brain 📝*
