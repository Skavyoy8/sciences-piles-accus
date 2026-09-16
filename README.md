# Piles & accumulateurs — fiche de révision et QCM

Page web de révision pour le chapitre **« Stocker de l'énergie électrique avec un système
électrochimique »**, au programme de sciences physiques en terminale bac pro.

Construite à partir de deux TP (pile au citron, pile Daniell), de la feuille de cours et de la
page d'exercices « Je teste mes acquis ».

## Utilisation

Ouvrir la page en ligne, ou télécharger `index.html` et l'ouvrir par double-clic.
Un seul fichier, aucune installation, fonctionne hors ligne (la connexion ne sert qu'aux polices).

## Contenu

- **Mémo éclair** — les six points à relire s'il ne reste que deux minutes.
- **1 · Oxydoréduction** — l'échange d'électrons, les couples oxydant/réducteur, la différence
  entre un échange spontané (pile) et un échange imposé (électrolyse).
- **2 · La pile** — schéma commenté de la pile Daniell : sens des électrons, rôle du pont salin,
  demi-équations sous chaque électrode. Tableau des tensions mesurées en TP (0,32 V au citron,
  0,64 V en série, 1,1 V pour la pile Daniell) et les deux questions classiques : comment
  augmenter la tension, comment augmenter l'intensité.
- **3 · L'accumulateur** — schéma de comparaison charge / décharge, les formules `Q = I × t` (Ah)
  et `E = Q × U` (Wh), trois calculs corrigés.
- **4 · QCM** — 18 questions corrigées une par une, avec explication à chaque réponse : les 10 de
  la feuille « Je teste mes acquis » et 8 tirées des TP.
- **5 · Pièges** et check-list de dernière minute.

## Points de cours les plus piégeux

- Dans la pile Daniell, le **zinc se ronge** et le **cuivre s'épaissit**, jamais l'inverse.
- Le pont salin laisse passer les **ions** ; les **électrons** passent par le fil extérieur.
- En série, les **tensions** s'additionnent et la capacité en Ah ne change pas. En parallèle,
  c'est l'inverse.
- La capacité se mesure en **Ah**, l'énergie en **Wh**.
- En charge, l'accumulateur se comporte comme un **électrolyseur** ; en décharge, comme une **pile**.

## Détails techniques

- Un seul fichier HTML : HTML + CSS + JavaScript vanilla, zéro dépendance hors Google Fonts.
- Les 18 questions du QCM sont dans un tableau de données en haut du script, séparé de la logique
  d'affichage. Les questions à réponses multiples sont détectées automatiquement.
- Les deux schémas (pile Daniell, charge/décharge) sont du SVG écrit à la main, sans image ni
  bibliothèque, et suivent la couleur du texte pour rester lisibles dans les deux thèmes.
- Mode sombre via `prefers-color-scheme`, `prefers-reduced-motion` respecté, focus clavier visible.
- Typographie : Archivo pour les titres, IBM Plex Serif pour le texte, IBM Plex Mono pour les
  unités et les équations.
