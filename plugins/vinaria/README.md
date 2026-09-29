# Vinaria

Vinaria aide les clients invités à trouver des sociétés, à qualifier des prospects et à conserver les résultats dans leur propre espace. Le plugin fournit une méthode commune, sans imposer de CRM, de tableur ou de source nationale. Il ne contacte personne et n'envoie aucun message.

## Installer et connecter

- **Cowork** : ouvrir Personnaliser → Plugins → Ajouter une marketplace, ajouter la source de ce dépôt, puis installer Vinaria.
- **Claude Code** : ajouter la marketplace de ce dépôt avec la commande `/plugin marketplace add`, puis installer `vinaria` depuis cette marketplace.
- **Codex** : ajouter la marketplace de ce dépôt avec `codex plugin marketplace add`, puis installer Vinaria depuis le catalogue.

Après l'installation, connecter le serveur Vinaria avec son compte invité : dans l'onglet Connecteurs du plugin pour Claude, ou via la connexion MCP dans Codex. L'authentification est assurée par le serveur OAuth. Ne saisir aucun secret dans la conversation.

Pour commencer, ouvrir le dossier où conserver son contexte et demander : « configure mon espace ». Le skill prépare `entreprise.md`, `catalogue.md` et `fonctionnement.md` après validation. Un fichier `prospects.csv` n'est créé que si aucun autre registre n'est utilisé.

Les recherches envoient des requêtes au serveur `https://app.vinaria.io/mcp`. Le plugin ne stocke rien d'autre : les fichiers de contexte et le registre restent dans l'espace choisi par le client.

Les mises à jour du plugin viennent de sa source. Dans Claude, utiliser « Vérifier les mises à jour » ou la synchronisation automatique. Dans Claude Code, utiliser `claude plugin update vinaria` ou la mise à jour automatique si elle est activée pour ce catalogue. Dans Codex, mettre à jour depuis le catalogue, puis ouvrir une nouvelle session. Une mise à jour ne modifie jamais les fichiers du client.
