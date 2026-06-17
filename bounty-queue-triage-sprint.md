# Bounty Queue Triage Sprint

For maintainers or bounty hosts with one issue and too many claim PRs.

This is not another implementation attempt. It is a short review-load reduction pass: group the current claims, show where they overlap, and point reviewers toward the smallest credible merge path.

## When This Helps

- One bounty issue has several `/attempt`, `/try`, `/claim`, or reward PRs.
- Contributors are solving adjacent slices and the thread is hard to scan.
- Reviewers need to know which PRs are duplicates, residual fixes, or likely out of scope.
- The maintainer does not want another public comment that adds pressure without reducing work.

## What A Sprint Produces

For one issue:

- claim PRs grouped by behavior area
- likely duplicate or overlapping fixes
- strongest validation evidence per group
- stale or out-of-scope claims
- one suggested merge / close / defer reading order
- remaining unclaimed gap, if one is visible

Maintainers still decide. The point is to make the queue easier to review, not to replace maintainer judgment.

## Sample Shape

```md
## Queue Read

Issue: owner/repo#123
Reward: visible bounty label / platform route
Current state: open, 18 comments, 9 claim PRs

### Bucket 1: Core Fix

- #201: covers the main failing path, includes focused test and build proof
- #204: similar path, weaker validation, likely duplicate of #201

Suggested read: review #201 before #204.

### Bucket 2: Startup / Config

- #206: separate config edge, may be mergeable after core fix
- #209: touches same files but solves a helper-script issue, probably secondary

Suggested read: defer until core fix is chosen.

### Remaining Gap

No clear unclaimed implementation gap. The useful next action is maintainer review, not another PR.
```

## Lightweight Scope

- `Queue map`: one issue, current claim PRs, overlap buckets, suggested review order.
- `Queue map + validation notes`: adds PR-by-PR evidence checks and a short maintainer handoff.

Typical range: `$75-$150`, depending on queue size and whether validation notes are included.

## Responsible Use

- Do not use this to campaign against other contributors.
- Do not present it as an official maintainer decision.
- Do not post a sales link in a bounty thread unless a maintainer asks for outside help or resources.
- If the queue is not crowded, write code or stay quiet.
