# Annexe : la version complète du skill

La version **light** de ce dépôt travaille uniquement avec des **données publiques** (le site, les pages de résultats, les profils publics). C'est suffisant pour un premier audit sérieux, mais certaines sections ne peuvent pas être chiffrées sans accès. Elles sont marquées **[ACCÈS REQUIS]** dans le skill.

Quand le client donne un **accès en lecture seule** à ses outils, ou quand le consultant dispose d'un outil de mesure SEO, une **version complète** du skill est disponible. Elle fait plus de travail, avec des données réelles au lieu d'observations.

## Ce que l'accès aux outils change

| Source d'accès | Ce que la version complète en fait | Sections concernées |
|---|---|---|
| **Outil de mesure SEO tiers** (type Semrush) | Autorité du domaine, trafic estimé, mots-clés positionnés, domaines référents, courbes sur 24 mois, comparatif chiffré avec les concurrents, volumes et concurrence des mots-clés | 3, 4, 11, ciblage du plan de déploiement |
| **Google Search Console** | Impressions, clics, CTR et positions réels par requête et par page ; rapport « Fonctionnalités d'IA générative » (impressions des Aperçus IA et du Mode IA, ratio IA / Web, découpage en phases) ; indexation page par page ; requêtes longues de type prompt ; demandes d'indexation et état avant / après | 3, 4, 5, 10, 15, passe GEO (points A1, A2, A7), KPI |
| **Google Analytics 4** | Croisement GA4 × Search Console : comportement, conversions, part de la marque contre le métier, leads segmentés | 4, 15 |
| **Administration de la fiche Google Business Profile** | Vues, appels, itinéraires, requêtes de recherche de la fiche, complétude réelle, benchmark détaillé contre les fiches concurrentes | 9 |
| **Termes de recherche Google Ads** (si le client fait de la publicité) | Longue traîne réelle en B2B de niche, mots-clés négatifs, synergie SEA ↔ SEO | 8, 14 |
| **Accès au CMS** (mission de déploiement) | Corrections appliquées et re-vérifiées en direct (robots.txt, maillage, blocs sources et auteur, hub de contenu, schema), avec sauvegarde avant chaque écriture | passe GEO (plan d'exécution), plan de déploiement |

## Ce que la version complète ajoute en méthode

- Des **règles de collecte** détaillées pour chaque source ci-dessus, avec le croisement systématique des données.
- Un **module de déploiement** qui va jusqu'à l'application des recommandations et à leur vérification en direct.

## Comment l'obtenir

Contacter l'auteur (voir le README) en précisant les accès dont vous disposez ou que votre client peut accorder en lecture seule.

## Rappel de transparence

Aucune version de ce skill ne garantit un résultat. Les objectifs chiffrés sont des cibles de pilotage ; la vitesse d'exécution et l'autorité du site restent les deux facteurs déterminants.
