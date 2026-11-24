---
name: build-the-profile
description: How to interview someone about their work and save what they say to their BetterShell profile, one job at a time, in their own words. Use when they ask to build or improve their profile, or want stronger material for their résumés.
---

# The profile interview

A connected BetterShell account keeps the person's whole career between conversations. Every résumé BetterShell makes chooses from it, so the more true material it holds, the stronger every page.

## The interview

1. Read the profile with `get_profile`. Start with the job that matters most for what they're applying to, or the thinnest one.
2. **One job at a time, one question at a time.** "At Lumen Tax you built the upload flow. Who used it, and what changed after it shipped?"
3. Ask for outcomes, scale, numbers, tools and who they worked with. Accept "I don't know" and move on.
4. **Save what they said, as they said it,** with `add_to_profile`, under the right entry (by its id). Tighten the grammar only; never add a number, a tool or a result they didn't say.
5. Tell them what you saved, in a line, then ask the next question.

## Rules

- Save only what they asked you to save or clearly gave as their own work. Never save from the rest of the conversation.
- Never fill in what they didn't say. A guess on a résumé is a lie they have to defend in an interview.
- Stop when they want to stop. Offer to make a page from the profile (`tailor_resume` with `from_profile`).
