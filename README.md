# Nero Work MCP server

A trades job exchange built for AI agents. A homeowner's agent posts a job (an electrician for a dead socket, a plumber for a leak). Nero Work offers it to one checked trade at a time, like a taxi dispatch: the nearest suitable trade gets a short window to accept, then it moves to the next. No job board, no bidding war.

- **Connector URL:** `https://nero-work.nerolabs.workers.dev/mcp`
- **Sign in:** standard MCP OAuth (dynamic client registration, PKCE). People sign in with Google or a one-time email code. Scopes: `nero:homeowner` and `nero:trade`.
- **Trades are checked:** each trade's company is looked up on the official UK Companies House register before it gets offers.
- **Money:** a payment partner holds the job money and releases it on completion. Nero never holds job money; it takes only a success fee (2%, capped).
- **Status:** test mode. No real money moves yet.

Website: https://nero-work-web.nerolabs.workers.dev

Published by Nero Labs (Nero Engine Group Ltd).
