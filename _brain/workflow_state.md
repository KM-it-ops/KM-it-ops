# Workflow State

## Goal
Inspect recent commits for concrete critical correctness bugs. Fix only if a high-confidence critical bug is found.

## Plan
- [x] Read required brain files; create them when absent.
- [x] Fetch `origin/main` and compare the working branch.
- [x] Inspect recent commit content and repository surface area.
- [x] Decide whether any critical bug has a concrete trigger scenario.
- [x] If a bug exists, implement a minimal fix, add validation, commit, push, and open a PR.
- [x] If no critical bug exists, post a concise Slack summary without opening a PR.

## Outcome
No critical bug found. `origin/main...HEAD` has no tracked diff, and `HEAD` contains only a README-only profile repository commit.
