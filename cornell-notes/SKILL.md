---
name: cornell-notes
description: Cornell-method notes from an article or web link. Four stages in sequence — cue-column notes, a summary, a fact-checked review saved to Notion, and a paper-ready condensed version.
argument-hint: [article URL]
---

## What this is for

Turns a single article URL into Cornell-style notes, run end to end through four
stages, no stopping between them unless a stage surfaces something that needs a
decision.

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

## Stage 3 — Review and save to Notion

Check the summary and notes for accuracy against the source. Use web search to
verify any claims that are time-sensitive or version-specific. List any
discrepancies found. Produce a corrected version of the document. Save it to
Notion as a new page: article title, the corrected content, and a "Reviewer
notes" section listing what was checked and what changed.

## Stage 4 — Polish

Condense the corrected document into a concise version ready to hand-copy onto
paper: no `[video]` tags, no reviewer notes, maximally terse.

## Output

End with two artifacts: the Notion page (link it) and the paper-ready text
(shown in chat).
