# Coredence

**See what your work says about you.**

Coredence reads what you have already written, distils it into rules about how
you actually work, and keeps every one of them pointed at the evidence it came
from. The result lives in a single file on your own machine.

→ **[coredence.com](https://coredence.com)**

---

## What this repository is

Releases, documentation and the issue tracker. **Not the source.**

The engine that reads your work is not published. The reason, and what you get
instead, is written out on [coredence.com/license](https://coredence.com/license) —
but the short version is that the claims worth checking are checkable without
it, and more conclusively:

```sh
lsof -i -a -p $(pgrep -x Coredence)    # prints nothing: there are no connections
sqlite3 ~/.karaca/brain.db '.tables'   # your whole identity, in a tool we did not write
```

Source code tells you what should happen. Those tell you what is happening.

## Status

Not released yet. Builds are signed with a Developer ID and notarised by Apple,
but none are public.

**Watch this repository** (Watch → Custom → Releases) and GitHub will tell you
when the first one lands. There is no mailing list, because there is no account
and nothing to put you in one.

## Getting it, when it lands

One download. The engine ships inside the app — nothing to clone, no Python to
install, no command to run. Open it and it asks which sources it may read.

A Windows version is planned. An identity is one file and moves between
machines with you.

## Documentation

- [Getting started](https://coredence.com/docs) — what it reads, what the five
  layers mean, what to do with a rule you disagree with
- [Privacy](https://coredence.com/privacy) — what is collected (nothing) and
  how to verify that rather than believe it
- [Security](https://coredence.com/security) — signing, notarisation, and how
  to check a build before you open it
- [Roadmap](https://coredence.com/roadmap) — what is next, and what has been
  decided against

## Issues and questions

Both belong here. Nothing is triaged in private, and there is no support
address that goes somewhere different from where the work is.

For anything that should not be public, open a
[private security advisory](../../security/advisories/new) instead.

---

Made by Akaya Labs.
