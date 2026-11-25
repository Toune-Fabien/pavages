# Pavages Bézier

Dessine des pavages périodiques à la Escher : édition de courbes de Bézier pour définir le contour d'un pavé (groupe de symétrie p2 — demi-tours et translations), motif au pinceau reproduit automatiquement dans toutes les copies, export en image (PNG) ou en gabarit SVG à l'échelle réelle (mm), pour impression et découpe.

Application 100% côté client (HTML/CSS/JS), sans serveur ni collecte de données. Le dessin est sauvegardé localement dans le navigateur (`localStorage`).

## Développement local

Servir le dossier avec n'importe quel serveur statique, par exemple :

```bash
python3 -m http.server 8000
```

Puis ouvrir `http://localhost:8000/`.

## PWA

- `manifest.webmanifest` : nom, icône, couleurs, mode `standalone`
- `sw.js` : service worker minimal (cache de l'app shell, réseau d'abord pour le HTML)

## Publication Android (EDU-CONSULT)

Voir le projet « Publication d'apps mobiles » : conversion en TWA (PWABuilder) ou en app Capacitor, puis publication sur la Google Play Console du compte organisation EDU-CONSULT.
