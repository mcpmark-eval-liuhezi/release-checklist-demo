# release-checklist-demo

A small, live example of our release flow — built for onboarding, not for a slide deck.

New teammate: walk the history of this repository top to bottom and you will see one full
release lifecycle:

1. **Branch** — `add-pre-merge-checklist-and-ci` is cut from `main`.
2. **Pull request** — the changes are proposed in [PR #2](https://github.com/mcpmark-eval-liuhezi/release-checklist-demo/pull/2), reviewed, then merged.
3. **Merge** — the branch's work lands on the default branch via a merge commit, never as a direct commit to `main`.
4. **CI** — GitHub Actions reacts: it runs on the pull request itself and again on the push to `main` after the merge.

## What's in here

| File | Purpose |
| --- | --- |
| `README.md` | This guide. |
| `RELEASE_CHECKLIST.md` | The short pre-merge checklist every change must pass. |
| `.github/workflows/ci.yml` | Minimal CI: triggers on pushes and pull requests, echoes one line. |

## Suggested walkthrough

1. Open **Insights → Network** (or `git log --graph --oneline --all`) and find the branch, its commits, and the merge.
2. Open **Pull requests → Closed** and look at PR #2: its diff, the branch it came from, and its final merged state.
3. Open the **Actions** tab and find the runs for both the pull request and the post-merge push.
4. Read `RELEASE_CHECKLIST.md` — that's the bar every change has to clear before merging.
