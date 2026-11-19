# RoadForge Mobile V0.2

Éditeur de cartes 2D pour Android via GitHub Pages.

## Nouveautés
- Croisements détectés et affichés par points verts (pas encore un graphe de navigation).
- Accrochage magnétique des nouveaux points aux extrémités existantes.
- Routes courbes quadratiques avec courbure automatique.
- Compatibilité avec les sauvegardes locales et fichiers JSON ForgeMap V1 de la V0.1.
- Mise à jour du cache PWA (v02).

## Installation GitHub Pages
Remplacer les fichiers à la racine du dépôt GitHub : `index.html`, `sw.js`, `manifest.webmanifest`, `README.md`.
Vérifier Settings > Pages > Deploy from branch > main > /(root). Attendre le déploiement, puis actualiser la page.

## Limites connues
- Les croisements ne sont pas encore des nœuds routables et les ponts ne sont pas distingués.
- La courbure est automatique; l'édition du point de contrôle est prévue plus tard.
- La sauvegarde locale reste liée au navigateur/appareil : exporter régulièrement le JSON.
- Pas de génération Unity 3D à ce stade.
