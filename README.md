# Mes skills ChatGPT et Codex

Ce dépôt privé conserve mes skills et l’historique de leurs modifications.
Ils sont regroupés dans un plugin nommé `mes-skills`.

## Organisation

- `.agents/plugins/marketplace.json` : catalogue des plugins.
- `plugins/mes-skills/.codex-plugin/plugin.json` : description et version du plugin.
- `plugins/mes-skills/skills/` : dossiers des skills.

## Skills disponibles

| Nom | Description |
|---|---|
| exemple-skill | Reformuler un court texte en langage clair. |

## Ajouter un skill depuis GitHub

1. À la racine du dépôt, choisir « Add file → Create new file ».
2. Saisir le chemin `plugins/mes-skills/skills/nom-du-skill/SKILL.md`.
3. Ajouter les champs `name` et `description` entre deux lignes `---`,
   puis les instructions du skill.
4. Utiliser le même nom pour le dossier et le champ `name`,
   en minuscules et avec des tirets.
5. Enregistrer avec « Commit changes ».
6. Ajouter le skill au tableau de ce README.
7. Augmenter la version dans
   `plugins/mes-skills/.codex-plugin/plugin.json`.

Si le skill utilise des scripts, références ou modèles,
ajouter également ces ressources dans son dossier.

## Modifier un skill

1. Ouvrir son fichier sur GitHub.
2. Cliquer sur le crayon.
3. Modifier le contenu.
4. Enregistrer avec un message décrivant la modification.
5. Augmenter la version du plugin.

## Consulter les anciennes versions

Ouvrir un fichier puis cliquer sur « History » pour consulter
ses modifications et ses versions précédentes.

## Installer et synchroniser

La présence des fichiers sur GitHub ne suffit pas à installer
le plugin dans ChatGPT ou Codex.

L’import d’une marketplace GitHub dans un espace ChatGPT
nécessite les fonctions d’administration correspondantes.
La méthode de connexion sera précisée après vérification
des options disponibles sur mon compte.

Les modifications réalisées dans ChatGPT ne sont pas
automatiquement reportées dans ce dépôt.
