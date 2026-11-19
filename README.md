# RoadForge Mobile V0.5 — prototype de test

Basé sur le ZIP V0.4 transmis par l'utilisateur.

## Ajouts
- Rond-point : bouton dédié, rayon 8–100 mètres, placement tactile. Huit segments de Bézier approximant un cercle. Pour raccorder une route, utilisez une extrémité du rond-point.
- Niveaux 0 à 3 : les croisements entre niveaux différents ne produisent pas de nœud commun. Ce sont des niveaux logiques, pas encore des ponts 3D.
- Diagnostic : composantes connexes, extrémités libres, nœuds et segments.
- Export du graphe en version 2, avec `level` sur les nœuds et arêtes.
- Format de carte ForgeMap v1 conservé, propriété `level` facultative.

## Limitations
- Ronds-points composés de 8 segments modifiables individuellement ; édition globale du rayon après placement non disponible.
- Pas de gestion du sens giratoire, des priorités, des voies ou des règles de circulation.
- Les intersections sont échantillonnées sur les courbes, avec une tolérance de 0,5 m sur les nœuds.
- Les routes à niveau différent peuvent sembler se croiser en vue 2D, mais ne sont pas connectées.
- Non testé sur Android : validation manuelle requise.

## Installation
Remplacer les quatre fichiers à la racine du dépôt GitHub Pages. Sauvegarder/exporter les cartes de test si besoin.
