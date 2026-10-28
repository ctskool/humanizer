---
name: humanizer-linkedin
description: "Turn a source (a news story, a link, notes, a transcript, or a draft) into a LinkedIn post in the user's saved Humanizer voice. Use for /humanizer-linkedin, \"turn this into a LinkedIn post\", \"write a LinkedIn post about this\", or \"humanize this for LinkedIn\"."
metadata:
  version: 1.0.0
---

# Humanizer for LinkedIn

Same voice as `/humanizer`, shaped for LinkedIn. The voice decides how it sounds; the rules below decide the shape.

## 1. Load the voice

Read the voice profile in `~/.humanizer/voices/`: the one the user names, else `default.md`. If there is none, say so, offer to set one up with `/humanizer` ("learn my voice"), and otherwise write in a plain, direct voice.

## 2. Read the source

Find the one idea worth posting and why it matters to the user's audience. Keep every fact, number, name and link exactly as the source has it. Never invent a statistic, a quote or a result. If the source is a link, read the page; if it's thin, say so.

## 3. Draft to LinkedIn's shape

- **The first two lines carry the post.** LinkedIn shows about two or three lines before "see more", so the hook and the stakes go there. No throat-clearing ("I've been thinking a lot about...").
- **One idea.** 120 to 300 words is the usual range; the limit is 3,000 characters.
- **Short paragraphs**, one or two sentences each, with a blank line between them. Lists only if the voice uses them.
- **Your take, not a summary.** Say what you think and what the reader should do or watch for.
- **End on a real point** or a specific question, never a bare "Thoughts?".
- **Hashtags:** none, or up to three at the end. Emoji only if the voice profile uses them.
- **Links:** if the post needs one, offer to put it in the first comment instead of the body.

## 4. Humanize it

Run the full `/humanizer` pass on the draft in embedded mode with the same voice: remove the AI tells, keep the facts.

## 5. Hand it over

Return the post and, on one line, the hook you chose. If a tool that can save LinkedIn drafts is connected, offer to save it there. **Never post without the user's yes.**
