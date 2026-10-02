---
name: plan-deploiement-post-audit
description: Brique réutilisable du skill audit-seo-geo-light. Transforme les constats d'un audit en plan de déploiement personnalisé (arborescence, cocons sémantiques, feuille de route, KPI).
type: module-skill
version: 1.0
---

# Module : plan de déploiement post-audit

> Répond à la question « **et après l'audit ?** ». L'audit dit ce qui ne va pas ; ce module dit **où l'on va (architecture cible) et comment on y va (cocons, feuille de route, pilotage)**, à partir des recommandations vues avec le client.
>
> Se branche après le tronc d'audit. Livrable : document de travail versionné, visuel, autonome, exportable en PDF.

---

## 1. Principe : tronc commun + emplacements personnalisés

La force du modèle : **la personnalisation est logée dans des emplacements fixes**. Le squelette (les 11 sections, la bibliothèque de composants, la doctrine) ne bouge pas ; on le remplit avec les données réelles du client issues de l'audit. Chaque section pose une **question invariante** ; la réponse est propre au client.

| # | Section (invariante) | Question à laquelle elle répond | Remplie avec (donnée client) |
|---|---|---|---|
| — | En-tête + En bref | Où en est-on, quelles décisions clés ? | 5 à 6 puces = les arbitrages du dossier |
| 1 | Diagnostic & différenciation | Pourquoi ce positionnement plutôt qu'un autre ? Quelle niche ? | Pivot lexical prouvé par les volumes + 1 angle principal + 2 alternatifs |
| 2 | Concurrence nationale & locale | Contre qui ne peut-on pas gagner de front, où est la brèche ? | Page de résultats (têtes de liste) + acteurs locaux + tableau de requêtes locales |
| 3 | Ciblage SEO & mots-clés | Quelle page vise quoi ? | Tableau page cible / mot-clé / volume / concurrence / longue traîne + glossaire d'entités |
| 4 | Arborescence cible | À quoi ressemble la structure idéale ? | Arbre ASCII : silos, sous-catégories, espace éditorial, page locale |
| 5 | Détail des silos & URL | Quelle URL, quel H1, quelle cible par page ? | Tableaux par silo + règle d'URL |
| 5 bis | Regrouper l'existant | Comment atteindre la cible sans tout casser ? | Catégories chapeau evergreen au-dessus de l'existant |
| 6 | Cocons sémantiques | Comment capter la longue traîne et nourrir les silos ? | Page mère + guides filles « citation-ready », par cocon |
| 7 | Couche SEO local | Le local est-il un levier, et lequel ? | GBP + page locale + liens locaux, **dosé selon le métier** |
| 8 | Règles de maillage interne | Comment circule la popularité ? | Doctrine fixe + « À faire / À éviter » adaptés |
| 9 | Technique, schema & CMS | Quoi baliser, quoi corriger côté technique ? | Tableau élément / recommandation + types de schema par page |
| 10 | Feuille de route | Dans quel ordre, sur combien de temps ? | Plan semaine par semaine + « en continu » |
| 11 | KPI & pilotage | Comment mesurer et itérer ? | 4 KPI + plan d'itération conditionnel + 2 contenus satellites suivants |

**Règle d'or (héritée du skill).** Chaque recommandation = **Constat → Cause → Solution prête à l'emploi (copiable : URL, H1, JSON-LD, chapô…) → Critère de validation.** On assume un document plus long : c'est ce qui rend le client autonome.

---

## 2. La trame détaillée (le tronc)

### En-tête + « En bref »
En-tête aux couleurs du consultant : sur-titre (« [CABINET] · ARCHITECTURE SEO »), titre du client, sous-titre (la thèse en une ou deux phrases), ligne méta (domaine · localisation · secteur · marché · « Document de travail v[n] »).
Puis un encadré **« En bref »** : 5 à 6 puces qui donnent les arbitrages majeurs sans lire tout le document (le pivot, les silos, les cocons, le levier local, la règle d'or du cocon).

### 1. Diagnostic & différenciation
- État actuel en 3 à 4 phrases (structure, signaux thématiques, pages d'atterrissage par intention).
- Bloc **« Pourquoi X plutôt que Y »** : l'arbitrage lexical justifié par les volumes comparés (exemple fictif : synonyme A à 2 900 contre synonyme B à 70). *La donnée décide, pas l'intuition.* Volumes **[ACCÈS REQUIS]** à un outil tiers ; sans outil, justifier par l'observation de la page de résultats et le marquer **[À CONFIRMER]**.
- **Recommandation de niche** : 1 angle principal + 2 alternatifs, pour ranker sur la longue traîne plutôt que d'affronter les géants sur les requêtes génériques.
- Doubles encadrés : **« Preuves à intégrer »** (signaux E-E-A-T : guides, page concept, fiches riches en matière) / **« Friction actuelle »** (ce qui bloque aujourd'hui).

### 2. Concurrence nationale & locale
- **National** : qui occupe la première page sur les requêtes génériques (marques, places de marché, pure players). Conclusion type : la brèche est la longue traîne et l'éditorial.
- **Local** : acteurs physiques et annuaires qui occupent la page de résultats + tableau de requêtes locales (requête / volume / concurrence / **lecture stratégique**).
- Encadré **« Lecture stratégique »** : quel mot local est un piège d'intention et sur quoi capitaliser à la place.

### 3. Ciblage SEO & mots-clés
- Tableau **page cible / mot-clé principal / volume / concurrence / secondaires et longue traîne**, marqué par type (pilier, sous-catégorie, cocon).
- **Glossaire d'entités à couvrir** : 20 à 30 entités (marques, matières, normes, concepts, lieux, termes métier) à intégrer naturellement dans les textes pour bâtir l'autorité thématique.
- Note de méthode : source et date des volumes, « concurrence 0-1 = indice », rappel que le business à court terme se joue sur la longue traîne.

### 4. Arborescence cible
Arbre **ASCII** lisible : silos piliers, sous-catégories avec URL, espace transversal (collections, offres), espace éditorial (le hub qui héberge les cocons), page locale optionnelle, pages de service (contact, compte, mentions légales). Indiquer la **profondeur maximale** (règle : 3 clics au plus de l'accueil à une fiche).

### 5. Détail des silos & URL
Par silo : page pilier (URL + H1 + rôle), puis tableau **sous-catégorie / URL / H1 / cible principale**. Encadré **« Règle d'URL »** : minuscules, tirets, pas de mot vide, slugs alignés sur le silo, suppression des préfixes parasites du CMS.

### 5 bis. Regrouper l'existant (catégories chapeau)
Le principe **« on ne casse rien »** : créer des catégories chapeau evergreen (les mots réellement tapés) **au-dessus** de l'existant, qui deviennent des sous-catégories. Tableau **catégorie chapeau (à créer) / regroupe (catégories actuelles) / cible et volume**. Bilan concret : combien de vraies catégories chapeau à créer. Encadrés **« pièges CMS »** (les produits des sous-catégories ne remontent pas toujours au parent sans réglage ; une collection n'est pas une catégorie taxonomique).

### 6. Cocons sémantiques
Définition en tête : *un cocon = une page mère (pilier), des pages filles qui répondent chacune à une sous-intention précise, un maillage contextuel qui fait circuler la popularité.* La mère vise le terme large ; les filles captent la longue traîne et poussent la popularité vers la mère et vers les pages à convertir.
Puis **une carte colorée par cocon** : badge (« Cocon 1 : [nom] »), accroche (quick win / identité de marque / soutien du silo), **page mère** (titre + URL), liste des **guides filles** avec volumes, note **« Maillage »** (vers quoi renvoie chaque guide) et format **« citation-ready »** : définition courte + étapes numérotées (schema `HowTo`) + mini-tableau « quel cas pour quel usage ».

### 7. Couche SEO local
Encadré contextuel. Trancher d'abord : *le local est-il un silo de conversion ou un levier de notoriété et de confiance ?* Puis, selon le métier :
- **Google Business Profile** : catégorie juste, zone de service, photos, publications régulières ; souvent le levier n°1.
- **Page locale** balisée `LocalBusiness` (+ `OnlineStore` si e-commerce) racontant l'ancrage, la personne, l'histoire.
- **Liens et citations locaux** : presse et blogs locaux, annuaires, places de marché « acheter local », partenariats.
- **NAP cohérent** (nom, adresse, téléphone identiques sur le site, la fiche GBP et les annuaires).

### 8. Règles de maillage interne
Doctrine fixe : (1) liens contextuels dans le corps, ancres descriptives, pas de « cliquez ici », pas de menu seul ; (2) sens de circulation mère ↔ filles, filles → une ou deux sœurs proches, pas de saut d'un cocon à l'autre ; (3) du contenu vers le produit ou la prestation ; (4) le pilier est la plaque tournante ; (5) fil d'Ariane systématique (`BreadcrumbList`). Doubles encadrés **« À faire / À éviter »**.

### 9. Technique, schema & CMS
Tableau **élément / recommandation** : structure d'URL, fil d'Ariane, pages catégories (`CollectionPage` + `ItemList`, texte unique de 120 à 250 mots), fiches produit (`Product` + `Offer`), guides (`Article` / `HowTo`), page locale (`LocalBusiness` / `OnlineStore` / `Organization`), gestion des collections vs catégories (canonique, anti-duplication), facettes et filtres (`noindex` ou paramètres), sitemap et menu.

### 10. Feuille de route de mise en œuvre
Plan **semaine par semaine** (semaine 1 = fondations + vocabulaire ; puis un cocon par semaine, en commençant par le quick win ; local et schema aux bons jalons) + une ligne **« en continu »** (enrichir les fiches, ajouter des guides, obtenir avis et liens). Chaque semaine = un objectif concret et un livrable.

### 11. KPI & pilotage
Quatre cartes KPI (impressions par silo ou cocon, position moyenne sur les cibles, CTR par page, vues et clics GBP : **[ACCÈS REQUIS]** pour les données de la Search Console et de la fiche). Puis **plan d'itération conditionnel** : « si les impressions montent mais le CTR est faible → retravailler title et méta » ; « si la position stagne en page 2 → renforcer le maillage et enrichir le contenu » ; « si peu d'impressions → vérifier l'indexation, la profondeur, les liens depuis le cocon ». Révision tous les 30 jours. Finir par **deux contenus satellites suivants** (extension des clusters).

### Pied de page
Note de méthode : source et date des données, nature des volumes (estimations), version, « à faire évoluer avec les premières données réelles ».

---

## 3. Bibliothèque de composants visuels

Réutiliser ces blocs pour tout dossier (voir `gabarit-visuel.md` pour l'inventaire complet). Le rendu visuel est le défaut ; une version texte sobre reste possible.

| Composant | Quand l'utiliser | Contenu type |
|---|---|---|
| En-tête | Ouverture | Sur-titre, titre client, thèse, ligne méta |
| Encadré « En bref » | Juste après l'en-tête | 5 à 6 puces d'arbitrages |
| Sommaire | Avant le corps | Liste numérotée des sections |
| Tableau volume / concurrence | §2, §3 | Requête / volume / concurrence / lecture |
| Arborescence ASCII | §4 | Arbre indenté avec URL |
| Carte de cocon colorée | §6 | Badge + mère + filles + maillage (une couleur par cocon) |
| Double encadré « À faire / À éviter » | §1, §8 | Deux colonnes vert / rouge |
| Encadré « piège » | §5 bis, §7 | Fond d'alerte, titre gras + explication + chemin |
| Encadré « lecture stratégique » | §2 | Fond neutre, l'arbitrage en clair |
| Frise « semaine par semaine » | §10 | Une ligne = une semaine = un objectif |
| Cartes KPI | §11 | Quatre tuiles titre + sous-titre |
| Pied de page méthodologique | Fin | Source, version, réserve sur les données |

---

## 4. Protocole de personnalisation

### Phase 0 : entrées (issues de l'audit, à ne pas recollecter)
Rassembler avant de rédiger : pivot lexical retenu et volumes comparés ; niche (1 + 2 angles) ; liste des silos et sous-catégories cibles ; 2 à 4 cocons (mère + filles + volumes) ; verdict sur la couche locale (levier ou non) et NAP ; stack technique (CMS, schema existant, pièges) ; contraintes business (marché, langue, saisonnalité).

### Remplissage
Parcourir les 11 sections dans l'ordre, en remplaçant chaque emplacement variable par la donnée du client. **Ne jamais livrer une section générique** : si une donnée manque, la marquer **[À CONFIRMER]** et la demander au client plutôt que d'inventer un volume ou un concurrent.

### Garde-fous qualité
- Règle d'or Constat → Cause → Solution prête → Validation sur chaque recommandation.
- Toute donnée chiffrée est sourcée et datée ; les incertitudes sont dites.
- Solutions livrées graphiquement (cartes, tableaux, arbres), pas en pavés.
- Réflexe GEO : format citation-ready des guides, `robots.txt` ouvert aux crawlers IA, vérification de la disponibilité des Aperçus IA dans le pays visé.

---

## 5. Adaptation par archétype (le squelette fléchit)

Le tronc reste ; le poids relatif des sections change selon le métier.

**E-commerce direct au consommateur.** Sections lourdes : 4 à 6 (arborescence, silos, cocons produits). Couche locale = levier de notoriété seulement. Schema : `Product` / `Offer` / `CollectionPage`. Enjeu CMS fort (catégories, canoniques, facettes).

**Artisan / commerce local.** La **couche locale (§7) devient centrale et non optionnelle** : GBP maximal, page locale forte, avis, NAP, liens locaux. Arborescence plus petite ; cocons = guides-services (« comment choisir… », « prix de… », « [service] à [ville] »). Schema `LocalBusiness` + `Service` prioritaires.

**B2B de niche / multilingue.** Cocons = contenu expert (normes, cas d'usage, comparatifs techniques). Arborescence par gamme ou application. Gérer le multilingue (hreflang, silos par langue). Local secondaire. Schema `Product` / `Organization` + éventuellement `TechArticle`. Cible = décideurs, cycles longs.

**Agence / formation.** Cocons = preuve d'expertise + capture d'intention commerciale (« formation X », « agence Y à Z »). Pages de prestations en `Service`, formation en `Course`. Avis et E-E-A-T déterminants. Local selon l'implantation. Feuille de route orientée acquisition et autorité.

---

## 6. Rendu & pipeline

HTML autonome → export **PDF** (Chromium ou Playwright en mode headless, ou tout outil d'export PDF). Toujours : « En bref » en tête, sommaire, pied de page de méthode et de version. Le document est un **outil de travail versionné** (v1, v2…) destiné à évoluer avec les premières données réelles.

---

## 7. Checklist de complétude du livrable

- [ ] En bref (5 à 6 arbitrages) + sommaire présents.
- [ ] Pivot et niche justifiés par des volumes sourcés et datés (ou marqués [À CONFIRMER]).
- [ ] Concurrence nationale ET locale traitées, avec lecture stratégique.
- [ ] Tableau de ciblage + glossaire d'entités (20 à 30).
- [ ] Arborescence ASCII avec URL et profondeur ≤ 3.
- [ ] Détail des silos et des URL + règle d'URL.
- [ ] Stratégie « regrouper l'existant » en cas de refonte d'un site vivant.
- [ ] 2 à 4 cocons en cartes, guides filles « citation-ready ».
- [ ] Couche locale dosée selon l'archétype.
- [ ] Règles de maillage + À faire / À éviter.
- [ ] Tableau technique et schema par type de page.
- [ ] Feuille de route datée + KPI + plan d'itération + 2 satellites.
- [ ] Chaque recommandation : Constat → Cause → Solution prête → Validation.
- [ ] Rendu visuel + export PDF + version + pied de page de méthode.
