# RoadForge Mobile V0.6 — Prototype Android

## Nouveautés
- Rond-point sélectionnable dans **Modifier** : panneau rayon (8–100 m), voies (1–3), appliquer, supprimer.
- Déplacer un segment d'un rond-point en mode Modifier déplace tout le rond-point.
- Les routes dont l'extrémité correspond à un point du rond-point (tolérance 0,51 m) suivent son déplacement/redimensionnement.
- Les huit segments du rond-point conservent un identifiant de groupe, un centre, un rayon et un nombre de voies.
- Les cartes V0.5 sans groupes restent importables ; les ronds-points créés dans les anciennes versions restent de simples segments indépendants.

## Limites connues
- Les voies sont des métadonnées, sans simulation de circulation.
- Les connexions aux points intermédiaires d'un arc ne sont pas préservées lors d'un redimensionnement.
- Les routes raccordées ne sont déplacées que par leurs extrémités ; une géométrie courbe peut devoir être retouchée.
- Le réseau est recalculé depuis la géométrie. Il n'y a pas encore de vrais raccordements 3D ou de routage directionnel.
- À tester manuellement sur Android avant validation.

## Publication
Extraire et remplacer les quatre fichiers du dépôt GitHub Pages. Vérifier que le titre indique V0.6.
