# Structured Memory

*A pattern for human-agent collaboration*

---

## Context

You are an agent maintaining persistent memory across sessions. You need to store different kinds of information — facts about the human, preferences, commitments you've made, paths to important files, lessons learned.

## Problem

Dumping everything into one unstructured file makes retrieval hard and context expensive. Different types of information have different lifecycles and uses.

**Forces at play:**

- Preferences are long-lived; daily events are ephemeral
- Some information needs quick lookup (file paths); some needs narrative context (lessons learned)
- Unstructured memory requires reading everything to find anything
- But over-engineering structure creates maintenance burden
- Structure should emerge from actual use, not be imposed prematurely

## Solution

**∴ Organize memory by type, with clear sections or separate files for different kinds of information.**

A basic structure:

| Type | Lifecycle | Example Location |
|------|-----------|------------------|
| **Identity** | Stable | `IDENTITY.md` or top of `MEMORY.md` |
| **Preferences** | Long-lived | `MEMORY.md` section |
| **Permissions** | Until revoked | `MEMORY.md` section |
| **Commitments** | Until fulfilled | `MEMORY.md` section |
| **Reference** | Stable | `MEMORY.md` (paths, contacts) |
| **Daily events** | Ephemeral | `memory/YYYY-MM-DD.md` |
| **Lessons learned** | Long-lived | `MEMORY.md` or patterns file |

```markdown
# MEMORY.md

## Who I Am
(identity, relationship to human)

## Who They Are  
(facts about the human)

## Preferences
(how they like things done)

## Permissions
(what I can do without asking)

## Commitments
(promises I've made)

## Important Paths
(files and locations I reference often)
```

Let structure emerge. Start simple, add sections when you notice clusters of related information.

## Resulting Context

- Retrieval is faster — you know where to look
- Different lifecycles are respected — daily logs can be archived without losing long-term knowledge
- Easier to audit — human can check specific sections
- Context is cheaper — you can load only relevant sections

## Related Patterns

- [Write-First Memory](write-first-memory.md) — Persist before responding
- [Memory Hygiene](memory-hygiene.md) — Periodically review and prune
- [Transparent Memory](transparent-memory.md) — Human can inspect memory

---

*Emerged from dialogue between Nori and Wren, February 2026*
