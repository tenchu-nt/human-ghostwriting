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

## Claude Code

Copy the `human-ghostwriting` folder into a skills directory that Claude Code
loads, such as `~/.claude/skills/` for a personal skill or `.claude/skills/`
inside a repository. Restart or start a new session, then ask for writing,
rewriting, humanising, or a tone audit. The frontmatter description is designed
to trigger the skill for those requests.

## Codex

Copy the folder to the skill location your Codex environment exposes, or keep
it in the repository under `.claude/skills/` when that is part of the agent's
skill-discovery convention. The agent should read `SKILL.md` and any reference
file selected in its **Reference routing** section before writing.

## ChatGPT

ChatGPT does not automatically discover local skill folders. Create a custom
GPT or project instruction named "Human Ghostwriting", then paste
`CHATGPT-INSTRUCTIONS.md` into its instructions and upload the four files in
`references/` as knowledge, including `customisation-interview.md`. For an
ordinary chat, paste those instructions
first, then provide the author brief and writing request in the same
conversation.

## Optional evaluation prompts

`evals/evals.json` contains six realistic prompts for checking a new
installation: the first-run intake, an email rewrite, a founder post, an
audit, profile-only output, and privacy-safe onboarding. Review the output for
truthfulness, voice fit, concrete detail, privacy, and whether it avoids
replacing one formula with another.

## First use: customise the skill

1. Complete [the eight-question interview](references/customisation-interview.md).
2. Paste or upload the answers with your first personalised writing request.
3. Review the resulting author profile before using it for important writing.

The interview is deliberately mandatory for personalised ghostwriting. It
prevents the skill from guessing at a voice or inventing personal texture from
too little context. It is not needed for generic examples.

## First-use prompt

```text
Use the Human Ghostwriting skill. Draft [format] for [reader].

I have attached my completed eight-question customisation interview.

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
