# BEON PASS for Cursor

**BEON PASS** is one access wallet for people and AI, developed by **BEON LIMITED**. This open-source Cursor plugin connects Cursor to the BEON PASS remote MCP server at `https://beonpass.com/mcp`, providing authorized access to connected developer and cloud services.

## Features

- Connect GitHub, Supabase, Cloudflare, Vercel, Railway, and other supported provider accounts through BEON PASS.
- Work with multiple accounts per provider and personal or organization wallets.
- Respect resource-level permissions, access requests, approvals, temporary access, and Autopilot authorization.
- Perform read and write operations only when allowed by the provider and BEON PASS access controls.
- Keep provider credentials in the BEON PASS authorization system rather than in this repository.

Available tools and permissions depend on each user's connected accounts, provider authorizations, and BEON PASS plan.

## Install and connect

1. Install BEON PASS from Cursor Marketplace after publication. For local testing, place this repository under `~/.cursor/plugins/local/beonpass` and run **Developer: Reload Window**.
2. In Cursor's plugin/MCP settings, connect the `beonpass` remote MCP server.
3. Complete the browser-based BEON PASS OAuth authorization when prompted.
4. At [beonpass.com](https://beonpass.com), connect your chosen provider accounts and configure access.
5. Ask Cursor to inspect a permitted resource. Confirm the correct wallet and provider account before making changes.

No API tokens or credentials are bundled with the plugin. The MCP server requires user authentication.

## Example prompts

- “Using BEON PASS, show my connected providers and active wallet.”
- “Using BEON PASS, list the GitHub repositories I can access.”
- “Using BEON PASS, inspect the status of my Vercel deployments without making changes.”
- “Using BEON PASS, show pending access requests for my organization.”

## Pricing

The **Cursor plugin is free to install**. BEON PASS offers a permanent free service tier for up to three active personal provider connections. Optional Pro and Team subscriptions offer additional BEON PASS service capabilities. Pricing and plan limitations are described on [beonpass.com](https://beonpass.com).

## Security and privacy

BEON PASS enforces authorization and resource restrictions independently of this Cursor plugin. High-impact actions may require confirmation or approval. Do not put provider credentials, passwords, API keys, or tokens into chat prompts or source files.

- [Documentation](https://beonpass.com/docs)
- [Privacy policy](https://beonpass.com/privacy)
- [Terms of service](https://beonpass.com/terms)
- [Support](https://beonpass.com/support)

## Publisher and license

Developed by **BEON LIMITED** — [beonpass.com](https://beonpass.com).

The integration files in this repository are licensed under the [MIT License](LICENSE). The BEON PASS hosted backend and connected third-party APIs are separate services governed by their respective terms.
