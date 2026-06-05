# Free Bounty Board Safety Scan

A quick filter for paid GitHub issue boards before you post `/try`, open a PR, or spend contributor time.

## Red Flags

- Issue is closed but the bounty page still shows money.
- Repository is archived, missing, or not accepting PRs.
- Several open PRs already target the same issue.
- Maintainers have warned about spam, bot PRs, or AI-generated attempts.
- Reward is token-only, social-stake, amountless, or "glory-only."
- Your intended comment mainly says you are interested instead of adding useful context.

## Green Flags

- Issue is open and recently touched by maintainers.
- Reward amount and payment route are explicit.
- Solver count is low, or existing PRs have a clear, fixable flaw.
- Scope is small enough to validate before claiming.
- You can write the PR body in a plain human voice: scope, validation, risk.

## Safe First Move

If you are not ready to start work now, do not comment. If you are ready:

```md
/try

I checked the thread and open PRs. I am going to focus on [specific scope] and will stop if I find overlap.
```

Then open a focused PR with real validation. No product links, no generic checklist comments, no "AI agent ready to help" language.
