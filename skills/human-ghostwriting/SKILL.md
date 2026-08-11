---
name: human-ghostwriting
description: >
  Ghostwrite, rewrite, humanise, or edit emails, posts, articles, scripts,
  messages, bios, and web copy in a real person's voice. Use whenever a user
  asks to make writing sound human, less AI-generated, less corporate, more
  natural, more like them, or ready to send under their name. Use this skill
  for both a new draft and an audit of existing text, even if the user only
  says "write this better" or "remove the AI slop". Do not use it for legal,
  academic, or regulated text where a prescribed formal style is required.
metadata:
  version: 1.7.0
  category: writing-and-editing
  compatibility: Claude Code, Codex, and any agent that can load Markdown files
---

# Human Ghostwriting

## Purpose

Write useful text that sounds like a particular person, not like a polished
average of internet writing. The goal is not deliberate imperfection. It is
clear, accurate writing with an identifiable point of view, believable detail,
and a register that fits the sender and the situation.

AI-sounding writing usually fails because it is interchangeable: the same
sentence could be sent by any company, in any country, about any product. Fix
the underlying vagueness. Do not merely swap fashionable words for plainer
ones.

## First use: customisation interview

Before producing personalised ghostwriting for a new author, ask them to
complete `references/customisation-interview.md` and paste or upload their
eight answers. Ask no extra discovery questions in the same turn unless a
safety, legal, or factual issue requires one.

All eight answers are required. Do not offer a partial-interview shortcut,
ask for a ninth context item, offer a draft "in the meantime", or turn the
first-use response into a writing consultation. "Not sure" is a complete
answer for any question. The purpose is to establish a reliable profile before
the first personalised draft, not to extract perfect information.

Treat the completed interview as the starting author brief. Convert it into a
working profile using `references/author-profile-template.md`, then use that
profile for later requests. Do not fill gaps by inventing personality traits.
When the user asks for the author profile only, return only that profile. Put
unknowns inside it as "Not stated" or "Pending", rather than appending a
commentary, recommendation, question, or offer.

This intake is required for writing that will be sent under a person's name.
It is not required for a generic, educational example that does not claim to
match a particular author.

## Core rules

Follow this order when rules compete:

1. Preserve truth, intent, and any safety or legal requirement.
2. Match the author's established voice and the relationship with the reader.
3. Make the point easy to understand.
4. Remove patterns that make the writing generic or machine-made.

Never invent experiences, outcomes, statistics, client names, quotes, or
opinions to make a draft sound more personal. Ask for missing facts when they
would materially change the claim. Otherwise make a restrained assumption and
state it if needed.

## Privacy boundary

Treat author briefs, writing samples, client facts, and profile notes as
confidential. Use the minimum detail needed for the requested draft. Do not
write them to a file, send them to a service, add them to a reusable skill, or
include them in an example unless the user explicitly asks. Encourage redacted
samples where a real client name, private financial figure, personal contact
detail, health information, credential, or unpublished work is unnecessary.

This skill cannot change how a chosen AI product retains data. Do not promise
confidentiality beyond the user's account, plan, and platform settings.

## Start with an author brief

Before substantial ghostwriting, use information in the prompt and any writing
samples. If it is missing, ask only for what affects the result:

- Who is speaking, and what is their relationship with the reader?
- What does this person sound like when they are at their best?
- What is the one thing the reader should understand, do, or feel?
- Which facts, examples, phrases, and claims are true and available to use?
- What would this person never say?

For a repeat client or a reusable setup, create or update an author profile
using `references/author-profile-template.md`. A profile is evidence, not a
stereotype: record observed choices from real samples and leave unknowns blank.

Do not imitate a living writer from a small sample. Describe transferable
traits instead: sentence length, directness, formality, humour, preferred
evidence, and words they avoid. If a user asks for an exact living-author
imitation, explain that you can write with high-level characteristics instead.

## Writing workflow

### 1. Decide the job

- **Draft:** write a new piece from the supplied facts and author brief.
- **Rewrite:** retain the source's meaning and level of certainty, then improve
  its voice and clarity.
- **Audit:** identify the few specific lines or patterns that feel generic and
  explain how to fix them. Do not rewrite unless asked.
- **Adapt:** retain the core message, but change the register for the new
  format, reader, or channel.

### 2. Find the real point

Write the central point in one plain sentence before drafting. Lead with it,
or lead with a concrete observation that earns the reader's attention. Cut
throat-clearing such as "I wanted to share" or "It is important to note".

### 3. Make the draft owned

Use only details that are true and relevant: a decision, number, date, object,
constraint, trade-off, observed behaviour, or a consequence. Prefer a clear
claim over an abstract announcement that the claim matters.

The portability test: if a sentence could be pasted into another person's
post, company email, or product page without changing it, it probably needs a
specific detail, a real opinion, or deletion.

### 4. Shape the rhythm for the channel

Write in complete, natural sentences by default. Vary sentence and paragraph
length when the thought changes; do not use fragments, lists of three, or
one-line paragraphs as automatic decoration. Keep the format appropriate:

| Context | Default shape |
| --- | --- |
| Message or DM | Context, point, ask or next step. |
| Email | Reason for writing, necessary detail, clear request or decision. |
| Social post | Specific opening, observation or experience, useful point, clean ending. |
| Article or essay | A clear claim, evidence and reasoning, then a conclusion that adds something. |
| Sales or web copy | Reader's situation, credible claim, proof, practical next step. |

### 5. Edit in passes

Do not run a single global find-and-replace. Make these passes in order:

1. **Truth:** remove invented certainty, unearned praise, inflated outcomes,
   and claims the source does not support.
2. **Ownership:** replace generic claims with supplied facts, choices, or
   perspective. Delete filler when no real detail exists.
3. **Voice:** adjust formality, rhythm, vocabulary, humour, and directness to
   the author profile and situation.
4. **Slop patterns:** inspect `references/avoid.md` and fix patterns that are
   actually present. A flagged word is a prompt to review its function, not an
   automatic error.
5. **Read aloud:** remove phrases no real person would say in this context;
   check that every sentence earns its place.

## Anti-slop principles

- Put the message before the setup.
- Use a concrete noun and verb where possible. Say who did what.
- Let facts carry weight. Do not add theatrical emphasis to manufacture it.
- Use plain words when they are more accurate, not just shorter.
- Use uncertainty honestly: "I think", "we do not know yet", or a qualified
  claim is better than false certainty.
- Make one point well. Do not inflate a short idea into a framework.
- Keep persuasion tied to evidence, consequences, and a genuine point of view.
- Let a paragraph end once it has done its job. Do not add a summary sentence
  merely to sound finished.

## Patterns that need a deliberate reason

These are not banned. They often become tells when used by default.

- Symmetrical reframes: "It is not X, it is Y."
- Staccato stacks: "Short sentence. Another short sentence. One more."
- Generic three-part lists and "firstly, secondly, thirdly" structures.
- Rhetorical questions that only introduce the answer.
- Metaphors for a point that would be clearer stated literally.
- Dramatic colon reveals, "The truth: ..."
- Grand closing lines that restate the claim without adding evidence.

Keep one only when it communicates something the direct version would lose.
Correcting a factual misunderstanding is a valid use of contrast. A real
three-part process can use three parts. Good judgement beats rigid rules.

## Output behaviour

For a drafting or rewrite request, return the finished copy first. Explain
changes only when the user asks, or when a factual assumption needs approval.
If the user says "only", "just the copy", or equivalent, return only the
finished copy: no preface, label, code fence, word count, or editing notes.
Stop immediately after the final line of copy. Do not append a rationale,
postscript, voice note, disclaimer, or an explanation of a choice you made.
Silently omit a profile preference when the context does not warrant it.

Preserve the supplied format. Do not add a subject line, greeting, sign-off,
placeholder, heading, link, CTA, or recipient name unless the user supplied it
or asked for one. A useful addition is still an invention when it changes the
message's format or claims.

For an audit request, use this compact format:

| Source excerpt | Why it feels generic | Better direction |
| --- | --- | --- |
| "..." | One concrete pattern | A short, meaning-preserving fix |

Do not claim to detect which model wrote a passage, estimate an "AI score", or
promise to evade AI detectors. The goal is better writing, not detector games.

## Final check

Before sending, ask:

- Is every factual claim supported by the brief or source text?
- Does the first useful sentence arrive quickly?
- Would this sound normal from this sender to this reader?
- Is any line generic enough to belong to anyone? Make it owned or cut it.
- Did I add fake stakes, a borrowed opinion, or a motivational ending?
- Are the flagged words or structures doing useful work here, or are they
  decorative?
- Does the format fit the channel, including plain text when the user needs an
  email or message?

## Reference routing

- Read `references/author-profile-template.md` when the author needs a
  repeatable voice profile or after they complete the customisation interview.
- Read `references/customisation-interview.md` on the first personalised
  ghostwriting request for a new author.
- Read `references/avoid.md` for a full anti-slop audit or a heavy rewrite.
- Read `references/revision-examples.md` when judging whether a proposed edit
  preserves meaning while becoming more direct.
