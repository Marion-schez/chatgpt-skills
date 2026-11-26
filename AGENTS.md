# Marketplace de skills ChatGPT : règles de modification

## Contexte

Ce dépôt regroupe des plugins et des skills destinés à ChatGPT.

Les personnes qui te parlent ne sont pas des développeurs : explique tout en langage simple, sans jargon git.

Ces instructions s'appliquent lorsque tu travailles sur ce dépôt.

**Règle d'or : ne sauvegarde et n'envoie jamais de changements sur GitHub sans avoir suivi le parcours ci-dessous, dans l'ordre. Si le numéro de version du skill modifié n'a pas changé, arrête-toi et signale-le.**

## Vérifier tes accès

Avant de commencer, vérifie que tu peux lire et modifier le dépôt et utiliser Git.

Si tu n'as pas les accès nécessaires :
- Explique simplement ce qui manque.
- Prépare les contenus que tu peux préparer.
- Guide-moi pas à pas pour les opérations à réaliser sur GitHub.
- Ne prétends jamais avoir synchronisé, modifié ou envoyé un fichier si tu ne l'as pas fait.
- Ne coche jamais une vérification que tu n'as pas réalisée.

## Le parcours obligatoire

À chaque modification d'un skill, suis ces étapes dans cet ordre :

1. **Synchroniser** : récupère la dernière version du dépôt avec `git pull` avant de modifier un fichier. Si des modifications locales sont déjà présentes, ne les écrase pas : signale-les et demande comment poursuivre.
2. **Modifier** : effectue uniquement les changements demandés dans le skill concerné, ainsi que les mises à jour de version et de changelog nécessaires.
3. **Incrémenter la version** du skill modifié selon les règles ci-dessous. Cette étape est obligatoire, même pour une simple virgule.
4. **Mettre à jour le changelog** : ajoute une entrée datée indiquant le skill, sa nouvelle version et le changement effectué.
5. **Vérifier** : recopie la checklist ci-dessous dans ta réponse et coche uniquement les vérifications réalisées.
6. **Résumer et demander mon accord** : explique en 3 à 5 lignes simples ce qui a changé et indique l'ancien et le nouveau numéro de version. Demande ensuite mon « ok » explicite et attends ma réponse.
7. **Sauvegarder et envoyer** : après mon accord, vérifie que toutes les cases sont cochées, puis crée un commit directement sur `main` avec un message clair et envoie-le sur GitHub avec `git push`.

Mon accord porte sur les changements présentés. Si tu modifies leur contenu après cet accord, présente le nouveau résultat et demande un nouvel accord avant de l'envoyer.

## La règle de version

**Où se trouve le numéro :**

[À COMPLÉTER : indique ici le chemin exact du fichier et le champ qui contient la version de chaque skill.]

**Où se trouve le changelog :**

[À COMPLÉTER : indique ici le chemin exact du changelog.]

Si ces emplacements ne sont pas renseignés, cherche-les dans le dépôt. Si tu ne peux pas les identifier avec certitude, demande-moi avant de modifier quoi que ce soit.

Ne suppose pas qu'un numéro de version de plugin correspond à celui d'un skill.

**Quand incrémenter la version :** toujours, dès qu'un fichier du skill change. Aucune exception.

**De combien :**

| Type de changement | Exemple | Niveau |
|---|---|---|
| Correction de faute ou reformulation sans changement de fonctionnement | 1.2.3 → 1.2.4 | patch |
| Nouvelle capacité, nouvelle section fonctionnelle ou ajout compatible avec l'usage existant | 1.2.3 → 1.3.0 | minor |
| Changement incompatible avec l'usage existant | 1.2.3 → 2.0.0 | major |

Si tu hésites entre deux niveaux, pose-moi la question avant de choisir.

Ne modifie jamais le numéro de version d'un skill que tu n'as pas touché.

## Checklist avant sauvegarde et envoi

Recopie cette checklist dans ta réponse.

Lors de la demande d'accord, laisse la dernière case décochée. Coche-la uniquement après avoir reçu mon « ok » explicite.

- [ ] J'ai récupéré la dernière version du dépôt avec `git pull` avant de commencer.
- [ ] La version du skill modifié a été incrémentée : ancienne → nouvelle.
- [ ] Le changelog contient une entrée datée pour ce changement.
- [ ] Le skill possède toujours un fichier `SKILL.md` avec un frontmatter YAML valide contenant `name` et `description`.
- [ ] Aucun fichier parasite n'est inclus : brouillons, fichiers temporaires ou `.DS_Store`.
- [ ] Les changements inclus concernent uniquement le skill demandé et les fichiers de suivi nécessaires.
- [ ] J'ai résumé les changements en langage simple et reçu un « ok » explicite pour les sauvegarder et les envoyer.

## Façon de communiquer

- Dis « sauvegarder et envoyer mes changements » plutôt que « commit » et « push ».
- Si le résultat d'une commande Git est difficile à comprendre, traduis-le en une phrase simple.
- En cas de doute sur ce que je veux modifier, demande avant d'agir.
- Si une étape est bloquée, indique clairement ce qui est fait et ce qui reste à faire.

## Ce que tu ne fais jamais

- Pas de `git push --force`, ni d'autre forme d'envoi forcé.
- Pas de suppression de fichiers, de skills ou d'historique sans mon accord explicite.
- Pas de sauvegarde et d'envoi si la checklist n'est pas entièrement cochée.
- Pas de modification de skills autres que celui dont on parle.
- Pas d'inclusion de changements déjà présents qui ne font pas partie de ma demande.
- Pas de contournement d'une protection de la branche `main`.

Si `git pull` ou `git push` échoue, arrête-toi, explique simplement le problème et attends mes instructions.

Si la branche `main` impose une autre procédure, explique-la et demande-moi comment poursuivre.

## Rappel final

**Version incrémentée ? Changelog à jour ? Vérifications terminées ? Accord reçu ?**

Si une réponse est non, ne sauvegarde et n'envoie pas les changements sur GitHub.
