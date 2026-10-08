# BEON PASS for Cursor

**BEON PASS** is one access wallet for people and AI, developed by **BEON LIMITED**. This open-source Cursor plugin connects Cursor to the existing BEON PASS remote MCP server, allowing authorized access to connected developer and cloud tools.

## What it does

- Connect to the BEON PASS wallet using the remote MCP endpoint.
- Work with connected providers such as GitHub, Supabase, Cloudflare, Vercel, Railway, and other providers supported by your account.
- Select between personal and organization contexts and multiple provider accounts where available.
- Respect BEON PASS access controls, resource restrictions, approvals, temporary access, and Autopilot grants.

The provider tools available depend on the connected accounts and their authorization. This plugin does not include or publish the BEON PASS backend.

## Install and connect

1. Install the plugin from Cursor Marketplace, or test locally by copying this repository into `~/.cursor/plugins/local/beonpass` and running **Developer: Reload Window**.
2. Open Cursor's plugin/MCP settings and connect the `beonpass` server.
3. Complete the BEON PASS OAuth sign-in in your browser when prompted.
4. Connect provider accounts at [beonpass.com](https://beonpass.com) and grant the desired access.
5. Ask Cursor to list your connected accounts or inspect an authorized resource.

The MCP endpoint is `https://beonpass.com/mcp`. No API keys or credentials are bundled in this repository.

## Example prompts

- “Using BEON PASS, list my connected providers and tell me which account is active.”
- “Using BEON PASS, list my GitHub repositories and Supabase projects that I can access.”
- “Using BEON PASS, inspect this project's deployment status without changing anything.”
- “Using BEON PASS, show access requests for my organization.”

## Pricing and marketplace policy

The **Cursor plugin package is free** to install. BEON PASS offers a free service tier and optional paid subscriptions for features beyond that tier. **Marketplace eligibility for optional paid service features must be confirmed with Cursor**, whose publisher terms prohibit direct or indirect fees for access to or use of marketplace plugins. Do not submit this repository as a compliant paid-service integration until Cursor clarifies that policy in writing.

## Security and privacy

The MCP server requires authentication. Access to third-party resources is governed by the connected providers and BEON PASS policies. Never paste credentials into Cursor prompts or commit them to this repository.

- [Documentation](https://beonpass.com/docs)
- [Privacy policy](https://beonpass.com/privacy)
- [Terms of service](https://beonpass.com/terms)
- [Support](https://beonpass.com/support)

## Publisher

BEON LIMITED — [beonpass.com](https://beonpass.com)

## License

The integration package in this repository is available under the MIT License. BEON PASS's hosted service and third-party provider APIs are not part of this repository and are governed by their respective terms.
