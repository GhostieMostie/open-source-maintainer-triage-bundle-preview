# Free Maintainer Triage Router

Use this when a pull request or issue is noisy and you need to decide what to ask for next.

## Step 1: What Is Blocking Review?

- [ ] Missing linked issue or accepted goal.
- [ ] Missing reproduction or before/after behavior.
- [ ] Missing validation commands.
- [ ] CI failed but the failure class is unclear.
- [ ] The change appears generated or low-context and human validation is unclear.
- [ ] Bounty/payment language appears before evidence is ready.
- [ ] Scope is too broad for a focused review.

## Step 2: Route It

| Main blocker | Route |
| --- | --- |
| Contribution evidence is missing | Agent PR Gatekeeper |
| CI failure needs classification | Flaky CI War Room Kit |
| Review/payment handoff needs packaging | Open-Source Maintainer CI and QA Kit |

## Step 3: Safe Public Comment Shape

```md
Thanks for the PR. Before deeper review, please add:

- linked issue or accepted goal
- reproduction or before/after notes
- validation commands and results
- current CI status and failure classification, if red
- scope/risk notes
- human-validation note for generated or tool-assisted changes

Once those are present, maintainers can review behavior instead of reconstructing context.
```

## Step 4: Do Not Overreach

- Do not accuse the contributor of AI misuse.
- Do not ask for payment or reward action before evidence is present.
- Do not auto-close until maintainers agree on policy and false-positive tolerance.
