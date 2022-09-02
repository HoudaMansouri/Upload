# Les récommandations SEO

## 1. Sémantique
- On vérifie l'utilisation des balises appropriées

## 2. Plus de sens avec les microdatas
- On utilise les définitions de schémas de schema.org
- https://schema.org/
- https://search.google.com/structured-data/testing-tool

## 3. Metadonnées
- On redige des title et une description pertinente par page
- Pourquoi pas tester les meta og pour avec des partages plus jolis sur facebook (et d'autres applications comme slack)

## 4. Rédaction des contenus
- On vérifie la pertinence de nos titres h1, h2, h3 etc
- Les intitulés des liens

## 5. Médias
- On rempli les textes alternatifs pour rendre comphérensibles nos images
- Pourquoi pas optimiser les images en jetant un oeil au format webp

Comment choisir le bon format d'image ?
-> Est-ce que mon image est du type photo ou du type image avec plein d'applats de couleurs
-> si beaucoup de couleur (photo) -> jpg
-> si beaucoup d'applats -> 
  -> si vectoriel -> svg
  -> si bitmap -> png
-> si transparence -> png

Avec webp -> si vectoriel -> svg -> sinon webp
/!\ le webp n'est supporté qu'à 80% à ce jour
Si on l'utilise en production il faut une solution

## 6. Faciliter l'exploration
- Sitemap.xml
- Le sitemap liste toutes les pages de notre site qu'on veut voir potientielement sur le moteur de recherche
- Il existe des outils qui "crawlent" qui parcourent notre site, explorent notre site pour trouver toutes les pages
- https://www.xml-sitemaps.com/
- Robots.txt
- Le Robots.txt s'adressent à tous les robots pour indiquer à des robots de ne pas regarder certains parties, il peut en plus s'adresser differement à chaque robot
- http://robots-txt.com/
- Un petit mot sur noindex, nofollow sur les liens ou la meta robots
```html
<!-- on peut aussi par page mettre une meta robots, noindex signifie on ne souhaite pas indexer cette page, nofollow signifie on ne souhaite pas que le robot explore les liens présents sur cette -->
<meta name="robots" content="noindex, nofollow">
```
- Il est également possible de passer ces infos directement sur un lien 
`<a rel="nofollow" href="http://radin.com">Codes promos pour des firugines</a>` ici le moteur de recherche n'ira pas voir radin.com

## 7. Audit
- Utiliser l'outil intégré à google chrome pour avoir une première évaluation