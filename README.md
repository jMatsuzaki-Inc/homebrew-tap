# TaskChute Cloud 2 CLI Homebrew Tap

> **Note:** The MCP server requires a Pro plan.
> Upgrade your plan at the [Plan Settings](https://taskchute.cloud/user/plan) page.

[TaskChute Cloud 2](https://taskchute.cloud) CLI - MCP Server for AI agents.

## Install

```bash
brew tap jMatsuzaki-Inc/tap
brew install tcc2
```

## Usage

```bash
# Login (opens browser for authentication)
tcc2 login

# Check login status
tcc2 status

# Start MCP server (for Claude Code, Cursor, etc.)
tcc2 mcp

# Logout
tcc2 logout
```

## Setting Up with Claude Code

Register tcc2 as an MCP server in Claude Code using the `claude mcp add` command:

```bash
claude mcp add taskchute -- tcc2 mcp
```

Once registered, Claude Code can interact with your TaskChute Cloud 2 tasks directly through the MCP protocol.

## Update

```bash
brew upgrade tcc2
```

## Uninstall

```bash
brew uninstall tcc2
brew untap jMatsuzaki-Inc/tap
```
