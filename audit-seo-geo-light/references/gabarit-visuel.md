# Référence : gabarit visuel & pipeline de rendu

Le rendu **visuel est le défaut** (version texte sobre en option). Les solutions sont livrées graphiquement, pas en pavés. Cette bibliothèque est l'inventaire des composants d'un audit visuel abouti.

## Charte

- Utiliser la **charte graphique du consultant** (couleurs, logo, typographie). À défaut, une palette sobre : un bleu profond pour le texte fort et l'en-tête, un ambre pour les accents et les quick wins, un teal pour l'accent secondaire.
- Vert = « À faire » / opportunité ; rouge ou orangé = « À éviter » / piège / message-clé « À retenir ».
- Badges de sévérité : PROBLÈME (rouge) · AVERTISSEMENT (orange) · MOYEN (jaune) · OPPORTUNITÉ / FAIBLE (vert ou gris).
- Typographie lisible, paragraphes courts, beaucoup d'air. Aucun emoji.

## Bibliothèque de composants

| Composant | Où | Contenu type |
|---|---|---|
| Cartouche de couverture | Page 1 | Titre client + baseline, logo, « Audit réalisé par », tableau Date · Périmètre · CMS · Visibilité · Volets, confidentiel + sources |
| Encadré « EN BREF » à bandeau | Synthèse exécutive | 8 constats prioritaires numérotés (gras + description) |
| Bloc « Synthèse des solutions » | Après l'En bref | 8 réponses numérotées, une par constat, avec objectif mesurable |
| Cartes KPI en grille de 4 | Visibilité, social | Grande valeur + libellé + sous-légende (uniquement si la donnée est disponible) |
| Courbes commentées | Visibilité | Deux séries (marque vs organique, client vs concurrent), annotations fléchées, période datée |
| Anneau de proportion | Trafic de marque | Part de la marque dans le trafic |
| Tableau problème / gravité | Technique | Problème / Gravité (badge) / Nb URL / Action |
| Tableau cartographie de pages | Technique | URL / Rôle / Observation |
| Tableau constat → action | Schema, maillage | Dimension / Constat / Action |
| Matrice de requêtes | Mots-clés, benchmark | Requête / Volume / Concurrence / Position / Action (badges À créer, À optimiser, À laisser) |
| Doubles blocs comparatifs | Diagnostic | « Le correctif » / « Pourquoi ça compte » ; « Couvert » / « Hors périmètre » ; forces / faiblesses |
| Encadrés étiquetés (en marge) | Messages-clés | « À RETENIR », « LA BASCULE », « LA RÈGLE », « SYNERGIE » |
| Bloc « Limites de mesure » | Méthode | Transparence : accès manquants, faux positifs possibles, données non connectées |
| Arborescence ASCII | Architecture cible | Arbre indenté avec URL, profondeur ≤ 3, redirections 301 |
| Carte de cocon colorée | Cocons (post-audit) | Badge + page mère + guides filles + note de maillage (une couleur par cocon) |
| Bloc « Avant / après » monospace | Réorganisation de silo | Pseudo-schéma de structure |
| Matrice impact/effort | Priorisation | 4 quadrants, zone « Quick wins » surlignée, points colorés par priorité |
| Feuille de route 30/60/90 | Priorisation | 3 colonnes datées |
| Tableaux de phases 6 à 12 mois | Plan | Phase / Actions / Livrables / Objectifs mesurables (colonnes SEO + SEA si pertinent) |
| Grille « Si… / Alors » | Pilotage | Diagnostic conditionnel itératif |
| Cartes d'état | GEO / robots IA | Liste de crawlers avec « Autorisé » / « Bloqué » colorés |
| Bloc « Investissement » | Plan (option) | Trois tuiles (prestation / engagement / budget publicitaire) |
| Cartes KPI de pilotage | Pilotage | Impressions, position, CTR, signaux GBP, citations IA |
| Page de clôture | Fin | Carte de contact + appel à l'action + bloc « Sources / méthodologie » |
| Pied de page répété | Toutes les pages | Nom de l'audit + « Confidentiel » + pagination |

Codes couleur des cocons : une teinte par cocon (ambre = quick win, violet = identité de marque, teal = soutien du silo). Garder la cohérence badge ↔ carte.

## Règle d'or appliquée au rendu

Chaque recommandation = mini-bloc **Constat → Cause → Solution prête (encadré copiable : URL, H1, JSON-LD, title, méta) → Objectif mesurable / Validation.** Le code copiable est en bloc monospace, complet, non tronqué. Fournir le **JSON-LD complet et les title / méta prêts à coller**, pas seulement la description des propriétés.

## Pipeline

1. Livrable en **HTML autonome** (CSS intégré, fichier unique, images en data-URI si besoin).
2. Vérifier le rendu (aperçu).
3. Export **PDF** : Chromium ou Playwright en mode headless (`page.pdf()`), ou tout outil d'export PDF disponible.
4. **Versionner** (v1, v2…) ; le document est un outil de travail destiné à évoluer avec les premières données réelles.

## Structure type du livrable

Couverture → Synthèse exécutive (8 constats + solutions) → 15 sections (règle d'or partout, section 8 = module sectoriel, section 9 dosée) → le cas échéant, module de déploiement post-audit → page de clôture + sources.
