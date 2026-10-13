# Installing the Coredence MCP server

Coredence is a desktop app; the MCP server ships inside it. There is nothing
to clone, build or install with npm or pip.

1. Ask the user to install Coredence from https://coredence.com/download
   (macOS 14+ on Apple silicon, or Windows 10+) and open it once. Opening it
   once sets up their identity and makes the `coredence` command available.
2. Check that the command exists: `coredence --help` should print usage.
   If it does not, the app has not been opened yet, or (on macOS) the user's
   shell does not have `~/.local/bin` on its PATH.
3. Add this server to the MCP settings:

```json
{
  "mcpServers": {
    "coredence": {
      "command": "coredence",
      "args": ["mcp"]
    }
  }
}
```

No API key or environment variable is needed. The server is read-only and
local: it answers from the identity database on this machine and opens no
network connections.

Tools: `identity` (the whole picture), `rules` (search by subject), `evidence`
(the moments behind a rule), `axes` (how they choose when nothing was said),
`topics` (what the identity covers).
