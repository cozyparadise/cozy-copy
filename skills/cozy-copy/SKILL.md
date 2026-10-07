---
name: cozy-copy
description: >-
  Write or review UX copy at an 8th-grade reading level. Covers buttons and calls to action,
  error messages, empty states, confirmations, tooltips, onboarding, consent and permission
  prompts, loading and success states, and copy for AI features. Use on "write copy for",
  "what should this button say", "review this error message", "fix this empty state",
  "word this dialog", or when naming a control, filling a blank state, or writing
  first-run text. One screen or one element at a time. Not for case studies, articles, or
  other long-form writing.
version: 0.1.0
user-invocable: true
argument-hint: "<screen, element, or copy to review>"
---

# cozy-copy

Copy for interfaces. It passes when a person reads it once, knows what happened, and knows
what to do next.

## Before you write

Ask for what's missing. Don't guess.

- **Where.** Which screen, flow, or element?
- **Who and when.** What is the person trying to do? How do they feel right now?
- **Tone.** Plain, warm, playful, calm?
- **Limits.** Character counts, platform rules, legal review?

Then read what's already on the screen. Find the labels, headings, and buttons around the
spot. Use the same words for the same things. If the app says "Delete" everywhere, don't
write "Remove" here.

## House rules

1. **8th-grade reading level.** Short sentences. Common words. Active voice. One idea per
   sentence. If a word needs explaining, pick a different word.
2. **Fewest words that still say it.** Cut filler like "just", "simply", "please note", and
   "in order to". Cut any word that doesn't help the person act.
3. **No colons in sentences.** Split into two sentences instead.
4. **Say what it does, not how it works.** "See the main points in seconds" beats "AI-powered
   summarization". Name the technology only when the law or the person's trust needs it.
5. **Hedge only when the system really doesn't know.** "This page may be restricted" is
   honest if the app can't tell. "This may take a moment" is filler if it's always quick.
6. **Never blame the person.** Name the cause, and put it where it really is.
7. **Never invent facts.** No made-up numbers, prices, limits, or legal claims. Ask.

## Patterns

### Buttons and calls to action
- Start with a verb and name the thing. "Save changes", "Create account", not "Submit".
- The label says what happens. If the button sends, it says "Send".
- A pair of buttons names both actions. "Delete files" and "Keep files", not "OK" and "Cancel".

### Error messages
- What happened, why if you know, and one way out.
- One way out, not three. "Try again" or "Close", whichever works.
- Name the real cause so people don't blame themselves or the app.

### Empty states
- What goes here, why it's empty, and how to start.
- The first action is a button, not a sentence telling them to find one.

### Confirmations
- Name the action and the count. "Delete 3 files?" not "Are you sure?"
- Give the consequence in one line. "You can't undo this."
- If you can offer undo instead, do. Undo beats a confirm box.

### Tooltips and onboarding
- One new idea at a time.
- Put the new thing inside a pattern people already know. A familiar tooltip leaves room to
  learn the one thing that's new.
- Tell people how to use it, then get out of the way.

### Consent and permissions
- Lead with what the person gets, then say plainly what you need from them.
- Say the hard part. If the data leaves the device, say so.
- Write each regional version the law requires. Some regions must name the AI up front.

### Loading and success
- Loading says what's happening, and how long if it's long.
- Success confirms what changed. Keep it calm. One line is enough.

## Examples from shipped work

Firefox for iOS, Shake to Summarize (2025). Each pattern above shows up in this copy.

| Element | Copy | Pattern |
|---|---|---|
| Tooltip on a new button | "Tap to summarize this page. Touch and hold for Reader View." | Verb first. Teaches the new action and the old one in two short lines |
| Consent | "Summarize this page? See the main points in seconds with Firefox." | Leads with what you get. No mention of how it works |
| Network error | "Error summarizing page. Try again later." | What happened, one way out |
| Page can't be read | "Limited content detected. This page may be restricted or mostly visual." | Puts the cause on the page, not the person. Hedges because the app can't tell which |

## Output

```markdown
## Copy: [element and screen]

**Recommended:** [copy]

| Option | Copy | Tone | Best for |
|---|---|---|---|
| A | ... | ... | ... |
| B | ... | ... | ... |

**Why it works:** [the person's state, what it tells them, what they do next]

**Reading level:** [grade estimate, and any word you swapped to get there]

**For translators:** [idioms to avoid, room for longer languages, anything cultural]
```

When reviewing copy, quote each line, say which rule it breaks, and give the fix.
