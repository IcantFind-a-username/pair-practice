# Pair Programming Notes

Scratch space for testing the co-authored commit workflow.

## Co-authored commits

Git supports attributing a single commit to more than one person via a
`Co-Authored-By:` trailer in the commit message:

```
docs: add pair programming notes

Co-Authored-By: Name <email@example.com>
```

Rules that matter:

- The trailer goes at the end of the message, after a blank line.
- The email must belong to a verified GitHub account, or be that
  account's `ID+username@users.noreply.github.com` address.
- One trailer line per co-author; several may be listed.
- Squash merges rewrite the commit message, which can drop the trailer.
  Prefer a merge commit or a rebase when the attribution matters.
