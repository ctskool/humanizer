---
name: humanizer-x
description: "Turn a source (a news story, a link, notes, a transcript, or a draft) into an X (Twitter) post or thread in the user's saved Humanizer voice. Use for /humanizer-x, \"write a tweet about this\", \"turn this into a thread\", or \"humanize this for X\"."
metadata:
  version: 1.0.0
---

# Humanizer for X

Same voice as `/humanizer`, shaped for X. The voice decides how it sounds; the rules below decide the shape.

## 1. Load the voice

Read the voice profile in `~/.humanizer/voices/`: the one the user names, else `default.md`. If there is none, say so, offer to set one up with `/humanizer` ("learn my voice"), and otherwise write in a plain, direct voice.

## 2. Read the source

Find the one idea worth posting. Keep every fact, number, name and link exactly as the source has it. Never invent a statistic, a quote or a result.

## 3. Draft to X's shape

- **Single post by default.** Keep it under 280 characters unless the user says they have a longer limit.
- **A thread only when the idea needs steps or proof.** The first post must stand on its own and make people open the rest. One point per post, 3 to 8 posts. No "🧵" or "1/" unless the voice uses them.
- **Lead with the claim or the result**, not the setup.
- **Plain words, no hashtags,** and emoji only if the voice profile uses them.
- **Links** go in the last post of a thread or in a reply, not the opening post.
- Write two openers and say which one you'd post.

## 4. Humanize it

Run the full `/humanizer` pass on the draft in embedded mode with the same voice: remove the AI tells, keep the facts.

## 5. Hand it over

Return the post or thread with a character count for each post. If a tool that can save X drafts or schedule posts is connected, offer to save it as a draft. **Never post without the user's yes.**
