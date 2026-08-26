---
name: cornell-notes
description: Cornell-method notes from an article or web link. Notes, a summary, a fact-checked review, and a condensed paper-ready version, saved as one consolidated Notion page — then an optional translation, asked for, never assumed.
argument-hint: [article URL]
---

## What this is for

Turns a single article URL into Cornell-style notes, run end to end, no stopping
between steps unless one surfaces something that needs a decision.

Stages 1-4 are working steps, not output — do not print their results to chat.
Run them silently and carry each stage's output into the next. Nothing goes to
the user until the final Output section.

## Stage 1 — Notes

Fetch the source content from the given URL. Produce only the cue column and the
main notes — no summary yet.

- Cue column: 4-8 self-test questions covering the article's main sections, in
  the order they appear.
- Notes: key points as terse paraphrases in your own words, never verbatim
  quotes. Organize by the article's own headers.
- Tag any claim that does not appear in the fetched text with `[video]`.

## Stage 2 — Summary

Using only the source article and the stage 1 notes, write a summary in your own
words — an interpretation, not a restatement. 2-4 sentences, capturing the core
takeaway of the whole article.

## Stage 3 — Review

Check the summary and notes for accuracy against the source. Use web search to
verify any claims that are time-sensitive or version-specific. List any
discrepancies found. Produce a corrected version of the document.

## Stage 4 — Polish

Condense the corrected document into a version ready to hand-copy onto paper: no
`[video]` tags, no reviewer notes, maximally terse.

## Stage 5 — Save to Notion

Save one consolidated page — not two separate documents — as a row in the
"Cornell Notes" database (data source `898d28a7-add3-48a2-9b30-b85bf2c53b53`),
not as a standalone private page. Set its properties: `Name` = article title,
`Source URL` = the input URL, `Date` = today, `Language` = `EN` (or the
translated language if Stage 6 ran instead of the English version). Page
content:

- The reviewed Cornell document: cue column, notes, summary.
- A short "Reviewer notes" section: what was checked and what changed.
- A "Paper-ready" section holding the Stage 4 condensed version.

Keep it consolidated, not two redundant write-ups stapled together — the
paper-ready section should read as a tightened distillation of the material
above it, not a repeat of it.

## Output

Show only the Notion page link in chat. Then ask whether the user wants a
translation of the page — optional, never run without being asked. If yes, ask
which language (default to Polish if the user doesn't say, per this machine's
usual translation target) and replace the page's content in place with the
translated version — same page, same structure (cue column, notes, summary,
reviewer notes, paper-ready), fully translated. Do not append the translation
below the English text; the translation is a swap, not an addition. Update the
row's `Language` property to match.
