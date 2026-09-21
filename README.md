# Piles & accumulateurs — réviser le DS

Page web de révision pour le chapitre **« Stocker de l'énergie électrique avec un système
électrochimique : oxydoréduction et pile chimique »**, au programme de sciences physiques en
terminale bac pro.

Construite à partir de deux TP (pile au citron, pile Daniell), de la feuille de cours et de la
page d'exercices « Je teste mes acquis ».

## Utilisation

Ouvrir la page en ligne, ou télécharger `index.html` et l'ouvrir par double-clic.
Un seul fichier, aucune installation, fonctionne hors ligne (la connexion ne sert qu'aux polices).

La partie « DS blanc » s'imprime proprement : les corrigés, repliés, ne sortent pas sur le papier.

## Contenu

Le parcours suit l'ordre d'exigence d'un devoir surveillé : restituer, écrire, calculer, composer.

- **Mémo éclair** — les six points à relire s'il ne reste que deux minutes.
- **1 · Oxydoréduction** — l'échange d'électrons, où placer les électrons dans une demi-équation,
  échange spontané (pile) contre échange imposé (électrolyse), et quel métal attaque l'autre.
- **2 · La pile, et les équations** — schéma commenté de la pile Daniell ; la méthode d'écriture
  d'une équation-bilan en trois temps, dont l'égalisation des électrons ; les trois piles du
  chapitre entièrement rédigées (zinc/cuivre, zinc/argent, cuivre/argent) ; six questions de
  contrôle ; un schéma nu à légender en sept repères.
- **3 · L'accumulateur** — schéma de comparaison charge / décharge, `Q = I × t` et `E = Q × U`
  avec leurs formes dérivées, série contre parallèle.
- **4 · Les calculs** — 17 exercices chiffrés en quatre séries (conversions, capacité, énergie,
  série/parallèle), réponse à saisir, indice en cas d'erreur, correction rédigée comme sur une copie.
- **5 · QCM** — 18 questions corrigées une par une : les 10 de « Je teste mes acquis » et 8 des TP.
- **6 · DS blanc** — un sujet complet sur 20 points, cinq exercices, barème par question et corrigé
  rédigé dépliable.
- **7 · Pièges** et check-list de dernière minute.

## Points de cours les plus piégeux

- Dans la pile Daniell, le **zinc se ronge** et le **cuivre s'épaissit**, jamais l'inverse.
- L'ion argent ne capte qu'**un** électron : `Ag⁺ + e⁻ → Ag`. Il faut donc doubler cette
  demi-équation avant de l'additionner à celle du zinc.
- Une **équation-bilan ne contient jamais d'électrons** : ils se simplifient.
- Le pont salin laisse passer les **ions** ; les **électrons** passent par le fil extérieur.
- En série, les **tensions** s'additionnent et la capacité en Ah ne change pas. En parallèle,
  c'est l'inverse.
- La capacité se mesure en **Ah**, l'énergie en **Wh**.
- En charge, l'accumulateur se comporte comme un **électrolyseur** ; en décharge, comme une **pile**.

## Détails techniques

- Un seul fichier HTML : HTML + CSS + JavaScript vanilla, zéro dépendance hors Google Fonts.
- Les questions, les exercices et les étiquettes de légende sont dans des tableaux de données en
  haut du script, séparés de la logique d'affichage. Le moteur de QCM est monté deux fois, sur les
  équations et sur le QCM général, et détecte tout seul les questions à réponses multiples.
- Saisie numérique tolérante : virgule ou point, espaces et unité tapée en trop sont ignorés,
  tolérance d'arrondi de 0,2 % avec un plancher absolu.
- Progression enregistrée en `localStorage` sous `try/catch` : si le stockage est indisponible
  (navigation privée, page ouverte en `file://` ou `data:`), la page fonctionne quand même.
- Les trois schémas (pile Daniell légendée, pile nue à légender, charge/décharge) sont du SVG
  écrit à la main, sans image ni bibliothèque, et suivent la couleur du texte pour rester lisibles
  dans les deux thèmes.
- Mode sombre via `prefers-color-scheme`, `prefers-reduced-motion` respecté, focus clavier visible,
  touche Entrée pour valider une réponse chiffrée, feuille de style d'impression pour le DS blanc.
- Typographie : Archivo pour les titres, IBM Plex Serif pour le texte, IBM Plex Mono pour les
  unités et les équations.

Les 17 réponses chiffrées et le barème du DS blanc (20 points répartis sur 20 questions) ont été
recalculés indépendamment du HTML avant publication.
