# TP7 : Docker avancé et Docker Compose

**Étudiant :** Ferid Saad
**Formation :** Master DevOps & Cloud, ISET Tozeur
**Environnement :** VM Ubuntu Server 26.04, Docker 29.1.3, Compose v5.6.0, Buildx v0.37.1

## 1. Objectif
Produire une image Docker petite et sûre (multi-stage, non-root, HEALTHCHECK), puis décrire une pile complète (app + PostgreSQL + Adminer) avec Docker Compose, et construire une image multi-architecture avec Buildx.

## 2. Partie 1 : Couches et cache
_À compléter : pourquoi `npm install` est réexécuté après modification de `server.ts` ?_

## 3. Partie 2 : Mesures de l'image naïve
_À compléter._

## 4. Partie 3 : Dockerfile multi-stage

| Indicateur | naive | multistage |
|---|---|---|
| Taille de l'image | | |
| Temps de build (à froid) | | |
| Temps de build (code modifié) | | |
| Vulnérabilités HIGH/CRITICAL | | |
| Utilisateur | | |

![Comparaison des images](captures/image-comparison.png)
![Utilisateur non-root](captures/non-root.png)

## 5. Partie 4 : Pile Docker Compose
_À compléter : persistance, isolation réseau, effet de `docker compose down -v`, problème du `--scale app=2` avec `ports`._

![docker compose ps](captures/compose-ps.png)
![Persistance](captures/persistence.png)

## 6. Partie 5 : Buildx multi-architecture
_À compléter._

![Manifest multi-arch](captures/buildx-manifest.png)

## 7. Défi (optionnel)
_Nginx reverse proxy et secret de build._

![Reverse proxy](captures/reverse-proxy.png)
