# Introduction à Git : Commandes de Base

Ce guide vous présente les commandes de base de Git, un système de gestion de version décentralisé. Vous apprendrez comment initialiser un dépôt, suivre les modifications, et collaborer avec d'autres développeurs.

## Table des Matières

1. [Initialisation](#initialisation)
2. [Clonage d'un Dépôt](#clonage-dun-dépôt)
3. [Suivi des Modifications](#suivi-des-modifications)
4. [Enregistrement des Modifications](#enregistrement-des-modifications)
5. [Envoi des Modifications](#envoi-des-modifications)
6. [Récupération des Modifications](#récupération-des-modifications)
7. [Branches](#branches)
8. [Fusion de Branches](#fusion-de-branches)
9. [Historique des Commits](#historique-des-commits)
10. [Dépôts Distants](#dépôts-distants)
11. [Rébase](#rébase)
12. [Différences](#différences)

---

## Initialisation

### `git init`

Cette commande initialise un nouveau dépôt Git dans le répertoire courant.

```bash
git init
```

### Exemple

```bash
mkdir mon-projet
cd mon-projet
git init
```

## Clonage d'un Dépôt

### `git clone <url>`

Clone un dépôt existant à partir de l'URL fournie.

```bash
git clone https://github.com/utilisateur/mon-projet.git
```

### Exemple

```bash
git clone https://github.com/octocat/Hello-World.git
```

## Suivi des Modifications

### `git status`

Affiche l'état des fichiers dans le répertoire de travail et l'index.

```bash
git status
```

### Exemple

```bash
git status
```

### `git add <fichier>`

Ajoute des modifications dans l'index.

```bash
git add fichier.txt
```

### Exemple

```bash
git add .   # Ajoute tous les fichiers modifiés
```

## Enregistrement des Modifications

### `git commit -m "message"`

Enregistre les modifications ajoutées dans l'index avec un message de commit.

```bash
git commit -m "Ajout du fichier de configuration"
```

### Exemple

```bash
git commit -m "Initial commit"
```

## Envoi des Modifications

### `git push <remote> <branche>`

Envoie les commits locaux vers le dépôt distant.

```bash
git push origin main
```

### Exemple

```bash
git push origin main
```

## Récupération des Modifications

### `git pull <remote> <branche>`

Récupère les modifications du dépôt distant et fusionne les dans la branche courante.

```bash
git pull origin main
```

### Exemple

```bash
git pull origin main
```

## Branches

### `git branch`

Affiche la liste des branches locales.

```bash
git branch
```

### Exemple

```bash
git branch -a  # Affiche aussi les branches distantes
```

### `git checkout <branche>`

Change de branche.

```bash
git checkout develop
```

### Exemple

```bash
git checkout -b nouvelle-branche  # Crée et bascule sur une nouvelle branche
```

## Fusion de Branches

### `git merge <branche>`

Fusionne la branche spécifiée dans la branche courante.

```bash
git merge feature-branch
```

### Exemple

```bash
git merge develop
```

## Historique des Commits

### `git log`

Affiche l'historique des commits.

```bash
git log
```

### Exemple

```bash
git log --oneline  # Affiche un historique compact
```

## Dépôts Distants

### `git remote`

Affiche les dépôts distants configurés.

```bash
git remote
```

### Exemple

```bash
git remote -v  # Affiche les URL associées
```

### `git fetch <remote>`

Télécharge les objets et les références du dépôt distant sans fusionner les changements.

```bash
git fetch origin
```

### Exemple

```bash
git fetch origin
```

## Rébase

### `git rebase <branche>`

Rebase la branche courante sur la branche spécifiée.

```bash
git rebase main
```

### Exemple

```bash
git rebase develop
```

## Différences

### `git diff`

Affiche les différences entre les fichiers suivis et leur version dans l'index ou entre deux commits.

```bash
git diff
```

### Exemple

```bash
git diff HEAD~1 HEAD  # Affiche les différences entre le dernier commit et celui d'avant
```

---

Ce guide vous fournit les bases pour commencer à utiliser Git. Pour approfondir vos connaissances, consultez la documentation officielle de Git ou des tutoriels en ligne.


Jean Narivelo