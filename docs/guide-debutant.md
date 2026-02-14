# Guide débutant – état actuel de la base de code

## 1) Structure générale du dépôt

Aujourd’hui, ce dépôt est **minimal** :

- `.git/` : métadonnées Git (historique, branches, etc.).
- `.gitkeep` : fichier vide utilisé pour garder un dépôt (ou un dossier) versionné, même sans code métier.

Il n’y a pas encore :

- de code applicatif (`src/`, `app/`, `backend/`, etc.),
- de dépendances (`package.json`, `pyproject.toml`, `Cargo.toml`, etc.),
- de tests,
- de documentation technique structurée.

## 2) Ce qu’il faut savoir en priorité

Si tu débutes, retiens surtout ceci :

1. **Le projet est au stade d’amorçage** : il faut d’abord définir la stack et l’architecture.
2. **Le repère principal est Git** : comme il n’y a pas encore de code, la discipline de commits et de conventions est le premier “socle”.
3. **Le prochain livrable utile** est un squelette clair (ex. arborescence + README + scripts de lancement/test).

## 3) Points de repère pour la suite de l’apprentissage

### A. Construire un socle lisible

Commencer par créer :

- un `README.md` avec but du projet, prérequis et commandes de base,
- une arborescence explicite (par exemple `src/`, `tests/`, `docs/`),
- un fichier de configuration dépendant de la techno choisie.

### B. Mettre en place le cycle de travail

- Définir une convention de commits (atomiques, messages explicites).
- Ajouter une commande de tests (même un test trivial au début).
- Préparer une CI simple (lint + test).

### C. Apprendre par incréments

Pour un néophyte, un bon ordre d’apprentissage :

1. Comprendre Git (status, add, commit, branch).
2. Savoir lancer le projet localement.
3. Lire l’entrée principale de l’application (fichier `main` / routeur / serveur selon stack).
4. Suivre un flux complet “entrée → logique → sortie”.
5. Écrire puis exécuter un test simple.

## 4) En résumé

La base actuelle est volontairement vide côté code métier. C’est une bonne opportunité pour poser des fondations propres avant de développer : structure, conventions, documentation et boucle de test.

## 5) Exemple de `index.html` avec logo "Agent AI"

Un fichier `index.html` a été ajouté dans `docs/` pour afficher un logo simple "Agent AI".
Tu peux l’ouvrir dans un navigateur pour voir le rendu.
