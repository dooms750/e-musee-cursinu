# e-Musée Cursinu

Musée virtuel immersif consacré au **Cursinu**, le chien corse.

Le visiteur suit le Cursinu en 3D le long d'un sentier, dans un paysage corse dont l'heure avance de l'aube au crépuscule. La visite traverse quatre espaces, tirés du cahier des charges du projet :

| Espace | Contenu |
|---|---|
| Accueil | Présentation du Cursinu et invitation à le suivre |
| I. Il vient de loin | Frise chronologique et archives antérieures à la reconnaissance |
| II. A casetta di u Cursinu | Bibliothèque, vidéothèque, dossier de reconnaissance, photothèque, objets et œuvres, standard 3D interactif |
| III. Le territoire | Carte de Corse des anecdotes et témoignages |
| IV. Le Cursinu s'éloigne | Livre d'or |

## Fonctionnalités

- Paysage 3D : relief, mer, ciel physique, brume, maquis, pins laricio, herbes au vent, ombres.
- Cursinu en 3D avec animation de trot calculée (pattes, queue, tête) et mouvements au repos.
- Visionneuse du standard : 13 régions du corps, rotation libre, points de repère.
- Recherche documentaire, navigation au clavier (flèches), ambiance sonore générée (vent, oiseaux, rivière, cloches).
- Site responsive (ordinateur, tablette, téléphone).

## Lancer le site en local

Le modèle 3D est chargé par le navigateur : ouvrir `index.html` directement depuis le disque ne fonctionne pas. Servez le dossier avec un petit serveur :

```bash
python3 -m http.server 8000
```

puis ouvrez http://localhost:8000.

## Publier avec GitHub Pages

Settings → Pages → Source : branche `main`, dossier racine. Le site est alors en ligne à l'adresse `https://<compte>.github.io/<dépôt>/`.

## Contenus à compléter

- Les documents marqués « À verser » sont des emplacements prêts à recevoir les numérisations (PDF, photos, vidéos, sons).
- Les fiches de la carte marquées « Exemple » attendent les témoignages réels.
- Les textes du standard 3D sont une synthèse de la description de la race, à remplacer par le texte officiel de la Société Centrale Canine.
- Le livre d'or enregistre les messages dans le navigateur du visiteur. Pour un livre d'or partagé, il faudra le relier à un service d'enregistrement (base de données ou formulaire).

## Crédits

- Conception : Jean Dominique Rossi.
- Modèle 3D du Cursinu : Jean Dominique Rossi et la société Arobase ([cursinu.corsica](https://cursinu.corsica/)). Version allégée pour le web (textures WebP, géométrie compressée).
- Bibliothèque 3D : [three.js](https://threejs.org/).
