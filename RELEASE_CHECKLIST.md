# Pre-merge Release Checklist

Run through every item below **before** merging a pull request. If any box cannot be checked,
the merge waits.

- [ ] All CI checks on the pull request are green.
- [ ] The diff has been reviewed by at least one teammate other than the author.
- [ ] The change works locally, not just in CI.
- [ ] No secrets, keys, or credentials appear anywhere in the diff.
- [ ] Documentation (README, CHANGELOG, in-code comments) is updated to match the change.

---

Once every box is checked, merge the pull request and confirm CI runs green again on `main`.
