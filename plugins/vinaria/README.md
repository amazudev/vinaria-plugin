# Vinaria

Vinaria helps its subscribers find companies, qualify prospects and keep the results in their own space. The plugin provides a shared method without imposing a CRM, a spreadsheet or a national data source. It never contacts anyone and never sends a message. It answers in the user's language.

## Install and connect

Repository: `https://github.com/amazudev/vinaria-plugin`

- **Cowork**: Customize → Plugins → Add marketplace, paste `amazudev/vinaria-plugin`, then install Vinaria.
- **Claude Code**: `/plugin marketplace add amazudev/vinaria-plugin`, then `/plugin install vinaria@vinaria`.
- **Codex**: `codex plugin marketplace add amazudev/vinaria-plugin`, then install Vinaria from the catalog.

After installing, connect the Vinaria server with your Vinaria account: the plugin's Connectors tab in Claude, or the MCP connection in Codex. Authentication goes through the server's OAuth. Never type a secret in the conversation. Without a connected Vinaria account, the plugin does not prospect.

## First use

Open the folder where you want to keep your context and run `/vinaria:set-up`, or simply ask to set up your space. It drafts `company.md`, `catalog.md` and `workflow.md` for your approval. A `prospects.csv` file is created only if you use no other register.

Then run `/vinaria:prospecting`, or simply ask, for example, "find wine shops in Rennes".

## Data

Searches send requests to `https://app.vinaria.io/mcp`. The plugin stores nothing else: your context files and register stay in the folder you chose.

## Updates

Updates come from this repository. In Claude, use "Check for updates" or automatic sync. In Claude Code, run `claude plugin update vinaria`, or rely on auto-update if enabled for this marketplace. In Codex, update from the catalog, then open a new session. An update never changes your files.
