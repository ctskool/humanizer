---
name: humanizer-email
description: "Turn a source (a news story, a link, notes, a transcript, or a draft) into an email or newsletter in the user's saved Humanizer voice. Use for /humanizer-email, \"write an email about this\", \"turn this into a newsletter\", or \"humanize this email\"."
metadata:
  version: 1.0.0
---

# Humanizer for email

Same voice as `/humanizer`, shaped for an inbox. The voice decides how it sounds; the rules below decide the shape.

## 1. Load the voice

Read the voice profile in `~/.humanizer/voices/`: the one the user names, else `default.md`. If there is none, say so, offer to set one up with `/humanizer` ("learn my voice"), and otherwise write in a plain, direct voice.

## 2. Read the source and pick the kind

Keep every fact, number, name and link exactly as the source has it. Never invent a statistic, a quote or a result. Then pick one:

- **Newsletter** (to a list): one main story, the user's take on it, and one link or action.
- **One-to-one** (to a person): written to them by name, about their situation, with one clear ask.

Ask only if you can't tell.

## 3. Draft to the inbox's shape

- **Subject line:** specific, under about 50 characters, no clickbait. Give two options.
- **Preview text:** one line that adds to the subject instead of repeating it.
- **Open with the point.** No "I hope this finds you well."
- **Short paragraphs,** plain text feel, and one ask or one link that matters.
- **Sign off** the way the voice profile does.

## 4. Humanize it

Run the full `/humanizer` pass on the draft in embedded mode with the same voice: remove the AI tells, keep the facts.

## 5. Hand it over

Return the subject options, preview text and body. If an email tool is connected (Gmail, for example), offer to save it as a draft. **Never send without the user's yes.**
