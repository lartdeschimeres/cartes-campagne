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

### Choisir la couleur des symboles
À gauche de chaque icône se trouve un **sélecteur de couleur** (petit carré coloré). Ce sélecteur permet de **teinter l'icône** avec la couleur de ton choix :
- Clique sur le sélecteur pour ouvrir la palette de couleurs.
- Choisis une couleur : l'icône sera automatiquement teintée avec cette couleur.
- La couleur est **sauvegardée avec le projet** et sera restaurée lors du chargement.

**Astuce :** Pour un meilleur résultat, utilise des icônes **noires ou blanches** en PNG transparent. Les icônes colorées peuvent ne pas bien réagir à la teinte.

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

**Note :** La palette de couleurs affecte les éléments d'interface (fond, texte, bordures), tandis que le **sélecteur de couleur des symboles** (voir section 3) permet de personnaliser individuellement chaque icône.

## 9. Sauvegarder et recharger un projet

Contrairement à l'export PDF (qui fige la carte en image), la sauvegarde de projet garde tout **modifiable** pour y revenir plus tard.

- **Sauvegarder** : clique sur **"Sauvegarder"** dans la barre d'outils. Un fichier `.json` est téléchargé (nommé automatiquement d'après le titre de ta carte) — il contient tous les textes, toutes les images (terrain, icônes, marqueurs), leurs positions, ainsi que la police et la palette choisies.
- **Charger** : clique sur **"Charger"**, sélectionne un fichier `.json` sauvegardé précédemment — la carte se reconstruit entièrement telle que tu l'avais laissée.

Range ces fichiers `.json` avec tes cartes (un par bataille/secteur) : ils te permettent de reprendre une carte en cours, ou de repartir d'une carte existante pour en faire une variante.

## 10. Annuler / Rétablir (Undo / Redo)

Toutes les opérations qui modifient la carte peuvent être annulées **et rétablies** :

- **↶ Annuler** : bouton dans la barre d'outils, ou **Ctrl+Z** (Cmd+Z sur Mac).
- **↷ Rétablir** : bouton dans la barre d'outils, ou **Ctrl+Y** (ou Ctrl+Shift+Z).

Sont annulables/rétablissables : ajout/suppression de ligne, ajout/suppression/déplacement/redimensionnement de marqueur, chargement d'une image (terrain ou icône), chargement d'un projet, création d'une nouvelle carte, **et les modifications de texte** dans tous les champs (titres, descriptions, noms de calques, étiquettes). L'historique conserve les 50 dernières actions. Dans les champs `<input>`/`<textarea>` natifs, c'est l'annulation native du navigateur qui s'applique.

## 11. Sauvegarde automatique

Le navigateur enregistre automatiquement ton travail (dans le `localStorage`), environ 800 ms après chaque modification. Si tu fermes l'onglet par accident, à la réouverture un message te proposera de **récupérer la carte précédente**. Cette sauvegarde est propre à chaque template (AoF et GF) et à chaque navigateur. Elle ne remplace pas la **Sauvegarde** manuelle (fichier `.json`) : pour archiver ou transférer une carte, utilise toujours « Sauvegarder ».

## 12. Nouvelle carte (vider la planche)

Le bouton **« Nouvelle carte »** remet la planche à vide (efface terrain, textes, icônes, marqueurs) pour repartir d'un fond propre. Une confirmation est demandée avant l'effacement. Comme toute action, elle est **annulable** via ↶ Annuler / Ctrl+Z si tu changes d'avis.

## 12. Dupliquer, redimensionner et organiser les marqueurs

- **Dupliquer un marqueur** : **Alt+clic** sur un marqueur, ou **clic droit** → une copie est créée juste à côté. Pratique pour poser plusieurs unités identiques.
- **Redimensionner un marqueur** : survole-le, une **poignée dorée** apparaît en bas à droite. Glisse-la pour ajuster la taille (16 à 200 px). La taille est conservée à la sauvegarde.
- **Calques** : ouvre le panneau **« Calques »** (bouton dans la barre d'outils). Crée plusieurs calques (ex. « Armées du Nord », « Renforts », « Objectifs »), choisis le **calque actif** via le menu déroulant : les nouveaux marqueurs/étiquettes y sont placés. Coche/décoche un calque pour l'afficher ou le masquer. Renomme un calque en éditant son nom directement ; supprime-le avec le **×** (ses marqueurs retournent sur le calque « Par défaut »).

## 13. Étiquettes de texte libre sur la carte

Le bouton **« + Étiquette »** crée une étiquette de texte positionnable sur la carte (noms de lieux, axes d'attaque, notes). Le texte est sélectionné à la création pour être édité immédiatement.

- **Éditer** le texte : clique simplement dedans.
- **Déplacer** l'étiquette : maintiens **Shift** et fais-la glisser (sans Shift, le clic édite le texte).
- **Supprimer** : le **×** en survol.

Les étiquettes appartiennent elles aussi à un calque et peuvent être masquées/affichées.

## 14. Exporter la carte finie

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
