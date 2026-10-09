# Spacefast

**Build and share your AI work.**

This is the official GitHub home of [Spacefast](https://spacefast.com), by [Automattic](https://automattic.com/).

Spacefast turns an idea into a website, dashboard, report, or small web tool you can share. Build it in a conversation with your AI assistant, or bring something you already made, and publish it. Then keep improving it through chat: change the content or design, share a preview, choose who can open it, connect your own domain, or restore an earlier version.

The fastest way to use Spacefast is from the AI tools you already use, through our **plugins** and **MCP server**.

---

## 🔌 Plugins — [`spacefast/plugins`](https://github.com/spacefast/plugins)

Official Spacefast plugins for AI coding assistants. Each plugin bundles focused skills and the MCP configuration its client needs.

| Client | Install |
| --- | --- |
| Claude Code | `claude plugin marketplace add spacefast/plugins`<br>`claude plugin install spacefast@spacefast` |
| Codex | `codex plugin marketplace add spacefast/plugins`<br>`codex plugin add spacefast@spacefast`<br>`codex mcp login spacefast` |
| Cursor | `npx -y plugins add spacefast/plugins -t cursor -y` |
| GitHub Copilot CLI | `copilot plugin install spacefast/plugins` |
| goose | See the [goose setup](https://github.com/spacefast/plugins#goose) |

Included skills:

| Skill | Use it to |
| --- | --- |
| [spacefast](https://github.com/spacefast/plugins/tree/main/skills/spacefast) | Publish your work |
| [build-website](https://github.com/spacefast/plugins/tree/main/skills/build-website) | Build a website |
| [edit-space](https://github.com/spacefast/plugins/tree/main/skills/edit-space) | Update your site |
| [share-space](https://github.com/spacefast/plugins/tree/main/skills/share-space) | Share with the right people |
| [custom-domain](https://github.com/spacefast/plugins/tree/main/skills/custom-domain) | Use your own domain |
| [fix-deployment](https://github.com/spacefast/plugins/tree/main/skills/fix-deployment) | Fix or restore a deployment |
| [setup](https://github.com/spacefast/plugins/tree/main/skills/setup) | Get started |

Then ask your agent: **“Publish this project with Spacefast.”**

---

## 🧩 MCP server — [`spacefast/mcp`](https://github.com/spacefast/mcp)

The hosted Spacefast MCP server works with any client that supports remote MCP servers and browser OAuth.

- **Endpoint:** `https://mcp.spacefast.com`
- **Transport:** Streamable HTTP
- **Auth:** OAuth sign-in with your Spacefast account — no API key needed
- **Registry:** [`io.github.spacefast/mcp`](https://registry.modelcontextprotocol.io/v0.1/servers/io.github.spacefast%2Fmcp/versions/latest) in the official MCP Registry

Add it to `.mcp.json` in your project:

```json
{
  "mcpServers": {
    "spacefast": {
      "type": "http",
      "url": "https://mcp.spacefast.com"
    }
  }
}
```

Or in Claude Code:

```sh
claude mcp add --transport http spacefast https://mcp.spacefast.com
```

With it, your agent can publish files, edit a Space's source, deploy changes, manage sharing and domains, and restore earlier versions. See the [MCP README](https://github.com/spacefast/mcp#readme) for VS Code, goose, and other clients.

---

## More from Spacefast

- [`cli`](https://github.com/spacefast/cli) — Spacefast CLI binaries and install docs
- [`docs`](https://github.com/spacefast/docs) — Spacefast documentation
- [`push-session`](https://github.com/spacefast/push-session) — Share local AI coding-agent sessions with one `npx` command
- [`wordpress`](https://github.com/spacefast/wordpress) — Publish WordPress sites and headless CMS changes to Spacefast
- [`frames`](https://github.com/spacefast/frames) — Secure Spacefast iframe sessions, browser library, and WordPress blocks
- [`examples`](https://github.com/spacefast/examples) — Example projects

## Links

- [spacefast.com](https://spacefast.com)
- [Documentation](https://spacefast.com/docs/)
- [Agent setup](https://spacefast.com/docs/setup/)
- [Support](https://automattic.com/contact/)
