# Piles & accumulateurs — du vocabulaire au DS

Cours progressif et exercices pour le chapitre **« Stocker de l'énergie électrique avec un système
électrochimique : oxydoréduction et pile chimique »**, au programme de sciences physiques en
terminale bac pro.

Construit à partir de deux TP (pile au citron, pile Daniell), de la feuille de cours et de la page
d'exercices « Je teste mes acquis ».

## Utilisation

Ouvrir la page en ligne, ou télécharger `index.html` et l'ouvrir par double-clic.
Un seul fichier, aucune installation, fonctionne hors ligne (la connexion ne sert qu'aux polices).

Les deux devoirs blancs s'impriment proprement : les corrigés, repliés, ne sortent pas sur le papier.

## Principe

Rien n'est supposé connu. La page commence par le **vocabulaire** et par la **lecture des symboles
chimiques**, et n'introduit qu'**une seule difficulté nouvelle à la fois**. Chaque notion est
présentée en trois temps : on explique, on montre un exemple entièrement résolu, puis on fait faire.

Les exercices portent tous une étiquette de niveau — *découverte* (une étape, aucune conversion),
*entraînement* (deux étapes, ou une conversion), *niveau DS* (énoncé habillé, questions enchaînées) —
et la majorité se trouve dans les deux premiers niveaux.

## Contenu

- **0 · Les mots du chapitre** — 14 fiches de vocabulaire : atome, électron, ion, électrode,
  électrolyte, tension contre intensité, capacité, heure décimale, calibre, série et parallèle,
  charge et décharge. Suivies de 10 questions de contrôle.
- **1 · Lire, puis écrire une équation** — décodage caractère par caractère de `Zn → Zn²⁺ + 2e⁻`,
  la règle d'or (le chiffre des charges donne le nombre d'électrons), coefficient contre exposant,
  oxydant et réducteur. Puis un escalier de 9 marches et 28 micro-questions, sans jamais parler de
  pile : on apprend d'abord à lire.
- **2 · Comment marche une pile** — le schéma de la pile Daniell monté en **trois temps** (le
  montage nu, on branche le fil, ce qui se passe chimiquement), la distinction électrons /
  courant conventionnel, l'axe `Zn — Cu — Ag` pour savoir qui est la borne −, les mesures des TP,
  un schéma nu à légender en sept repères et 8 questions sur les TP.
- **3 · Écrire l'équation-bilan** — deux exemples entièrement rédigés (le cas facile, puis le cas
  avec équilibrage), un escalier de 7 marches et 21 micro-questions, les pièges annoncés **avant**
  d'écrire, le tableau des trois piles en synthèse, et 6 questions de contrôle.
- **4 · L'accumulateur** — cours, schéma charge / décharge, les deux formules avec leurs triangles
  mnémotechniques, un entraînement à retourner une formule **sans chiffres**, et 10 questions de cours.
- **5 · Les calculs** — 61 exercices chiffrés en cinq séries, réponse à saisir, indice en cas
  d'erreur, correction rédigée comme au tableau.
- **6 · Mini-DS** — 10 points, 20 minutes, pour apprendre le format.
- **7 · DS blanc** — 20 points, 50 minutes, barème par question, corrigés dépliables.
- **8 · Les réponses de cours à savoir rédiger** — 10 questions avec leur réponse modèle à masquer.
- **9 · Les pièges** · **10 · Mémo éclair et check-list** · **11 · QR code de partage**.

Au total : 64 micro-questions, 24 questions de QCM, 61 exercices chiffrés, 7 repères de légende et
10 restitutions de cours.

## Points de cours les plus piégeux

- `Cu` et `Cu²⁺` ne sont pas la même chose : l'un est le métal de la lame, l'autre un ion dissous.
- Le chiffre des charges donne le nombre d'électrons : `Cu²⁺` en prend 2, `Ag⁺` n'en prend qu'**un**.
- Le chiffre **devant** compte les objets, celui **en haut à droite** compte les charges ; on ne
  modifie jamais un exposant.
- Une **équation-bilan ne contient jamais d'électrons** : ils se simplifient.
- Dans la pile Daniell, le **zinc se ronge** et le **cuivre s'épaissit**, jamais l'inverse.
- Les **électrons** vont du − vers le + ; le courant conventionnel est dessiné dans l'autre sens.
- Le pont salin laisse passer les **ions** ; les **électrons** passent par le fil.
- En série les **tensions** s'additionnent et la capacité ne bouge pas ; en parallèle, l'inverse.
- `1,3 h` vaut 1 h 18 min, pas 1 h 30.

## Détails techniques

- Un seul fichier HTML : HTML + CSS + JavaScript vanilla, zéro dépendance hors Google Fonts.
- Questions, micro-questions, exercices, étiquettes de légende et réponses de cours sont dans des
  tableaux de données en haut du script, séparés de la logique d'affichage. Le moteur de QCM est
  monté trois fois, le moteur d'escalier quatre fois.
- Saisie numérique tolérante : virgule ou point, espaces et unité tapée en trop ignorés, tolérance
  d'arrondi de 0,2 % avec un plancher absolu.
- Progression enregistrée en `localStorage` sous `try/catch` : si le stockage est indisponible
  (navigation privée, page ouverte en `file://` ou `data:`), la page fonctionne quand même.
- Huit schémas SVG écrits à la main, sans image ni bibliothèque, qui suivent la couleur du texte
  pour rester lisibles dans les deux thèmes. Le QR code est lui aussi du SVG généré hors ligne.
- Mode sombre via `prefers-color-scheme`, `prefers-reduced-motion` respecté, focus clavier visible,
  touche Entrée pour valider une réponse chiffrée, feuille de style d'impression pour les devoirs.
- Typographie : Archivo pour les titres, IBM Plex Serif pour le texte, IBM Plex Mono pour les
  unités et les équations.

Les 61 réponses chiffrées et le barème des deux devoirs ont été recalculés indépendamment du HTML.
Les banques de questions sont vérifiées automatiquement (index de bonne réponse dans les bornes,
pas de proposition en double, indice et corrigé présents partout) avant publication.
