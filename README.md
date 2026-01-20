# Gamodoo

Plateforme permettant la gestion de tâches à réaliser interactives avec une jauge d’expérience évolutive dans une DA de jeu-vidéo.

## Installation

Cetter partie est pour la première installation. 
Le projet est composé de deux sous-modules qui sont les repos pour le front et le back.
Pour cloner le projet complet, voici l'ordre des commandes GIT :
```bash
git clone https://github.com/Wildyax/gamodoo.git
cd gamodoo
git submodule update --init --recursive
```

## Docker

Pour lancer le front et le back en même temps il faut se mettre à la racine du projet et :

La première fois il faut build les container
```bash
docker compose build
```

Ensuite on peut utiliser cette commande
```bash
docker compose up
```

- Url du front docker : http://localhost:3000/
- Url du back docker : http://localhost:8080/
