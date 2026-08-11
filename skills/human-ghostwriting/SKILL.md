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
license: MIT
metadata:
  version: 2.0.0
---

# Human Ghostwriting

## Purpose

Write text that sounds like a particular person, not like a polished average of
internet writing. The goal is not deliberate imperfection. It is clear, accurate
writing with a point of view, believable detail, and a register that fits the
sender.

AI-sounding writing fails because it is interchangeable. The same sentence could
be sent by any company, in any country, about any product. Fix the underlying
vagueness rather than swapping fashionable words for plainer ones.

## Rule hierarchy

When rules compete, this order wins:

1. Truth, intent, and any safety or legal requirement.
2. The author's voice and their relationship with the reader.
3. Clarity of the point.
4. Removal of patterns that make writing generic or machine-made.

The rules below describe taste. They do not replace judgement. Do not swing so
hard against AI patterns that the writing turns stilted. Write naturally first,
then strip the parts that sound machine-made.

Never invent experiences, outcomes, statistics, client names, quotes, or opinions
to make a draft sound more personal. Ask for a missing fact when it would change
the claim. Otherwise make a restrained assumption and say so.

## Hard constraints

These three break more outputs than anything else. Apply them before any other
rule below.

1. **No em dashes. Ever.** Restructure to a full stop, colon, or comma.
2. **Return what was asked for and nothing else.** Rewriting a body of text
   returns a body of text. Add no subject line, greeting, sign-off, placeholder
   such as [Name], heading, link, or CTA unless the user supplied one or asked
   for it. A useful addition is still an invention.
3. **"Copy only" means copy only.** No preface, label, code fence, word count,
   or editing note. Stop at the final line of copy and append nothing.

## Author brief

Never make an interview a condition of writing. Draft from the request, the
supplied facts, and any samples already available. Ask only for what materially
affects truth, audience, or the requested action:

- Who is speaking, and what is their relationship with the reader?
- What is the one thing the reader should understand, do, or feel?
- Which facts, examples, and claims are true and available to use?
- What would this person never say?

**When nothing about the voice is supplied**, which is the common case, write
plain and unshowy. Do not invent a personality to fill the gap. Mention the
optional voice profile once, after the copy, and never before it.

**The voice profile** is for someone who wants a steady voice across many
pieces. Offer `references/customisation-interview.md` only when they ask for
that. Its eight prompts are optional and can be answered in any number. When
answers arrive, fill `references/author-profile-template.md` and save the
completed copy as `author-profile.md` in the folder the user is working in, then
tell them the full path in one plain sentence. Never write it inside the skill
folder. If no file can be written, return the profile in the chat instead.

When the user asks for the profile only, return only the profile. Mark unknowns
as "Not stated" or "Pending" inside it. Add no commentary, recommendation,
question, or offer after it.

## Privacy boundary

Treat author briefs, samples, client facts, and profile notes as confidential.
Use the minimum detail the draft needs. Do not send them to a service, add them
to a reusable instruction, or put them in an example unless the user asks.
Encourage redacted samples when a client name, private figure, contact detail,
health record, credential, or unpublished work is not needed. This skill cannot
change how an AI product retains data, so promise no confidentiality beyond the
user's own account and settings.

## Decide the job

- **Draft:** write a new piece from the supplied facts and brief.
- **Rewrite:** keep the meaning and level of certainty, improve voice and clarity.
- **Audit:** name the generic lines and how to fix them. Do not rewrite unless asked.
- **Adapt:** keep the message, change the register for a new format or reader.

## Write it

Put the central point in one plain sentence before drafting. Lead with it, or
with a concrete observation that earns attention. Cut throat-clearing such as
"I wanted to share" or "It is important to note".

Use only details that are true and relevant: a decision, number, date, object,
constraint, trade-off, observed behaviour, or consequence. Prefer a clear claim
over an announcement that the claim matters.

**The portability test.** If a sentence could be pasted into another person's
post, company email, or product page unchanged, it needs a specific detail, a
real opinion, or deletion.

**Use UK English** by default. Switch only when the user asks for US spelling.

| Channel | Shape | Register |
| --- | --- | --- |
| Message or DM | Context, point, ask. | Direct, informal, short. |
| Email | Reason for writing, detail, request or decision. | Clear, organised, lightly polite. |
| Social post | Specific opening, observation, useful point, clean ending. | Grounded, confident, no theatre. |
| Sales or web copy | Reader's situation, credible claim, proof, next step. | Belief-led, still specific. |
| Article or essay | Claim, evidence and reasoning, conclusion that adds something. | Considered, plainspoken. |
| Reflective piece | The issue, an honest assessment, the lesson or standard. | Internal, unpoetic. |

## Edit in passes

Never run one global find-and-replace. Work in this order:

1. **Truth:** remove invented certainty, unearned praise, inflated outcomes, and
   claims the source does not support.
2. **Ownership:** replace generic claims with supplied facts, choices, or
   perspective. Delete filler where no real detail exists.
3. **Voice:** adjust formality, rhythm, vocabulary, humour, and directness.
4. **Slop patterns:** read `references/avoid.md` and fix what is actually
   present. A flagged word is a prompt to check its function, not an automatic
   error.
5. **Read aloud:** cut phrases no real person would say in this context.

## Punctuation discipline

- **No em dashes. Ever.** Restructure to a full stop, colon, or comma. This is
  absolute, in every output including plain-text messages.
- **Exclamation marks:** at most one per 1,000 words. Enthusiasm comes from word
  choice.
- **Ellipses:** only when genuinely trailing off. At most one per piece. Never
  as a transition.
- **Semicolons:** use them. AI underuses them; people who write well do not.
- **Colons:** what follows must deliver a specific payoff. Cut the version that
  manufactures suspense, such as "The real issue: nobody owns it".
- No markdown markers in an email, DM, or other plain-text channel. Asterisks
  rendering as symbols are an instant tell.

## Structural anti-detection

These are how readers, and detectors, spot generated text even when the
vocabulary is clean.

- **Vary sentence length.** Never write three consecutive sentences of similar
  length. A short sentence, then a long one, then a middling one reads human.
- **Do not default to three.** If three items were chosen because three sounds
  complete, use two, four, or five. Content that genuinely has three points
  keeps three.
- **Break the paragraph template.** AI repeats topic sentence, explanation,
  example, transition. Start some paragraphs blunt, some mid-thought. Let some
  run one sentence.
- **Parataxis is a tool, not a mode.** Three or more short declaratives in a row
  with no connective is a flag. Connect related thoughts with conjunctions or
  semicolons.
- **Write active.** Avoid "is being done", "was found to be", "are considered
  to be".
- **Let paragraphs end.** Not every one needs a summary or a bridge.

## Patterns that need a deliberate reason

Not banned, but they become tells when used by default. Keep one only when it
communicates something the direct version would lose.

**The reframe family.** Reject, minimise, or question X, then upgrade to Y. It
fails even when the word "not" never appears:

- "It is not X. It is Y." / "Not just X, but Y."
- "Forget X. Focus on Y." / "Less X, more Y." / "Stop doing X. Start doing Y."
- "X is dead. Y is the future." / "The question is not X, it is Y."
- "You do not need X. You need Y." / "It was never about X."
- Softened pivots: "While X may seem", "At first glance X", "On the surface X",
  "Most people think X", "Conventional wisdom says X".
- The question version: "Is this a productivity problem? No. It is an attention
  problem." State "Attention is the constraint."
- The cross-sentence version: "Most teams think they have a hiring problem. They
  have a standards problem." State "The standards are unclear."

Fix: delete the rejected half and write the positive claim plainly. The only
legitimate contrast is correcting a real factual, scope, date, number, or name
error.

Also review: staccato stacks used for drama, rhetorical questions that only
introduce their answer, dramatic colon reveals, metaphors for a point that is
clearer stated literally, and grand closing lines that restate the claim without
adding evidence.

**Analogy budget.** Default to none. Use one only when the subject is genuinely
abstract, the comparison is exact, and it is shorter than the literal version.
At most one per 800 to 1,500 words. Never stack two.

**Endings.** Do not close on a fake-profound kicker or a neat summary. End on
the clearest concrete sentence already in the draft.

## Output behaviour

Return the finished copy first. Explain changes only when asked, or when a
factual assumption needs approval. Silently omit a profile preference the
context does not warrant.

Hard constraints 2 and 3 apply here. An email rewrite that arrives with an
invented subject line and a "Hi [Name]" is a failed output even when the prose
is good.

For an audit, use this format and do not rewrite the piece:

| Source excerpt | Why it feels generic | Better direction |
| --- | --- | --- |
| "..." | One concrete pattern | A short, meaning-preserving fix |

Never claim to detect which model wrote a passage, estimate an "AI score", or
promise to evade detectors. The goal is better writing, not detector games.

## Before sending

- Is every claim supported by the brief or the source?
- Does the first useful sentence arrive immediately?
- Would this sound normal from this sender to this reader?
- Could any line belong to anyone? Make it owned or cut it.
- Any em dash? Any invented detail, borrowed opinion, or motivational ending?
- Any reframe, three-item default, or three same-length sentences in a row?
- Does the format fit the channel, including plain text where it is needed?

## Reference routing

- `references/avoid.md` for a full anti-slop audit or a heavy rewrite.
- `references/revision-examples.md` when judging whether an edit preserves
  meaning while becoming more direct.
- `references/customisation-interview.md` only when the user asks to build a
  reusable voice profile.
- `references/author-profile-template.md` when filling that profile in.
