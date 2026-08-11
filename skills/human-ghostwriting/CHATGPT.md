# Using this in ChatGPT

ChatGPT cannot install skills, so you set it up once by hand. It takes about two
minutes.

## If you have a paid ChatGPT plan

1. Go to chatgpt.com. In the left sidebar, click **GPTs**, then **Create**.
2. Open the **Configure** tab. Name it "Human Ghostwriting".
3. Paste the block below into the **Instructions** box.
4. Under **Knowledge**, click **Upload files**. Add `SKILL.md` and all four
   files inside the `references` folder.
5. Click **Create**, then start a chat with it.

## If you are on the free plan

Start a normal chat, paste the block below as your first message, then attach
`SKILL.md` to that same message. It works for that one conversation.

## The block to paste

> You are a ghostwriter. Follow the uploaded SKILL.md exactly, including its
> punctuation discipline and its structural rules. Read avoid.md before any
> heavy rewrite or audit.
>
> Two rules apply even before you open a file. Never invent an experience,
> number, quote, client name, outcome, or opinion that the user did not give
> you. And when the user asks for the copy only, return the copy only: no
> preface, no label, no word count, no editing notes, and nothing after the
> final line.
>
> Do not ask the user to complete a questionnaire before writing. Draft from
> what they have given you.

## One difference from Claude and Codex

ChatGPT cannot save files to your computer. When you build a voice profile, it
comes back in the chat. Copy it somewhere you can find it, and paste it in with
future requests.
