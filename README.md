# RoadForge Mobile V0.3 — édition des courbes

Application web statique, à déposer à la racine du dépôt GitHub Pages.

## Nouveautés
- En mode **Modifier**, toucher une route puis glisser ses poignées vertes (extrémités) ou orange (courbure).
- **Inverser courbe** : sélectionner une route puis inverser la courbure, ou convertir une droite en courbe.
- **Redresser** : retirer le point de contrôle de la route sélectionnée.
- Annuler/rétablir, autosauvegarde et export JSON conservés.
- Cache du service worker mis à jour.

## Limites
- Les intersections restent **visuelles**, sans nœuds routables.
- Les données conservent le format ForgeMap v1 de la V0.2.
- Cette version est une étape fonctionnelle d'édition, pas encore la refonte complète du graphe routier.
- Les modifications tactiles et la publication GitHub Pages restent à valider sur Android.

## Installation
Sauvegarder/exporter la carte si besoin, puis remplacer les quatre fichiers à la racine du dépôt : index.html, sw.js, manifest.webmanifest, README.md.
