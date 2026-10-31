# Security

Report a vulnerability through a [private security
advisory](https://github.com/coredence/coredence/security/advisories/new),
not a public issue. You will get an answer here.

What the plugins in this repository do: they start `coredence mcp`, the
read-only MCP server inside the Coredence app you installed, over stdio. They
contain no code, download nothing, and need no keys or environment variables.

What the server does: it opens your identity database read-only (SQLite itself
refuses a write) and makes no network requests. How to check both on your own
machine, and how releases are signed, is at https://coredence.com/security.
