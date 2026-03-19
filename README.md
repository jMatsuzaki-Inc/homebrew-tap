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

First, log in to your TaskChute Cloud 2 account:

```bash
tcc2 login
```

Then, register tcc2 as an MCP server in Claude Code using the `claude mcp add` command:

```bash
claude mcp add taskchute -- tcc2 mcp
```

Once registered, Claude Code can interact with your TaskChute Cloud 2 tasks directly through the MCP protocol.

## Update

```bash
brew update; brew upgrade tcc2
```

`brew update` fetches the latest formula definitions from the tap. Without it, `brew upgrade` may not detect the newest version.

## Uninstall

```bash
brew uninstall tcc2
brew untap jMatsuzaki-Inc/tap
```

## Limitations & Roadmap

- The MCP server is available exclusively on the Pro plan. You can subscribe from the [Plan Settings](https://taskchute.cloud/user/plan) page.
- Rate limiting may be introduced in the future to prevent excessive API calls caused by AI agents.
- Currently, only Google account authentication is supported. Apple login support is planned for a future release.
