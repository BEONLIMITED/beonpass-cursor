# BEON PASS for Cursor

**BEON PASS** is one access wallet for people and AI, developed by **BEON LIMITED**. This public repository connects Cursor to the remote MCP server at `https://beonpass.com/mcp`.

## What you can do

- Use supported GitHub, Supabase, Cloudflare, Vercel, Railway, and other provider operations through your BEON PASS wallet.
- Select among multiple accounts for a provider and work within a personal or organization wallet.
- Inspect permitted repositories, projects, deployments, and other resources; make changes within the access you have authorized.
- Manage supported access requests, temporary access, and Autopilot grants.
- Review activity and distinguish completed, denied, failed, and pending operations.

Tools are supplied by the hosted server, not bundled in this repository. Availability depends on the integration, connected accounts, provider permissions, selected AI access, organization rules, and plan. Updating this repository does not grant additional account access.

## Connect in Cursor

This repository is available directly; it does not claim a published Cursor Marketplace listing.

Add the following remote server to your Cursor MCP configuration, or use the included `mcp.json`:

```json
{
  "mcpServers": {
    "beonpass": {
      "url": "https://beonpass.com/mcp"
    }
  }
}
```

Complete BEON PASS OAuth sign-in when Cursor prompts you. In your BEON PASS wallet, connect the provider accounts you want to use and review the access authorized for Cursor. Start with a read-only request and verify the intended wallet, account, and resource.

The repository also includes a Cursor plugin manifest and a BEON PASS skill. Keep the repository structure intact when installing it as a local plugin using your Cursor version's supported plugin workflow.

No provider API keys or passwords belong in the MCP configuration or chat. Enter private values only in BEON PASS's secure input flow. If Cursor still shows an older tool catalog after a server update, use its available MCP reload/reconnect controls and check the resulting catalog before requesting a new action.

## Example prompts

- “Using BEON PASS, show my connected providers and active wallet.”
- “Which of my GitHub accounts can access this repository?”
- “Inspect my selected Vercel project's deployment status without changing anything.”
- “Show the access I have in this organization.”
- “Show pending access requests for my organization.”

## Access and confirmations

BEON PASS checks both the person's and AI client's effective access. Organization roles, resource restrictions, expiry, and provider scopes continue to apply. A default account is not a substitute for resolving ambiguity between multiple accounts.

Cursor controls its own action confirmations. BEON PASS enforces authorization and may require a separate access decision or secure private input. Autopilot provides standing authorization within its configured limits; it does not disable Cursor's confirmation rules.

Public integrations and custom connections have distinct authorization boundaries. The public integration does not automatically gain arbitrary private tool schemas after sign-in. Private custom-connection functionality is not promised by this package.

## Current release limits

The October 14, 2026 production release includes limited app/Preview checkpoint functionality. Availability must be checked in the connected client's actual tool catalog. This is not general application, database, Auth, or Storage recovery, and does not promise arbitrary code builds.

At the production release receipt, private custom-connection activation remained disabled and Stripe provider access was restricted to designated reviewers. Neither is advertised here as generally available. Existing subscription billing is separate from Stripe provider access.

## Pricing

The repository is free to use. BEON PASS has free and paid service plans; see [beonpass.com](https://beonpass.com) for current capabilities and limits.

## Security, support, and license

Never put provider credentials, passwords, API keys, or tokens in chat prompts or source files. If an action is denied, resolve the missing permission through the supported flow; do not switch accounts or endpoints to bypass it.

- [Documentation](https://beonpass.com/docs)
- [Privacy policy](https://beonpass.com/privacy)
- [Terms of service](https://beonpass.com/terms)
- [Support](https://beonpass.com/support)

Developed by **BEON LIMITED**. The integration files are licensed under the [MIT License](LICENSE). The hosted BEON PASS backend and third-party APIs are separate services governed by their respective terms.
