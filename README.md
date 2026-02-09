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

Plusieurs changements ont été réalisés sur le docker.

### Back en docker && Front en local

Avec cette configuration seul le backend tourne sous docker. Ceci est requis pour pouvoir dev sur le front en même temps car windows/mac os + turbopack ne permettent pas de surveiller les changement de fichier lorsque next.js est lancé avec docker.

La première fois avec le build :

```bash
docker compose -f docker-compose.yml -f docker-compose.dev.yml up --build
```
Les fois suivantes pour aller plus vite :

```bash
docker compose -f docker-compose.yml -f docker-compose.dev.yml up
```

Enfin pour lancer le front depuis sont local 

```bash
npx next dev 
```

Ou

```bash
npm run dev
```

### Back && Front en docker

Cette configuration fait tourner le front et le back en même temps sur docker. Surout utile pour le rendu final ou pour juste tester la connexion entre les deux.

La première fois avec le build :

```bash
docker compose up --build
```
Les fois suivantes pour aller plus vite :

```bash
docker compose up
```

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
