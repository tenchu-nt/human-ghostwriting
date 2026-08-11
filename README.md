# Human Ghostwriting

Makes AI write like a person instead of like a press release. It removes the
words and sentence patterns that make text obviously machine-written, keeps
whatever facts you gave it, and never invents a story about you to sound more
personal.

It works for emails, social posts, messages, articles, bios, and web copy. It
does not promise to beat AI detectors, and it will not pretend to be a specific
famous writer.

## Install it

You need Claude Code or Codex already installed. Then:

1. Open Terminal. Press **Cmd + Space**, type `Terminal`, press **Return**.
2. Copy the line below, paste it into the black window, press **Return**.

```
npx --yes skills@latest add tenchu-nt/human-ghostwriting -g -a claude-code -a codex -y
```

3. Wait for it to finish. It takes under a minute.
4. Close Claude Code or Codex completely, then open it again.

**If you see `command not found: npx`**, you need Node.js first. Go to
[nodejs.org](https://nodejs.org), click the big green download button, open the
file it downloads, and click Continue until it finishes. Then paste the command
from step 2 again.

**If you would rather not use Terminal**, see "Install by hand" at the bottom.

## Check it worked

Start a new chat in Claude Code or Codex and paste this:

```
Rewrite this so it sounds like a person: I hope this email finds you well. I
wanted to circle back regarding the deliverables and leverage our synergies
moving forward.
```

If it comes back short, plain, and direct, it is working. If it comes back
sounding the same, close the app and reopen it.

## How to use it

You do not have to set anything up. Just ask:

- "Humanise this email, keep every fact, and make the ask clear."
- "Write a LinkedIn post about this. Do not invent any numbers."
- "Audit this page for generic AI language. Do not rewrite it."
- "Turn this technical update into a short client message that sounds calm."

It writes in UK English unless you ask for US spelling.

## Optional: teach it your voice

If you want it to sound like *you* rather than just sound human, ask it to build
your voice profile. It will ask you up to eight questions, save the answers to a
file called `author-profile.md` in whatever folder you are working in, and tell
you where that file is. Attach that file to future requests.

This is optional. Skip it and it still writes.

## ChatGPT

ChatGPT cannot install this automatically. Open
[CHATGPT.md](skills/human-ghostwriting/CHATGPT.md) and follow the five steps.

## Install by hand

Use this if the command did not work, or if someone sent you the folder
directly.

1. Download this repository (green **Code** button, then **Download ZIP**) and
   unzip it. Inside you will find a folder called `human-ghostwriting`.
2. In Finder, press **Cmd + Shift + G**, type `~/.claude/skills`, press
   **Return**. If that folder does not exist, go to `~/.claude` and create a new
   folder called `skills`.
3. Drag the `human-ghostwriting` folder into it.
4. For Codex, do the same with `~/.codex/skills`.
5. Close the app and open it again.

## Updating and removing

```
npx skills update human-ghostwriting
npx skills remove human-ghostwriting
```

## Privacy

There is no code in this, no tracking, and nothing that connects to the
internet. It is a set of written instructions. It tells the AI to use the least
personal detail it needs and not to save your writing samples anywhere you did
not ask for. Your own ChatGPT, Claude, or Codex account settings still control
what those companies keep.

Do not paste passwords, client contracts, health information, or anything you do
not have permission to share.

## Licence

MIT. Use it, change it, sell work made with it. Keep the licence notice with any
copy you pass on.
