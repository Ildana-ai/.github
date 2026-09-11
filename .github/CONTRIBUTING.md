# Contributing

Thanks for looking at an Ildana project. These are small, local-first tools — no server, no
telemetry, no account beyond what the underlying app already requires. Contributions that keep
that shape are welcome.

## Before you open a PR

- For anything beyond a small fix, open an issue first. It saves everyone a rewritten PR.
- Keep the scope of a PR to one change. Unrelated formatting or refactor diffs make review slower
  and get pushed back.
- New dependencies need a reason in the PR description — why the standard library isn't enough.
- No new network calls, install scripts, or credential handling without a clear explanation of
  what they do and why.
- No bulk or machine-generated changes — a sweep that touches every file for a cosmetic reason is
  hard to review and easy to miss a real change inside. Split it, or open an issue first and ask.

## What happens after you open a PR

Every PR is reviewed as follows before it merges:

1. The full diff is read, including anything outside the obvious change — new dependencies,
   network or install code, anything touching credentials.
2. The test suite runs against your branch, on every platform and runtime the project supports
   (see the CI workflow for the exact matrix).
3. A maintainer approves the merge.

This applies to every contribution, regardless of who's submitting it. It's not personal — it's
the same bar every change goes through. Expect a few days, not a few hours; these are side
projects, not staffed products.

## Tests

CI runs on push and pull request across the supported OS/runtime matrix. A PR that doesn't pass CI
won't be merged. If you're adding a feature, add or update the tests that cover it.

## License

By contributing, you agree your contribution is licensed under the project's MIT license.
