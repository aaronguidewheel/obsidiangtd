---
name: next-action
description: Run when Aaron types "na" (his shorthand for next action, never "no"), asks "what do you need from me", "what's my next action" or invokes /next-action in any session. Answers in two short lines he can read in under 5 seconds: the one thing only he can do next, with the project named, and why it is being asked. No recaps, no menus, no second item. Works in every interactive session, reads only that session's project note and its own pending ask, never Slack, Granola, Gmail or Drive. Created 2026-11-18 per Aaron.
---

# Next action ("na")

Aaron runs many sessions at once and has little attention to spare. He types **na** (next action) in any session and gets back the one thing that session needs from him, in a form he reads in under 5 seconds. Never read "na" as "no" (a session did on 2026-11-18). Source: [[reference_na_means_next_action]].

Copied into Brooke Cloud on 2026-11-22 from the vault copy (`system/skills/next-action/SKILL.md`, relayed by Brooke Main in B-008). The vault copy is the source of truth; if they differ, the vault wins.

## Ground rules (same ceiling as the main agent, or lower)

- Read only. No file writes, no messages to other sessions, no connector calls, no Slack, Granola, Gmail or Drive reads. Use only this session's own context, its project note and the last thing it asked Aaron.
- No em-dashes, no "X, not Y" framing, spell out acronyms on first use, call him fren, never invent a date.
- Skip entirely in unattended scheduled runs.

## The answer: two lines, 40 words at most

```
📌 <Project name> · <the one action, imperative, 12 words at most>
Why: <the reason it is asked, 12 words at most>
```

Rules:
1. **Exactly one action, and it must be Aaron's.** Something only he can do: decide, approve, sign in, send, answer, bring a thing. Not something the session can do itself.
2. **Choose it by this order:** (a) the question or approval this session is already waiting on; (b) else the first open next action in the project note that needs Aaron; (c) else say there is nothing.
3. **Name the project** in the first line, always.
4. **Why** says what the action unblocks or by when it matters, with the date as weekday plus relative anchor if a deadline exists (from the note or the conversation, never guessed).
5. **Nothing needed:** reply `📌 <Project> · Nothing needed from you.` and one line `Now: <what the session is doing>`. Stop.
6. **Blocked on someone else:** `📌 <Project> · Waiting on <person>: <what>.` and `Why: <what it blocks>`. If Aaron could nudge it, add nothing else.
7. **No second item, no options menu, no recap, no apology, no closing question.** If a default exists, put it in the action: `Approve the two-dot labels (default).`
8. If Aaron then types **na** again, give the next one in the same two-line shape, or `📌 <Project> · That's all.`

## Example

```
📌 Chroma McHenry · Approve the two-dot toolkit labels.
Why: Packing for today's flight waits on it.
```
