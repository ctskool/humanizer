# Voice setup: learn how the writer writes

Follow this file when the user asks Humanizer to learn their voice, set up or update a voice, or write like a writer they admire. The result is a voice profile that every later rewrite reads first.

Work one step at a time. Wait for the user at each step.

## 1. Ask what the voice is for

Ask two things:

- **Whose voice?** Their own, or a writer they want to sound more like. For another writer, learn the style only: sentence shape, rhythm, and habits. Never reuse that writer's lines, and never present the result as that writer's work.
- **For what?** Everything they write, or one channel, such as LinkedIn, email, newsletters, or video scripts. One profile per channel is fine. Name the profile after its use: `default`, `linkedin`, `email`.

## 2. Collect samples

Ask for three to ten pieces, about 1,500 words in total. More helps, up to roughly 5,000 words. They can paste text or name files or folders. Good samples:

- come from the person whose voice this is, without heavy AI help
- match the use from step 1 (LinkedIn samples for a LinkedIn voice)
- are recent, since voices drift

Transcripts of the person talking (videos, podcasts, voice notes) work well for word choice, rhythm, and how they explain things. Their punctuation comes from the transcription tool, not the person, so for transcripts take punctuation habits from the interview instead of measuring them.

If they only have a little, take it and say the profile will improve with more.

## 3. Interview

Skim the samples first, then ask three or four questions at a time, skipping any the samples already answer. Stop when the answers stop adding anything, usually after eight to twelve questions.

- Who reads this, and what do they already know?
- How should a reader feel after reading?
- How formal are you, on a scale from texting a friend to writing a contract?
- Words or phrases you use on purpose?
- Words or phrases you never want to see?
- How do you usually open? How do you usually close?
- Do you use humor? What kind?
- Emoji, exclamation marks, dashes, all caps, sentence fragments: which do you use, and how often?
- Any rules from an editor, a style guide, or your own pet peeves?
- Paste a line you love that you wrote, and one you hate.

## 4. Study the samples

Measure what you can and describe the rest. Quote only short phrases as examples. Look for:

- **Sentences:** typical length, shortest, longest, and how often length changes.
- **Paragraphs:** typical length; one-line paragraphs and when they appear.
- **Punctuation:** rate of dashes, colons, parentheses, exclamation marks, questions, emoji, and ellipses.
- **Person and tone:** I, you, or we; contractions; slang; profanity.
- **Openings and closings:** how pieces and paragraphs start and end.
- **Signature moves:** phrases they repeat, the kinds of examples they reach for, and how they handle numbers.
- **Formatting:** headings, lists, bold, and line breaks.

Where the samples and the interview disagree, the samples show what they do and the interview shows what they want. Note both and ask which wins.

Some habits in the samples may be tells from §1 to §5 of `SKILL.md`, such as "not X but Y" or a staged "Here's the thing." Don't record those as signature moves. Point them out instead, and keep one only if the user says it's deliberate; then list it under Rules.

## 5. Write the profile

Fill in `voice-profile-template.md` from this skill's folder. Keep the profile under 600 words: every rewrite reads it. Leave out any section the samples and interview gave you nothing useful for. Show it to the user and ask what's wrong or missing. Revise until they agree it sounds like them.

## 6. Test it

Take a paragraph of stiff, AI-sounding text on the user's own topic. Write one if they don't have any. Rewrite it with the full Humanizer process plus the new profile. Show the before and after, and ask whether the after sounds like them. Adjust the profile and test again until it does.

## 7. Save it

Save the profile as `~/.humanizer/voices/<name>.md`, creating the folder if needed. If the agent can't write files, give the user the profile to save themselves and tell them to paste it in with their text.

Then tell the user how to use it:

- `/humanizer` with their text uses the `default` voice when it exists.
- "Use my linkedin voice" picks a named profile.
- "Update my voice" adds new samples, repeats steps 3 to 6, and saves over the old profile.

## Privacy

The profile records style, not content. Don't save the samples, personal details, client names, or anything the user calls private. Short quoted phrases are fine when they show a habit.
