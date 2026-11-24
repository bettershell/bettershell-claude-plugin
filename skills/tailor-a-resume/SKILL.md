---
name: tailor-a-resume
description: How to make a tailored résumé with BetterShell when someone shares their résumé or CV and a job (a posting link, its text, or the kind of role). Covers what to send, when to ask for more, and how to present the finished page.
---

# Tailoring a résumé with BetterShell

BetterShell's `tailor_resume` makes a finished one-page PDF from the person's own résumé: it picks their strongest material for the job, rewrites lines toward the posting's language without adding facts, and fits the page in the look their content fills. Your part is the conversation.

## Before calling

1. **Send everything they've shared.** Every job, project and activity, every line, word for word. If they attached a file and the tool takes `resume_file`, pass the file. If they told you more in the chat, include it. Never trim to "keep it short": choosing is BetterShell's job, and it chooses better from more.
2. **Send the job.** The posting's full text is best; a link works (`read_job_posting` shows what it asks for); a kind of role works when there's no posting.
3. **If they've connected BetterShell and have a saved profile,** `from_profile: true` makes the page from all of it with no résumé to send.

## When it asks first

`tailor_resume` may answer `needs_more`, for instance when the résumé would fill only part of the page. Ask the questions in one message, in your own words, and name anything the posting wants that the résumé doesn't show. Then call again with the `asked` value it gave and what they added. Going ahead with nothing added is their decision, never yours: don't offer it as the easy way out, and don't decide it for them.

## When it's made

- The card shows the page, what BetterShell picked and changed, and a **Download PDF** button. Don't repeat the résumé's text or the links when the card is there.
- Say in a sentence what it did for this job, in plain words.
- Offer the next step that fits: a change to a line or the look (`edit_resume`), the next application, or interview prep.

## A matching cover letter

When they want a cover letter for a job BetterShell made their résumé for, read the résumé (`read_resume`), write the letter from its facts and what they tell you (never a claim the résumé doesn't support; under 350 words), and send the paragraphs with the résumé's link to `make_cover_letter`. BetterShell prints it as the résumé's pair: same header, type and colours, one page.

## Changes after

Use `read_resume` for the line ids, write the new words from the person's own facts, and send them with `edit_resume`. BetterShell fits the page again and redraws the PDF.
