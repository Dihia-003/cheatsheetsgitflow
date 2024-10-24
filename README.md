# Cheat Sheet Gitflow

## Introduction
Gitflow est un modèle de gestion de branches qui aide à organiser le développement de logiciels. Il utilise plusieurs types de branches pour faciliter le travail en équipe.

## Branches principales
- **`main`** : contient le code de production.
- **`develop`** : contient le code en cours de développement.

## Branches de fonctionnalités
- **`feature/*`** : pour le développement de nouvelles fonctionnalités.

### Commandes
```
git checkout develop
git checkout -b feature/nom_de_la_fonctionnalité.
```
#### Branches de fcorrection
- **`hotfix/*`** : pour corriger rapidement des bugs en production.
##### Commandes
```
git checkout develop
git checkout -b feature/nom_de_la_fonctionnalité.
```
###### Branches de release

- **`release/*`** : pour préparer une nouvelle version.

#### Commandes
```
git checkout develop
git checkout -b release/nom_de_la_version
```
##### Visualiser l’historique
```
git log --oneline --graph --decorate --all
```
###### Fusionner des branches
```
git checkout develop
git merge feature/nom_de_la_fonctionnalité
```
## 🛠️ **Commandes Git**

| **Commande**                 | **Description**                                  |
| ---------------------------- | ------------------------------------------------ |
| `git                         | Initialise un dépôt Git local                    |
| `git clone [url]`            | Clone un dépôt distant                           |
| `git status`                 | Affiche l'état des fichiers dans le répertoire   |
| `git add [file]`             | Ajoute un fichier à l'index                      |
| `git commit -m "message"`    | Commit les modifications avec un message         |
| `git pull`                   | Récupère et fusionne les modifications distantes |
| `git push`                   | Envoie les commits locaux au dépôt distant       |
| `git branch`                 | Liste les branches                               |
| `git checkout [branch-name]` | Change de branche                                |
| `git merge [branch-name]`    | Fusionne une branche dans l'actuelle             |
| `git log`                    | Affiche l'historique des commits                 |
| `git reset --hard [commit]`  | Réinitialise à un commit précédent               |

---