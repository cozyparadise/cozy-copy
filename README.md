# cozy-copy

UX copy an agent can write at an 8th-grade reading level.

```bash
npx skills add cozyparadise/cozy-copy
```

Ask an agent for a button and you get "Submit". Ask for an error message and you get an apology with no way out. This skill gives it a pattern for each kind of copy, a reading level to hit, and the words already on your screen to match.

The sharpest rule is that **an error never blames the person.** It names what happened, puts the cause where it really is, and gives one way out. When Firefox can't summarize a page that's locked or mostly images, it says "Limited content detected. This page may be restricted or mostly visual." The page is the limit, not you and not Firefox.

## What it covers

| Copy | The pattern |
| --- | --- |
| Buttons | Verb first, name the thing, say what happens |
| Errors | What happened, why, one way out. No blame |
| Empty states | What goes here, why it's empty, a button to start |
| Confirmations | Name the action and the count. Undo beats "Are you sure?" |
| Tooltips and onboarding | One new idea, inside a pattern people already know |
| Consent | What you get first, then the hard part, said plainly |
| AI features | Say what it does, not how it works |

## Use it

```
/cozy-copy write the empty state for a new team's project list
/cozy-copy review "Oops! Something went wrong. Please try again later."
```

Before writing, it asks where the copy lives, what the person is doing, the tone, and any limits. It gives one pick, a few alternatives, why the pick works, a reading-level check, and notes for translators.

## Why 8th grade

Most US adults read most comfortably at about that level, and nobody reads interface copy slowly. Plain words help experts too.

## Where it comes from

- **Anthropic's `ux-copy`** skill, from the Design plugin in [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (Apache 2.0), gave the shape. Ask for context first, use a pattern per element, give alternatives with reasons. This skill rewrites it in plain words and adds its own rules.
- **Shipping Shake to Summarize in Firefox for iOS** (2025) gave the rest. That meant introducing a new gesture, asking for consent on an AI feature from users who don't trust AI, writing consent with legal, and writing errors with Firefox's copy team. The examples in the skill are the shipped strings, found in Mozilla's open-source [firefox-ios](https://github.com/mozilla-mobile/firefox-ios) repo.

UX standards beyond copy live in [cozy-ux](https://github.com/cozyparadise/cozy-ux). Motion craft lives in [tune-animations](https://github.com/cozyparadise/tune-animations).

## License

MIT
