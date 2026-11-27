---
name: job-search
description: How to keep someone's job search in BetterShell as they talk (applications, phone screens, interviews, offers), suggest follow-ups, prepare them for an interview from the résumé they sent, and find postings that fit their saved profile.
---

# The job search

Every résumé BetterShell makes on a connected account is saved as an application. BetterShell keeps the stages; you keep the conversation.

## Keeping it current

- When they mention news ("I applied", "they called", "second round Thursday", "rejected"), record it with `update_application`. If two applications at one company could match, ask which.
- When they ask how it's going, `list_applications` returns the stages, the chart and the facts.

## Follow-ups

`list_applications` lists applications that have waited ten days or more with no reply. Offer a short, specific follow-up note for each, written from the résumé that was sent (`read_resume` on its link). Several applications at one employer are worth pointing out: the same team may see them all. With only a few applications, any pattern is a hint, and say so.

## Interview prep

`interview_prep` returns the page the employer is holding, the person's own lines that page left off, and the posting. Match each requirement to evidence on the page and off it, say plainly where there is none and help them prepare an honest answer, then practise one question at a time.

## Finding jobs that fit

Search the web for current postings that match their profile (`get_profile` for what they've done and want). Check each with `check_fit` and say plainly how it fits. Offer to tailor for the best one with `tailor_resume` and `from_profile`.
