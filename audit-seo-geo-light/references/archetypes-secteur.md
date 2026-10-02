# Référence : playbooks sectoriels (les 4 archétypes)

La trame de `SKILL.md` reste ; la **section 8 (volet stratégique)** et le **dosage des sections 9 à 11** changent selon l'archétype. Les exemples ci-dessous sont **fictifs ou génériques** et servent à illustrer la méthode.

---

## A. Artisan / commerce local (exemple : artisan du bâtiment, métier de pose ou de rénovation)

**Enjeu central : le SEO local générique est souvent vacant.** Tous les acteurs partent quasiment de zéro ; le premier à publier des pages « [métier] + ville » propres, balisées `LocalBusiness`, avec un flux d'avis actif, prend la page de résultats.

- **Section 8 = pages de service géolocalisées** : une page par prestation, croisée avec la ville (ex. « [prestation] [ville] »). Le plafond de trafic est le nombre de pages de service ; chaque page peut faire bouger l'aiguille.
- **Pages villes** en déclinaison, **conditionnées par les données de la Search Console** (**[ACCÈS REQUIS]**, sinon relevé de la page de résultats) et par une décision géographique explicite, pour éviter la cannibalisation entre villes qui se recouvrent.
- **Architecture à double public sur un domaine unique** : espace B2C (moteur SEO transactionnel) et espace professionnel B2B compact (prescripteurs, conversion sur recommandation). Un domaine unique concentre 100 % des signaux, à l'inverse d'une stratégie à deux sites qui divise les liens entrants.
- **Schema** : `LocalBusiness` (sous-type métier le plus précis disponible) + `Service` + `Review` / `AggregateRating` si les avis sont réels et éligibles. Un `Organization` générique est une opportunité manquée.
- **Couche locale = section 9 maximale** (voir `section-gbp-local.md`) : NAP cohérent partout, GBP avec catégorie métier, photos géolocalisées et zone d'intervention, avis (objectif chiffré sur 90 jours), citations dans les annuaires métier et les fédérations professionnelles.
- **E-E-A-T de terrain** : fiches chantier ou réalisation documentées (photos, matériaux, contraintes, avant/après), témoignages de prescripteurs, mentions des labels, assurances et normes du métier.
- **UX mobile locale** : barre fixe « Appeler / Devis », double appel à l'action d'orientation dès l'accueil, bloc d'avis Google en en-tête.
- **Modèle de pondération d'une page de service (indicatif)** : accroche 10 % · preuves 30 % · réassurance 25 % · process 20 % · conversion 15 %. « Convaincre d'abord, convertir ensuite. »
- **Cohérence sémantique** : libellé de menu, URL et contenu alignés (éviter un menu « Nos revêtements » qui pointe vers une URL au nom d'un autre sujet).

---

## B. B2B de niche / multilingue (exemple : bureau d'études ou prestataire technique)

**Enjeu central : « tout est là, rien n'est branché ».** Un site riche, dont la couche dans la langue principale est mal reliée et invisible des moteurs de réponse. Un volume d'outil proche de zéro est normal : la demande se lit dans la Search Console et dans les termes de recherche des campagnes publicitaires.

- **Section 8 = rebranchement multilingue + arborescence par gamme ou service** : corriger les ancres qui pointent vers une autre langue (tableau de correspondance destination actuelle → équivalent dans la langue principale) ; mapper chaque service métier à un cluster de requêtes puis à une page cible dédiée, plus une requête « chapeau » du métier.
- **Cohérence géographique du schema** : vérifier qu'aucun JSON-LD ne déclare une entité d'un autre pays (organisation étrangère, zone géographique ou FAQ dans une autre langue) sur la couche principale. Déclarer l'établissement réel.
- **Cocon expert « normes et référentiels »** : organiser les articles techniques autour des normes et référentiels du métier. C'est le contenu citation-ready et le signal d'expertise.
- **Cibles décideurs, cycle long, panier élevé, faible volume** : objectiver la longue traîne via la Search Console et les termes publicitaires (**[ACCÈS REQUIS]**), pas via un outil tiers. Utiliser le vocabulaire de niche pour les title, H1 et mots-clés négatifs.
- **Références prestigieuses** (grands comptes, ouvrages emblématiques) comme signaux d'autorité.
- **Schema** : `Organization` de l'établissement réel + `Service` ; articles techniques proches d'un usage `TechArticle`.
- **Section 9 (local) légère** : une page de contact dans la langue principale avec NAP, formulaire et carte (souvent en 404), fiche GBP mono-établissement à revendiquer ; pas de démultiplication de pages villes.
- **Brique SEA complémentaire** (section 14) : la publicité comble le temps que le SEO s'installe ; une campagne de recherche, des groupes d'annonces par service, une liste de négatifs, une page d'atterrissage avec formulaire, une synergie SEA ↔ SEO (les termes de recherche payants nourrissent le plan SEO).

---

## C. E-commerce direct au consommateur (exemple : boutique en ligne d'habillement ou d'équipement)

**Enjeu central : un catalogue à plat sans signal thématique.** Structurer proprement autour d'un pivot lexical prouvé et de cocons éditoriaux. (Détail complet dans `plan-deploiement-post-audit.md`.)

- **Pivot lexical prouvé par les volumes** : choisir, entre deux synonymes, celui que les internautes tapent réellement (exemple fictif : synonyme A à 2 900 recherches par mois contre synonyme B à 70), puis aligner tout le champ lexical dessus et en faire l'épine dorsale d'un silo commercial. Volumes **[ACCÈS REQUIS]** à un outil tiers.
- **Section 8 = silos produits + cocons éditoriaux** : deux silos piliers avec sous-catégories cohérentes ; un espace éditorial qui héberge les cocons ; catégories chapeau evergreen **au-dessus** de l'existant (on ne casse rien).
- **Cocons** = page mère (terme large) + guides filles de longue traîne « citation-ready » (définition courte + étapes numérotées `HowTo` + mini-tableau « quel cas pour quel usage »).
- **Pièges des CMS e-commerce** : les produits des sous-catégories ne remontent pas toujours au parent sans réglage ; supprimer les préfixes d'URL parasites des catégories et produits ; une collection n'est pas une catégorie taxonomique (canonique vers la catégorie, texte unique sur la collection) ; facettes en `noindex`.
- **Schema** : `Product` + `Offer`, `CollectionPage` + `ItemList`, guides en `Article` ou `HowTo`.
- **Section 9 (local) = notoriété seulement** : GBP de marque, page locale et liens locaux comme signal de confiance et d'E-E-A-T, pas comme silo de conversion. Attention au piège d'intention locale (un mot local peut désigner autre chose que ce que vend la boutique, par exemple la seconde main pour un vendeur de neuf).

---

## D. Agence / organisme de formation (exemple : agence de communication ou de marketing qui forme)

**Enjeu central : deux activités = deux silos à terrains opposés.** L'agence se joue en local (une ville qui a du volume), la formation en national (les requêtes « formation + thème » tombent à zéro dès qu'on ajoute une ville).

- **Section 8 = double silo** :
  - *Silo agence (local)* : page pivot dédiée sur « agence [métier] [ville] » ; décharger l'accueil, qui garde le positionnement large et la marque. `ProfessionalService` ou `LocalBusiness`.
  - *Silo formation (national)* : catalogue pivot par thème (une page = une formation = une requête nationale) ; ciblage par **financement** (compte personnel de formation, opérateurs de compétences, distanciel, éligibilité à la certification), jamais « à [ville] » ; attaquer d'abord les **niches sectorielles à faible concurrence** (formation pour un métier précis) avant les requêtes disputées. `Course` / `EducationalOccupationalProgram` (organisme, modalité, public, certification).
- **`FAQPage`** sur les pages de services qui ont déjà une FAQ non balisée (gain direct pour les Aperçus IA).
- **E-E-A-T par la preuve** : certification, ancienneté, études de cas clients avant/après, coulisses de formation, avis collectés après chaque prestation ET après chaque formation.
- **Capture d'intention commerciale** : contenus « combien coûte / tarifs et prestations » reliés aux pages de services.
- **Le social comme preuve d'expertise** : LinkedIn ou YouTube pour une cible B2B ou collectivités ; réutiliser le contenu de formation en social pour générer des demandes finançables.
- **Angle GEO différenciateur** : un organisme certifié qui forme au GEO occupe un positionnement que ses concurrents locaux n'ont pas.
- **Section 9 (local)** de poids moyen : NAP complet dans le pied de page de tout le site, carte Google sur la page de contact, GBP à 100 % (catégories « agence » et « centre de formation »), collecte systématique d'avis ; indicateurs locaux (appels, itinéraires, avis) suivis à part des demandes de formation.

---

## Règle transverse

Quel que soit l'archétype : la trame, la règle d'or, la doctrine et le rendu visuel ne changent pas. Seuls changent le **volet stratégique (section 8)**, le **dosage de la couche locale (section 9)**, les **types de schema** et l'**angle des cocons**. En cas de doute sur l'archétype, trancher d'abord : *le local est-il un silo de conversion ou un levier de notoriété ?* et *la demande est-elle mesurable dans un outil tiers ou seulement dans la Search Console et les termes publicitaires ?*
