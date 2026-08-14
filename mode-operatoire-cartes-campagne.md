# Mode opératoire — Templates de cartes de campagne (GF & AoF)

Ce mode opératoire couvre les deux templates (`gf-campaign-map-template.html` et `aof-campaign-map-template.html`). Ils fonctionnent exactement de la même façon ; seuls le style visuel, les polices et les palettes disponibles diffèrent.

**Pour commencer :** ouvre le fichier `.html` dans un navigateur (double-clic dessus, ou glisse-le dans une fenêtre de navigateur). Tout se passe dans la page, aucune installation n'est nécessaire. Ton travail n'est pas sauvegardé automatiquement — voir la section Export en fin de document.

---

## 1. Charger le relief de terrain

1. Clique n'importe où sur la grande zone centrale (le fond de la carte).
2. Choisis ton image de terrain (relief, heightmap, rendu Blender, etc.) depuis ton ordinateur.
3. Tu peux aussi glisser-déposer l'image directement sur cette zone.
4. Pour la remplacer, utilise le bouton **"Changer le terrain"** dans la barre d'outils en bas de l'écran.
5. Une fois l'image en place, deux réglages sont disponibles :
   - **Curseur d'échelle** (à côté du bouton "Changer le terrain") : zoome ou dézoome le terrain.
   - **Glisser l'image directement** : clique dessus et déplace la souris pour la repositionner dans le cadre.

## 2. Remplir les textes

Tous les textes sont directement modifiables :
- Clique sur un champ (titre, sous-titre, notes, titres de panneaux, noms, descriptions).
- Tape ton texte.
- Clique en dehors pour valider — pas de bouton "enregistrer" à part entière.

## 3. Personnaliser les icônes (légende, factions, soutien)

Chaque petit symbole vide (rond ou carré) à côté d'un nom est une zone d'upload :
1. Clique dessus pour choisir une image (idéalement un **PNG à fond transparent** pour un rendu propre).
2. Ou glisse-dépose ton image directement dessus.

## 4. Ajouter / supprimer des lignes

En bas de chaque panneau (**Légende / Points remarquables**, **Factions**, **Soutien**), un bouton **"+ Ajouter..."** permet de créer autant de lignes que nécessaire.

Pour supprimer une ligne : survole-la avec la souris, un **×** rouge apparaît en haut à droite — clique dessus.

## 5. Supprimer / réafficher un panneau entier

Si tu n'as pas besoin d'un panneau (ex. pas de "Soutien" pour cette bataille) :
- Survole le panneau : un **×** apparaît en haut à droite du cadre — clique dessus pour le masquer.
- Pour le faire réapparaître, clique sur son nom dans la barre d'outils (**Légende / Factions / Soutien**) — ces boutons s'assombrissent quand le panneau correspondant est masqué, pour indiquer son état.

Le contenu du panneau n'est pas perdu quand tu le masques, seulement caché.

## 6. Placer des symboles directement sur la carte

Deux façons de poser un symbole sur le terrain :

- **Marqueur vierge** : clique sur **"+ Marqueur"** dans la barre d'outils. Un petit cadre vide apparaît au centre de la carte — clique dessus pour lui assigner une image, comme pour les icônes de légende.
- **Copier un symbole existant** : une fois qu'une icône de légende, de faction ou de soutien a une image, tu peux la **glisser directement sur la carte** pour en poser une copie à l'endroit voulu.

Une fois posé, un marqueur se **déplace** en cliquant dessus et en le faisant glisser où tu veux sur la carte.

Pour le supprimer : survole-le, un **×** apparaît en haut à droite du marqueur — clique dessus (un petit mouvement de souris pendant le clic est interprété comme un déplacement, pas une suppression — vise directement le ×).

## 7. Changer la police

Menu déroulant **"Police de la carte"** dans la barre d'outils : 5 choix par template, appliqués instantanément à l'ensemble de la carte (titres et texte courant).

- **GF** : Tactique, Orbital, Militaire, Cybernétique, Brutaliste.
- **AoF** : Vieux Monde, Chronique, Grimoire, Royaume, Runique.

## 8. Changer la palette de couleurs

Menu déroulant **"Palette de couleurs"**, juste à côté du choix de police. 5 choix par template, indépendants de la police (tu peux combiner librement) :

- **GF** : Teal Tactique, Rouge Sanglant, Vert Toxique, Or Impérial, Violet Psychique.
- **AoF** : Vieux Monde, Royaume Vert, Sang et Acier, Glace et Os, Sable Doré.

## 9. Sauvegarder et recharger un projet

Contrairement à l'export PDF (qui fige la carte en image), la sauvegarde de projet garde tout **modifiable** pour y revenir plus tard.

- **Sauvegarder** : clique sur **"Sauvegarder"** dans la barre d'outils. Un fichier `.json` est téléchargé (nommé automatiquement d'après le titre de ta carte) — il contient tous les textes, toutes les images (terrain, icônes, marqueurs), leurs positions, ainsi que la police et la palette choisies.
- **Charger** : clique sur **"Charger"**, sélectionne un fichier `.json` sauvegardé précédemment — la carte se reconstruit entièrement telle que tu l'avais laissée.

Range ces fichiers `.json` avec tes cartes (un par bataille/secteur) : ils te permettent de reprendre une carte en cours, ou de repartir d'une carte existante pour en faire une variante.

## 10. Exporter la carte finie

Deux formats possibles selon l'usage :

- **"Exporter en PNG"** : télécharge la carte sous forme d'**image**, prête à être uploadée sur ton blog WordPress (ou tout autre site) comme une photo classique — c'est l'option à privilégier pour partager ton travail en ligne.
- **"Imprimer / PDF"** : ouvre la fenêtre d'impression du navigateur. Choisis **"Enregistrer en PDF"** comme imprimante (au lieu d'une imprimante physique), en orientation **paysage**. Utile pour l'impression physique ou un envoi en PDF.

Dans les deux cas, la barre d'outils et les boutons de suppression/ajout disparaissent automatiquement — seule la carte est visible dans le résultat final.

---

## Points de vigilance

- Le travail n'est **pas sauvegardé automatiquement** si tu fermes l'onglet : utilise le bouton **"Sauvegarder"** (fichier `.json`, modifiable plus tard) avant de fermer, et **"Imprimer / PDF"** une fois la carte terminée.
- Une carte par bataille/secteur : duplique le fichier `.html` (ou garde un `.json` par carte) pour garder tes anciennes versions.
- Prévois des images de symboles en **PNG transparent** carré (ex. 200×200 px) pour un rendu net une fois redimensionné.
- Le fichier `.json` de sauvegarde n'est utilisable qu'avec le même template (`.html`) dont il provient — garde les deux ensemble.
