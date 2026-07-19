# Security Questionnaire Reuse Kit — Synthetic Proof Sample

You have an active B2B deal and a 250-row security questionnaire due soon. You already have approved answers. The painful part is finding which answers are safe to reuse, keeping their source and review date visible, and refusing to invent the rest.

This repository lets you inspect a fixed, fully synthetic output before deciding whether the paid kit fits that job.

## Inspect the 250-row result

[Open the fixed synthetic CSV](./security-questionnaire-fixed-synthetic-output-v1.0.0.csv).

| Result state | Rows | What the output does |
| --- | ---: | --- |
| `MATCHED` | 80 | Carries a synthetic approved answer into the output with its source fields visible |
| `STALE` | 30 | Leaves the answer blank because its review date is stale |
| `AMBIGUOUS` | 40 | Leaves the answer blank because more than one candidate needs human review |
| `REVIEW_REQUIRED` | 100 | Leaves the answer blank because there is no approved reusable answer |

The point is not to auto-answer everything. It is to reuse approved ground truth where the match is deterministic and surface the rest as an explicit review queue.

## What this sample proves

- One fixed 250-row fixture produces 80 matched rows and 170 deliberately blank review rows.
- Matched rows keep their source, owner, review date, evidence, match type, and confidence fields visible.
- The output does not fill stale, ambiguous, or unsupported answers.
- The file is synthetic and safe to inspect publicly.

## What it does not prove

- It is not customer data, a customer result, an accuracy benchmark, compliance evidence, or a set of answers to submit.
- `MATCHED` does not mean a fact was revalidated or is ready for final submission.
- An authorized person remains responsible for factual review and final submission.
- The fictional sample values must never be used as real security answers.

## Is the paid kit a fit?

It is designed for a small B2B SaaS team that already has an approved answer library and repeatedly receives XLSX or CSV security questionnaires during active deals.

It is not a fit if you need answers invented from scratch, policy authoring, evidence collection, compliance certification, consulting, customization, file review, or individualized support.

The paid download is a fixed self-serve kit: a local browser tool, starter workbooks, synthetic fixtures, CSV/XLSX outputs, a standalone match manifest, a review queue, operating instructions, and a license. Questionnaire and answer-library contents stay in the browser session; the tool does not upload them to a vendor service.

## See the full proof or buy once

- [Inspect the full product proof and compatibility details](https://security-questionnaire-reuse-kit.miri-orot.chatgpt.site/?ref=github)
- [Buy the fixed kit for $99 one time](https://gum.co/u/odhhl6k9)

No subscription, setup call, consulting, customization, manual fulfillment, or individualized support is included.

## File integrity

The expected SHA-256 is recorded in [`SHA256SUMS`](./SHA256SUMS).
