# Audit SEO + GEO : skill Claude (version light)

Un skill pour **Claude** qui produit un **audit SEO, GEO (optimisation pour les moteurs de réponse IA) et technique** à partir d'un simple nom de domaine, avec un plan d'action priorisé et une passe de diagnostic de **citabilité par les LLM**.

La version light travaille uniquement avec des **données publiques** : aucun accès à Semrush, à la Search Console, à GA4 ni à l'administration de la fiche Google Business Profile n'est nécessaire. Les points qui en demandent un sont signalés **[ACCÈS REQUIS]** et jamais inventés.

## Ce que le skill produit

- Un audit en **15 sections** : méthode, contexte, visibilité, technique, schema.org, architecture et maillage, volet sectoriel, SEO local, GEO, benchmark, réseaux sociaux, priorisation impact/effort, plan à 6 à 12 mois, pilotage.
- Une **synthèse exécutive** : 8 constats prioritaires + solutions point par point.
- Une **passe GEO / citabilité LLM** en 9 points de diagnostic et un plan d'exécution « sprint » d'une journée.
- Un **module de déploiement post-audit** : arborescence cible, cocons sémantiques, feuille de route, KPI.
- 4 **playbooks sectoriels** : artisan ou commerce local, B2B de niche, e-commerce, agence ou organisme de formation.

## Principes de méthode

- Chaque recommandation suit la chaîne **Constat → Cause → Solution prête à l'emploi → Objectif mesurable**.
- **Aucune donnée inventée** : ce qui n'est pas observable est marqué [À CONFIRMER] ou [ACCÈS REQUIS].
- **Vérification systématique** de chaque constat sur le site réel avant livraison ; ce qui est déjà bien fait est crédité comme une force.
- Une idée directrice : **le contenu citable ne sert à rien s'il n'est ni indexé, ni relié, ni sourcé.**

## Contenu du dépôt

```
README.md
LICENSE
ANNEXE-version-complete.md          Ce que couvre la version complète (avec accès)
audit-seo-geo-light/
  SKILL.md                          Le skill (trame, doctrine, passe GEO)
  references/
    archetypes-secteur.md
    collecte-donnees.md
    section-gbp-local.md
    gabarit-visuel.md
    plan-deploiement-post-audit.md
```

## Installation

- **Claude Code** : copier le dossier `audit-seo-geo-light/` dans `~/.claude/skills/` (ou dans `.claude/skills/` d'un projet).
- **Claude (application)** : importer le dossier compressé (fichier `.skill` ou `.zip`) depuis la section des skills, selon l'interface de votre version.

Puis demander, par exemple : « Fais l'audit SEO et GEO complet de example.com ».

## Version complète

Avec un outil de mesure SEO tiers, l'accès en lecture à la Search Console, à GA4 et à la fiche Google, une version complète du skill chiffre les sections marquées [ACCÈS REQUIS] et peut aller jusqu'à l'application des correctifs. Voir [ANNEXE-version-complete.md](ANNEXE-version-complete.md).

## Limites

Ce skill est une **méthode**, pas une garantie de résultat. Les objectifs chiffrés sont des cibles de pilotage. Les fonctionnalités des moteurs de recherche et des assistants IA évoluent vite : vérifier les points sensibles sur la documentation officielle avant d'affirmer quoi que ce soit à un client.

## Auteur

**Ludovic Scolard**, consultant SEO et GEO, fondateur de Sell Expert (Nancy, Grand Est), actif depuis 2016. Site : https://sell-expert.fr

## Licence

MIT, voir [LICENSE](LICENSE). Vous pouvez utiliser, adapter et redistribuer ce skill, en conservant la mention de l'auteur.
