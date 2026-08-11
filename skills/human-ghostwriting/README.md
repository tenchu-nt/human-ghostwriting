# Human Ghostwriting

A portable skill for drafting and editing writing in a real person's voice.
It reduces generic, over-polished AI writing through author evidence, concrete
detail, and a review of common slop patterns. It does not imitate a specific
person by default and it does not promise to bypass AI detectors.

Released under the MIT License. See `LICENSE`.

## Privacy

The skill has no code, telemetry, network calls, or external data store. It
instructs the agent to use only the minimum personal context needed and not to
write samples or author profiles to files or external services without explicit
user direction. Redact client names, credentials, contact details, private
financial figures, health information, and unpublished work unless they are
needed for the request. Your AI product's own account, plan, and retention
settings still apply.

## Package contents

```text
human-ghostwriting/
├── CHATGPT-INSTRUCTIONS.md
├── SKILL.md
├── evals/evals.json
└── references/
    ├── author-profile-template.md
    ├── customisation-interview.md
    ├── avoid.md
    └── revision-examples.md
```

## Install in one command

Open Terminal, paste this, and press Return:

```bash
npx --yes skills@latest add tenchu-nt/human-ghostwriting --copy -y
```

There is only one skill in the repository. The installer detects compatible
coding agents such as Claude Code and Codex and installs it without requiring
the user to select a skill. Start a new chat when it finishes and ask for
writing, rewriting, humanising, or a tone audit.

## ChatGPT

ChatGPT does not install local skills from a terminal command. Create a custom
GPT or project instruction named "Human Ghostwriting", then paste
`CHATGPT-INSTRUCTIONS.md` into its instructions and upload the four files in
`references/` as knowledge, including `customisation-interview.md`. For an
ordinary chat, paste those instructions
first, then provide the author brief and writing request in the same
conversation.

## Optional evaluation prompts

`evals/evals.json` contains six realistic prompts for checking a new
installation: an immediate first-use draft, an email rewrite, a founder post,
an audit, profile-only output, and privacy-safe optional onboarding. Review
the output for truthfulness, voice fit, concrete detail, privacy, and whether
it avoids replacing one formula with another.

## Optional customisation

Write immediately with the context you have. For a reusable author profile or
more consistent voice across future work, optionally complete any or all of
[the eight customisation prompts](references/customisation-interview.md), then
ask the skill to build an author profile. It will not delay a draft while
waiting for answers.

## First-use prompt

```text
Use the Human Ghostwriting skill. Draft [format] for [reader].

Optional author profile or voice notes: [attach if available]

Author: [role and relationship to the reader]
Voice: [direct/formal/warm/dry, plus 2-3 approved samples or traits]
Point: [one thing the reader should understand, do, or feel]
Facts I can stand behind: [facts, numbers, examples]
Avoid: [words, claims, or tones]
```

For a repeat author, complete `references/author-profile-template.md` once and
include it with later requests.

## Example requests

- "Humanise this email, keep every fact, and make the ask clear."
- "Write this LinkedIn post in my author profile. Do not invent numbers."
- "Audit this landing-page section for generic AI language. Do not rewrite it."
- "Turn this technical update into a short client message that sounds direct
  and calm."
