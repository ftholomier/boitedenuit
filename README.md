# Easy Night — Club &amp; Rooftop

Site web vitrine pour la boîte de nuit **Easy Night**. Site statique (HTML / CSS / JS
sans build), prêt à héberger tel quel (GitHub Pages, Netlify, Vercel, n'importe quel
serveur statique).

## Aperçu

Page unique (one-page) avec navigation ancrée et les sections suivantes :

- **Hero** — accroche, horaires clés, appels à l'action
- **Le club** — concept (Main Floor, Rooftop, Carré VIP) + statistiques animées
- **Programmation** — liste des prochaines soirées
- **Galerie** — grille de visuels (blocs de démo à remplacer par les vraies photos)
- **Tables VIP** — formules Silver / Gold / Black
- **Infos** — horaires, accès, dress code, réseaux sociaux
- **Réservation** — formulaire (démo front-end, à brancher sur un back-end / service)

Design sombre « néon » (magenta / violet / cyan), responsive, avec animations au scroll
et respect de `prefers-reduced-motion`.

## Structure

```
.
├── index.html        # structure de la page
├── css/styles.css    # styles + responsive + animations
├── js/main.js        # nav mobile, reveal au scroll, compteurs, formulaire
└── README.md
```

## Lancer en local

Aucune dépendance. Ouvre `index.html` dans un navigateur, ou sers le dossier :

```bash
python3 -m http.server 8000
# puis http://localhost:8000
```

## À personnaliser

- **Visuels** : remplacer les blocs `.gallery__item` par de vraies images (dossier
  `assets/` à créer) et ajouter une image de fond au hero si souhaité.
- **Coordonnées** : adresse, horaires et réseaux sociaux dans la section « Infos »
  de `index.html`.
- **Programmation** : mettre à jour les `<article class="event">`.
- **Formulaire** : le `submit` est une démo côté client. Le brancher sur un service
  (Formspree, Netlify Forms, une API…) pour recevoir réellement les demandes.
- **Couleurs / typos** : variables CSS en haut de `css/styles.css` (`:root`).

## Note sur le design d'origine

Ce site a été construit à partir du nom et du concept « Easy Night » — le fichier
`Easy Night.dc.html` du projet Claude Design n'a pas pu être récupéré automatiquement
dans cet environnement (projet privé, authentification indisponible en session web).
Pour aligner exactement les couleurs et la typographie sur la maquette, envoie le
design via « Send to Claude Code » ou colle son contenu.
