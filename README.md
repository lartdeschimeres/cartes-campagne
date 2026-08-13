# Cartes de campagne — Grimdark Future & Age of Fantasy

Générateur de cartes tactiques pour campagnes de wargaming, basé sur le ruleset gratuit **One Page Rules** (OPR). Deux styles disponibles :

- **Grimdark Future** (sci-fi) — style HUD tactique, tons froids.
- **Age of Fantasy** (fantasy) — style chronique/parchemin.

Tout se passe directement dans le navigateur, aucune installation requise : upload d'un fond de terrain, personnalisation des textes et des icônes, placement de marqueurs, choix de police et de palette, sauvegarde/rechargement de projet, export en PNG.

## Voir les cartes en ligne

👉 **[Page d'index](../../)** — choisis ta carte entre GF et AoF.

Accès direct :
- [Grimdark Future](./gf-campaign-map-template.html)
- [Age of Fantasy](./aof-campaign-map-template.html)

## Utilisation

1. Ouvre la carte voulue (lien ci-dessus, ou double-clique sur le fichier `.html` en local).
2. Clique sur la zone centrale pour charger ton fond de terrain (relief, heightmap, rendu...).
3. Personnalise les textes, les icônes de légende/factions/soutien, et pose des marqueurs sur la carte.
4. Ajuste la police et la palette de couleurs via les menus déroulants de la barre d'outils.
5. Exporte le résultat :
   - **Exporter en PNG** — image prête à publier (blog, réseaux sociaux, etc.).
   - **Imprimer / PDF** — pour une impression physique.
   - **Sauvegarder** — génère un fichier `.json` conservant tout le projet (textes, images, positions, police, palette), rechargeable via **Charger** pour reprendre le travail plus tard.

Le mode opératoire détaillé est disponible dans [`mode-operatoire-cartes-campagne.md`](./mode-operatoire-cartes-campagne.md).

## Structure du dépôt

```
index.html                        → page d'accueil (choix de la carte)
gf-campaign-map-template.html     → template Grimdark Future
aof-campaign-map-template.html    → template Age of Fantasy
mode-operatoire-cartes-campagne.md → guide d'utilisation détaillé
```

## Mettre à jour une carte

Pour modifier un template : remplace le fichier correspondant dans le dépôt (même nom) et commit. Si le dépôt est publié via **GitHub Pages**, les liens et iframes existants (ex. intégrés dans un blog WordPress) se mettent à jour automatiquement, sans rien changer côté site.

## Notes techniques

- Aucune dépendance à installer : les polices (Google Fonts) et la librairie d'export d'image (html2canvas) sont chargées depuis un CDN au moment de l'ouverture de la page.
- Les projets sauvegardés (`.json`) contiennent les images en base64 — ils ne sont utilisables qu'avec le template (`.html`) dont ils proviennent.
- Formats d'image supportés pour le terrain et les icônes : PNG, JPG, WebP. Les formats TIFF/EXR ne sont pas affichables par les navigateurs — un message d'avertissement s'affiche le cas échéant.

## Licence

Distribué sous licence [MIT](./LICENSE).
