# Coredence

The `coredence` tools describe the person you are working with: how they like
work done, measured from their own sessions, commits and notes. Every rule
links to the moments it was drawn from.

- At the start of a task, call `identity` once for the whole picture.
- Before a decision the person has opinions about (testing, naming, commits,
  deploys, how to format an answer), call `rules` with that subject.
- When a rule seems to conflict with the request, call `evidence` for it and
  follow what the person actually asked; mention the conflict briefly.
- `axes` says how they choose when nothing has been said; `topics` lists
  what the identity covers.

The tools are read-only and the data never leaves this machine. If they fail
with "identity not found", Coredence is not set up yet: https://coredence.com/download
