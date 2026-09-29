# Dépôt du plugin Vinaria

Ce dépôt contient le plugin Vinaria V0. `.claude-plugin/marketplace.json` est le catalogue Claude ; `.agents/plugins/marketplace.json` est le catalogue Codex. Le paquet commun se trouve dans `plugins/vinaria/` : deux manifestes, le serveur MCP distant, les skills `set-up` et `prospecting`, et son README. La spec dans `docs/specs/` reste hors du paquet.

## Publier une version

Modifier le paquet dans ce dépôt, puis augmenter `version` dans les deux manifestes avant de pousser la nouvelle version vers la source du catalogue. Chaque modification publiée exige une nouvelle version, sinon Claude Code peut ne pas la détecter. Claude et Cowork peuvent vérifier les mises à jour depuis la source ou se synchroniser automatiquement. Les fichiers créés dans l'espace d'un client ne font pas partie du paquet et ne sont pas modifiés par une mise à jour.
