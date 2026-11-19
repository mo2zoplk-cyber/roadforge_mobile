# RoadForge Mobile V0.1

Prototype autonome d'éditeur de réseau routier 2D pour mobile.

## Démarrer

Sur ordinateur, dans ce dossier : `python -m http.server 8080` puis ouvrir `http://localhost:8080`.

Sur téléphone, héberger ces fichiers sur un serveur HTTPS statique (par exemple GitHub Pages) et ouvrir l'adresse dans Chrome. Le service worker met les fichiers en cache pour une utilisation ultérieure hors ligne. Ouvrir `index.html` directement peut fonctionner mais les fonctions PWA nécessitent HTTP(S).

## Contrôles

Mode Route : toucher le départ puis l'arrivée. Les coordonnées sont arrondies sur une grille de 5 mètres. Mode Déplacer : glisser la carte. Pincer avec deux doigts pour zoomer. Mode Modifier : sélectionner et glisser une route ; Supprimer enlève la route sélectionnée. Annuler / Rétablir. Exporter/importer des fichiers JSON.

## Limites connues

- Pas encore d'intersections automatiques, courbes, terrains, quartiers, ni de génération Unity.
- Le stockage local dépend du navigateur/appareil et peut être effacé ; exporter régulièrement une copie JSON.
- La PWA n'a pas encore d'icônes d'installation dédiées.
- Le rendu est une maquette fonctionnelle à tester sur appareil ; aucun test physique Android n'a été effectué.

## ForgeMap V1

`{ "format":"ForgeMap", "version":1, "units":"meters", "roads":[{"id":"...", "type":"street", "a":{"x":0,"y":0}, "b":{"x":100,"y":0}}] }`

Les axes X/Y représentent le plan horizontal de la carte. À l'import Unity, mapper X vers Unity X et Y vers Unity Z. La topologie (nœuds, croisements) sera explicitement modélisée dans une prochaine version.
