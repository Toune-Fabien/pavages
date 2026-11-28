# Pavages Bézier

Dessine des pavages périodiques à la Escher : édition de courbes de Bézier pour définir le contour d'un pavé (groupe de symétrie p2 - demi-tours et translations), motif au pinceau reproduit automatiquement dans toutes les copies, export en image (PNG) ou en gabarit SVG à l'échelle réelle (mm), pour impression et découpe.

Application 100% côté client (HTML/CSS/JS), sans serveur ni collecte de données. Le dessin est sauvegardé localement dans le navigateur (`localStorage`).

## Disponible sur Google Play

Pavages Bézier est publiée en production sur le Google Play Store (compte développeur organisation EDU-CONSULT, package `be.educonsult.pavages`) :

https://play.google.com/store/apps/details?id=be.educonsult.pavages

## Développement local (PWA)

Servir ce dossier avec n'importe quel serveur statique, par exemple :

```bash
python3 -m http.server 8000
```

Puis ouvrir `http://localhost:8000/`.

## PWA

- `manifest.webmanifest` : nom, icône, couleurs, mode `standalone`
- `sw.js` : service worker minimal (cache de l'app shell, réseau d'abord pour le HTML)

## Publication Android (EDU-CONSULT)

Ce dépôt contient uniquement la PWA (source web). L'app Android est produite à partir de ce code via un wrapper Capacitor (projet séparé, non versionné ici pour l'instant - voir https://github.com/Toune-Fabien/pavages-capacitor), puis publiée sur la Google Play Console du compte organisation EDU-CONSULT.
