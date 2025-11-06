# Gamodoo

Plateforme permettant la gestion de tâches à réaliser interactives avec une jauge d’expérience évolutive dans une DA de jeu-vidéo.

## Installation

Cetter partie est pour la première installation. 
Le projet est composé de deux sous-modules qui sont les repos pour le front et le back.
Pour cloner le projet complet, voici l'ordre des commandes GIT :

```
git clone https://github.com/Wildyax/gamodoo.git
cd gamodoo
git submodule update --init --recursive
```

## Docker

Pour lancer le back en dev, ouvrir un terminal et faire la commande :

```
docker compose -f docker-compose.dev.yml up --build
```

Pour lancer le front en local en même temps que le back, faire la commande suivante sur un autre terminal :

```
npx next dev 
```