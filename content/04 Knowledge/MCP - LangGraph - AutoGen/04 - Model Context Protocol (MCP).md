# Model Context Protocol (MCP) in Sprout

## What It Is
- A protocol for injecting structured, relevant external context into LLM calls
- Not for agent-to-agent comms

## How Sprout Can Use MCP
- Each agent has a context provider (e.g. `git-logs`, `screen-time`, `daily-logs`)
- MCP server pulls context before passing to GPT
- Cleaner, modular GPT calls with structured injection

## Example (Historian)
1. Git context provider returns commit logs
2. VS Code provider returns session times
3. Obsidian provider returns tagged notes
4. All passed into GPT via MCP for summarization

## Tools
- GitHub's MCP server repo: github.com/github/github-mcp-server
- gRPC-based, allows modular plug-in architecture for context