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
#### Branches de correction
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