# Keeping this README current

This repo's `README.md` renders as the profile page at github.com/tahovig, so
it's worth keeping deliberately accurate rather than growing stale or
aspirational. Process:

## When to add a project

Add a row to the portfolio/skills tables only once a repo is demo-ready:
it has its own README, working code, and (where applicable) passing tests —
not just at the moment the repo is created. An empty or barely-started repo
doesn't belong here yet.

## When to prune

If a project is renamed, abandoned, or superseded by a later one, update or
remove its row rather than leaving a stale or broken link.

## Review trigger

Treat a new or meaningfully updated description on a `poc-*` (or similar
portfolio) repo as the signal to revisit this README. Two things watch for
that automatically:
- The link-check workflow (`.github/workflows/link-check.yml`) catches
  broken/dead links on every push.
- A scheduled weekly check diffs the account's repo list against what's
  listed here and flags drift for manual review — it does not auto-edit
  the README.

## Local workflow

```bash
git pull
# edit README.md
git add README.md
git commit -m "..."
git push
```

Solo repo, no branches/PRs needed for routine edits.
