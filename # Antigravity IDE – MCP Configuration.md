# Antigravity IDE – MCP Configuration

**Configuration file (Windows):**

`%USERPROFILE%\.gemini\config\mcp_config.json`

## Complete configuration

```json
{
  "mcpServers": {
    "github": {
      "serverUrl": "https://api.githubcopilot.com/mcp/",
      "headers": {
        "Authorization": "Bearer YOUR_GITHUB_PERSONAL_ACCESS_TOKEN"
      }
    },
    "chrome-devtools": {
      "command": "npx",
      "args": [
        "-y",
        "chrome-devtools-mcp@latest"
      ]
    },
    "supabase": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote",
        "https://mcp.supabase.com/mcp"
      ]
    }
  }
}
```

## MCP servers

1. **GitHub MCP**
   - Connects your GitHub account.
   - Searches repositories and works with code.

2. **Chrome DevTools MCP**
   - Connects to Chrome.
   - Inspects websites, debugs and tests web applications.

3. **Supabase MCP**
   - Connects your Supabase account.
   - Works with database tables, schemas and backend functionality.

## How to check the connection

Open Antigravity → Manage MCP Servers.

Check that all three servers appear and their tools are loaded.

**Important:** Replace `YOUR_GITHUB_PERSONAL_ACCESS_TOKEN` with your own GitHub token. Never share your actual token with anyone.