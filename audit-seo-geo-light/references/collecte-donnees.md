# Référence : méthode de collecte des données (depuis un simple domaine)

But : rendre l'audit **reproductible** à partir d'un seul nom de domaine, sans accès client. Toute donnée reportée est **sourcée et datée**. Ne jamais inventer un volume, une position ou un concurrent : si une donnée manque, la marquer **[À CONFIRMER]** ou **[ACCÈS REQUIS]** et la demander.

Accès à débloquer côté client pour passer à la version complète (lecture seule suffit) : Search Console, GA4, administration de la fiche Google Business Profile, et, si le consultant en dispose, un outil de mesure SEO tiers.

## Par section : où chercher (version light)

| Section | Source(s) publique(s) | Comment |
|---|---|---|
| Couverture / méthode | Site, WHOIS, détection du CMS | CMS, périmètre (langue, pays), volets couverts |
| 2. Contexte & cibles | Site, fiche Google Maps, LinkedIn, mentions légales, registres publics (data.gouv, Pappers) | Métier, cibles B2C ou B2B, zone, forme juridique, SIRET |
| 3. Visibilité organique | Pages de résultats Google et Bing, `site:domaine` | Relevé manuel de 10 à 20 requêtes cibles : position observée, type de résultat. Chiffres d'autorité et de trafic : **[ACCÈS REQUIS]** |
| 4. Trafic marque vs métier | Page de résultats (requête de marque, puis requêtes métier) | Lecture qualitative. Part de marque chiffrée : **[ACCÈS REQUIS]** |
| 5. Technique | Crawl type **Screaming Frog**, inspection navigateur, en-têtes HTTP | Titles, méta, H1, codes, profondeur, rendu JS, HSTS, CSP, X-Frame |
| 6. Schema | Inspection JSON-LD en direct (navigateur), test des résultats enrichis | Types présents et attendus, cohérence visible + géographie, avis auto-attribués, doublons de plugins |
| 7. Architecture & maillage | Crawl du menu et du sitemap, profondeur de clic | Silos, pivots, cannibalisation, fil d'Ariane, liens entrants éditoriaux |
| 8. Module sectoriel | Selon l'archétype | Voir `archetypes-secteur.md` |
| 9. GBP / local | Google Maps, page de résultats locale, fiches concurrentes | Voir `section-gbp-local.md` |
| 10. GEO / IA | `robots.txt`, requêtes dans les assistants conversationnels et Google | Crawlers IA autorisés, présence dans les réponses IA, citation-readiness |
| 11. Benchmark | Page de résultats, fiches concurrentes | Qui occupe la page, concurrents qui divisent leurs signaux sur deux sites. Comparatif chiffré : **[ACCÈS REQUIS]** |
| 12. Image / social | Profils sociaux, Meta Ad Library | Abonnés visibles, engagement visible, piliers, cohérence NAP et bio |
| 13-15. Priorisation / plan / KPI | Croisement des sections | Matrice impact/effort, KPI, satellites |

## Outils

- **Crawl on-site** (type Screaming Frog, version gratuite suffisante pour un petit site) : titles, méta et H1 manquants ou trop longs, doublons, profondeur, codes de réponse, images lourdes, rendu JS.
- **Inspection en direct (navigateur)** : extraire le JSON-LD (`script[type="application/ld+json"]`), lire les niveaux de titres (selon le thème, le titre de la page n'est pas toujours rendu en `<h1>` : vérifier en direct), vérifier le contenu injecté en JavaScript (non crawlable), lire les en-têtes de sécurité.
- **robots.txt et sitemaps** : blocages, segmentation ; **crawlers IA** (GPTBot, ClaudeBot, Google-Extended, PerplexityBot, CCBot, Bytespider…). Recommander au minimum d'autoriser Google-Extended.
- **GBP et page de résultats locale** : relevé de la fiche et de 3 à 5 fiches concurrentes (voir `section-gbp-local.md`).
- **Registres et transparence publicitaire** : data.gouv, Pappers (identité), Google Ads Transparency Center et Meta Ad Library (pression publicitaire concurrente).
- **Outil de mesure tiers (facultatif, si le consultant en dispose)** : toujours préciser la base géographique et la date du relevé. Ces outils peuvent annoncer un volume élevé là où la réalité (impressions de la Search Console) est marginale, et inversement afficher zéro sur des requêtes B2B pourtant travaillées : croiser avec la Search Console dès que possible.

## Deux règles de lecture importantes

- **Croiser GA4 × Search Console (section 4, version complète).** La Search Console donne requêtes et positions ; GA4 donne comportement et conversions. Isoler la marque du métier. Un audit sans ce croisement surestime la santé SEO. En version light, le dire explicitement dans les limites de mesure.
- **B2B de niche : lire la Search Console et les termes de recherche publicitaires, pas l'outil tiers.** Un volume affiché proche de zéro est normal (cycle long, faible volume, panier élevé) ; la vraie longue traîne est dans ces deux sources.

## Bloc « Limites de mesure » (transparence : à mettre dans la section 1 et au pied du document)

Lister honnêtement : absence d'accès à la Search Console, à GA4 et à la fiche GBP ; volumes non chiffrés ; faux positifs possibles des outils tiers ; compteurs sociaux non extractibles ; relevés de page de résultats faits depuis une session personnalisée ; sources et dates. C'est un marqueur de sérieux, pas un aveu de faiblesse.
