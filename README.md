# Vinaria plugin repository

This repository holds the Vinaria plugin. `.claude-plugin/marketplace.json` is the Claude catalog; `.agents/plugins/marketplace.json` is the Codex catalog. The package lives in `plugins/vinaria/`: two manifests, the remote MCP server, the `set-up` and `prospecting` skills, and its README. The spec in `docs/specs/` is not part of the package.

## Publish a version

Change the package, then bump `version` in both manifests before pushing. Every published change needs a new version, otherwise Claude Code may not detect it. Claude and Cowork can check for updates from the source or sync automatically. Files created in a subscriber's folder are not part of the package and are never changed by an update.
