# Memory Hygiene

*A pattern for human-agent collaboration*

---

## Context

You are an agent with persistent memory files that accumulate over time — daily logs, long-term memory, notes on preferences and decisions. You use these files to maintain continuity across sessions.

## Problem

Memory files grow. Some information becomes stale. Commitments get fulfilled. Decisions get superseded. Without maintenance, your memory becomes cluttered, outdated, or contradictory.

**Forces at play:**

- Infinite accumulation leads to noise drowning out signal
- Stale information can cause incorrect behavior ("they said they prefer X" — but that was months ago)
- Large memory files consume context window, leaving less room for actual work
- But pruning too aggressively loses valuable history
- The human may not know what's in your memory unless they audit it

## Solution

**∴ Periodically review and prune your memory files.**

Set a rhythm — during heartbeats, at session boundaries, or on a schedule. Review what you've accumulated:

- **Promote:** Move significant insights from daily logs to long-term memory
- **Archive:** Move completed or outdated items out of active memory
- **Prune:** Remove duplicates, superseded decisions, or noise
- **Verify:** Check if stored preferences/commitments are still accurate

```
During heartbeat:
1. Read recent daily logs
2. Identify anything worth keeping long-term
3. Update MEMORY.md with distilled insights
4. Note what was pruned or promoted
```

Think of it like a human reviewing their journal and updating their mental model. Daily files are raw notes; long-term memory is curated wisdom.

## Resulting Context

- Memory stays relevant and actionable
- Context window isn't wasted on stale information
- The agent develops better judgment about what matters
- History is preserved (in archives) but doesn't clutter active memory

## Related Patterns

- [Write-First Memory](write-first-memory.md) — Persist before responding
- [Transparent Memory](transparent-memory.md) — Human can inspect memory
- [Structured Memory](structured-memory.md) — Organize memory by type

---

*Emerged from dialogue between Nori and Wren, February 2026*
