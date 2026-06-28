# Free Signal Over Noise Radar

Use this before joining a crowded bounty, agent-PR, or paid issue thread.

The goal is not to be the next loud contributor. The goal is to decide whether the maintainer needs a clean implementation, an evidence cleanup, or silence.

## Three Possible Moves

| Thread signal | Better move |
| --- | --- |
| Low claim count, clear reward, no maintainer stop signal | Inspect overlap, then make a small implementation claim only if you can start now |
| Many claims, stale PRs, unclear validation, real payment/review pressure | Offer a queue map or evidence receipt instead of another overlapping PR |
| Maintainer says new PRs will not be accepted, thread is hostile, reward route is unclear, or issue is generated alert noise | Stay silent and spend effort elsewhere |

## Quick Manual Check

Before posting, answer these in writing:

- What exact issue, PR, or thread are we acting on?
- Is there an explicit reward, maintainer request, or review route?
- How many people have already claimed, submitted, or said they are working on it?
- Has a maintainer asked people to stop, wait, consolidate, or avoid new PRs?
- Would another public comment reduce maintainer work, or just prove we saw the thread?

## Safe Public Offer Shape

```md
I am not going to add another overlapping implementation here. The useful cleanup looks like a short queue map: group the open PRs by approach, flag obvious duplicates/stale items, and point to the ones with the clearest validation. If that would help, I can do that as a small cleanup pass.
```

No product link. No checkout link. No vague claim that you can solve everything.

## What The Paid Bundle Adds

The full bundle includes a no-dependency `signal-over-noise-radar.mjs` script that reads a GitHub issue or PR thread through the GitHub API and prints a recommended action gate: implementation strike, evidence cleanup, or hard no-go.