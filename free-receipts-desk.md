# Free Maintainer Receipts Desk

Use this when a PR, failed CI run, bounty attempt, or review request needs one clean page before anyone asks for review, merge, rerun, or payment.

The point is not to sound polished. The point is to make the facts easy to check.

## Copy This Shape

```md
# Receipt: [short title]

Context:
- [PR, issue, bounty, or CI run]

What changed:
- [concrete change]
- [concrete change]

Evidence:
- [command, check, screenshot, log, reproduction, linked run, or artifact]
- [command, check, screenshot, log, reproduction, linked run, or artifact]

Open questions:
- [what still needs a maintainer, reviewer, or bounty host decision]

Not claimed:
- [payment, security, performance, compatibility, or scope boundary]

Next action:
- [smallest useful action]
```

## Example

```md
# Receipt: Classify fork-only preview failure

Context:
- PR #123 has passing local tests but a failed preview deploy.

What changed:
- Updated one browser fixture.
- No production code path changed.

Evidence:
- `npm test -- --runInBand` passed locally.
- Unit job passed on the fork.
- Preview deploy failed before app build because deployment secrets are not available to forks.

Open questions:
- Maintainer needs to decide whether to rerun preview from a trusted branch.

Not claimed:
- This does not prove the protected preview environment works.
- No payment or merge claim is being made from fork-only evidence.

Next action:
- Mark the preview failure as auth-only or rerun from a trusted branch.
```

## Keep It Human

- Use facts and commands instead of adjectives.
- Say what is still unknown.
- Separate evidence from claims.
- Keep it short enough to read in one screen.
- Do not link products in third-party threads unless someone explicitly asked for tools or templates.
