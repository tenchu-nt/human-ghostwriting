# Human Ghostwriting

Human Ghostwriting is a portable skill for drafting and editing writing in a
real person's voice. It keeps the writing specific, accurate, and natural
without relying on a brittle blacklist of words.

## Install

Open Terminal, paste this command, and press Return:

```bash
npx --yes skills@latest add tenchu-nt/human-ghostwriting --copy -y
```

That is the only command needed. The repository contains one skill, so the
installer finds it automatically without requiring the user to choose a skill.
It detects compatible coding agents such as Claude Code and Codex.

## Use it immediately; customise only if helpful

Write with the context already in your request. The optional
[eight-question customisation guide](skills/human-ghostwriting/references/customisation-interview.md)
is for people who want a reusable author profile or more consistent voice
across future work; answer any number of prompts, or skip it entirely.

For ChatGPT, paste [CHATGPT-INSTRUCTIONS.md](skills/human-ghostwriting/CHATGPT-INSTRUCTIONS.md) into a custom GPT or project instruction, then upload the
four files in `skills/human-ghostwriting/references/` as knowledge.

## What is included

- `skills/human-ghostwriting/SKILL.md`: the portable Claude Code and Codex
  skill.
- `references/customisation-interview.md`: an optional eight-prompt guide for
  building a reusable profile.
- `references/author-profile-template.md`: the resulting reusable author
  profile.
- `references/avoid.md`: words, phrases, and writing patterns to review.
- `references/revision-examples.md`: meaning-preserving editing examples.

The skill does not promise detector evasion. It is designed to make writing
more specific, grounded, and recognisably owned by the sender.

## Licence

MIT. You may use, modify, distribute, and use the skill commercially, provided
that the copyright and licence notice stay with substantial copies.

## Privacy

The skill contains no executable code, telemetry, network calls, or external
data store. Do not enter private client data, credentials, contact details,
health information, private financial figures, or unpublished work unless it
is necessary and you have permission to use it.
