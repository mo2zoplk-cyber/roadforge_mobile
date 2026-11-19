# RoadForge Mobile V0.4 — Graphe routier (étape 1)

## Ajouts
- Détection de carrefours (croix, T, Y) entre routes droites et courbes au même niveau.
- Graphe routier dérivé avec nœuds, connexions, identifiants de route et coordonnées métriques.
- Bouton **Nœuds** pour afficher/masquer les carrefours.
- Bouton **Réseau JSON** pour exporter `roadforge-network.json` (distinct de la sauvegarde de carte).
- Compatible avec les cartes ForgeMap V1 de la V0.3.

## Limites connues
- Les croisements courbes sont approximés par 48 segments ; précision à affiner.
- Pas encore de ponts ni de tunnels : tous les croisements sont au même niveau.
- Pas encore de sens de circulation, voies, feux, priorités ou ronds-points.
- Les nœuds proches de moins de 0,5 m sont fusionnés pour le graphe, sans déplacer visuellement les routes.
- Les routes qui se superposent sur une longueur ne sont pas fusionnées.
- Tests tactiles Android et tests de routage Unity non encore effectués.

## Installation
Remplacer à la racine du dépôt GitHub Pages les quatre fichiers du ZIP. Après publication, recharger la page.

## Test suggéré
Créer une croix avec deux routes droites ; un nœud vert doit apparaître au croisement. Créer un T en terminant une route sur une autre ; le nœud doit également apparaître. Exporter le réseau JSON et vérifier les nœuds/connexions.
