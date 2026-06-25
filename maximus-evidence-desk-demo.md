# Maximus Evidence Desk Demo

This is a sample of the receipt Maximus should produce before review, rerun, merge, or payment decisions.

It is intentionally plain. The goal is not to sound impressive. The goal is to save a maintainer from reconstructing the facts.

## Example Situation

A repository has a paid issue, several overlapping PRs, red CI on one submission, and a contributor asking whether their work is ready for review.

## Evidence Receipt

| Field | Receipt |
| --- | --- |
| Work item | Paid issue with multiple implementation attempts |
| Current state | Open, crowded, no final maintainer selection yet |
| Payment route | Explicit reward exists, but payout depends on maintainer acceptance |
| Submitted work | One PR is complete enough to evaluate; two later PRs overlap the same scope |
| CI state | One failure appears auth/secret-related; no code-actionable failure confirmed |
| Evidence present | Linked issue, focused implementation, passing local tests, concise validation notes |
| Evidence missing | Maintainer selection, reward confirmation, non-auth CI rerun if required |
| Overlap risk | High; do not post broad claims or imply ownership of the full issue |
| Safe public note | Short status only if it answers a maintainer request or clarifies validation |
| Smallest next action | Wait for maintainer selection unless a requested change, CI rerun, or payment instruction appears |

## Maintainer-Safe Comment Shape

```md
I checked the current state again. My PR is still limited to the scoped fix and the local validation listed in the description. I am not claiming the broader issue beyond that.

I will wait for maintainer direction unless you want a specific rerun, narrower patch, or comparison against the other open attempts.
```

## Why This Helps

- It does not pressure the maintainer.
- It does not market a product in the thread.
- It names what is known, unknown, and not being claimed.
- It keeps the next action smaller than another round of noisy comments.

## Full Workflow

The paid bundle includes the Maximus Evidence Desk Sprint workflow, Receipts Desk generator, Deposit Radar, Opire reward scanner, and the three component kits for PR intake, CI triage, and evidence packaging.

Full bundle:
https://buy.polar.sh/polar_cl_O4VAFwUcew1m5QSjAFdrrUhaKPGgrQWAa3Y3y0Nwwoi