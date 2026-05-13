# Workflow State

## Goal
Inspect recent commits for concrete critical correctness bugs. Fix only if a high-confidence critical bug is found.

## Plan
- [x] Read required brain files; note they were absent on this branch and recover prior context from visible automation branch history.
- [x] Fetch `origin/main` and compare the working branch.
- [x] Inspect recent commit content and repository surface area.
- [x] Decide whether any critical bug has a concrete trigger scenario.
- [ ] If a bug exists, implement a minimal fix, add validation, commit, push, and open a PR.
- [ ] If no critical bug exists, post a concise Slack summary without opening a PR.

## Notes
- `HEAD` matches `origin/main`.
- The repository currently tracks only `README.md`.
- No application code, data paths, auth paths, or behavioral diff were present for a critical-bug fix.
