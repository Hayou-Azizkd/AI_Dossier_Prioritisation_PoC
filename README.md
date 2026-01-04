# AI Dossier Prioritization — Proof of Concept (PoC)
**Responsible AI for Decision Support**

## 1. Contexte du projet
Les organisations publiques traitent quotidiennement un grand volume de **dossiers de demandes administratives**.  
Ces dossiers varient en urgence, en complexité et en impact potentiel, ce qui rend leur **priorisation** difficile et chronophage.

Ce projet explore comment l’**intelligence artificielle** peut **soutenir** les équipes administratives dans la priorisation des dossiers, **sans automatiser la décision**, et en maintenant un **contrôle humain explicite**.

---

## 2. Problème métier
Les équipes font face à plusieurs enjeux :
- Identifier rapidement les dossiers potentiellement urgents ou bloqués
- Prioriser l’attention humaine de manière cohérente et transparente
- Éviter une surcharge liée au traitement séquentiel des demandes
- Maintenir des pratiques responsables et auditables

L’objectif n’est **pas** de remplacer les agents humains, mais de **les aider à orienter leur analyse**.

---

## 3. Objectif de la preuve de concept (PoC)
Ce PoC vise à explorer comment un **agent IA** peut analyser :
- une **description textuelle** de dossier,
- des **métadonnées simples** (date, catégorie, urgence déclarée),

afin de produire une **priorisation indicative** des dossiers, accompagnée d’une **justification explicable**.

Le PoC permet d’évaluer la **faisabilité**, la **clarté** et les **limites** de cette approche dans un cadre d’aide à la décision.

---

## 4. Hypothèse du PoC
La combinaison d’une analyse textuelle simple et de métadonnées permet de générer une **priorité suggérée** utile pour guider l’analyse humaine, **sans déclencher de décision automatique**.

---

## 5. Périmètre du PoC

### Inclus
- Analyse de descriptions textuelles de dossiers
- Utilisation de métadonnées (date, catégorie, urgence déclarée)
- Production d’un **niveau de priorité suggéré** (Faible / Moyenne / Élevée)
- Génération d’une **justification textuelle**
- Validation finale par un humain (human-in-the-loop)
- Analyse des risques et limites (IA responsable)

### Exclu
- Décision automatisée
- Apprentissage supervisé complexe
- Optimisation de performance
- Déploiement en production
- Intégration à des systèmes réels

Le périmètre est volontairement limité afin de réduire les risques et de favoriser une évaluation éclairée.

---

## 6. Données utilisées
Dans le cadre de ce PoC, un **jeu de données synthétique** est utilisé afin d’illustrer la logique de priorisation.

Chaque dossier comprend :
- un identifiant
- une date de soumission
- une catégorie
- une urgence déclarée
- une description textuelle

L’objectif est de tester la **logique de raisonnement** et la **capacité d’explication**, non la performance sur des données réelles.

---

## 7. Approche IA proposée
L’agent IA repose sur une approche **simple et transparente**, combinant :
- des règles heuristiques explicites,
- des signaux issus du texte (mots-clés),
- des métadonnées temporelles.

Cette approche s’inscrit dans une logique **agentic AI**, où le système :
- perçoit des informations,
- raisonne sur une priorisation,
- propose une recommandation,
tout en laissant la **décision finale à l’humain**.

Aucune optimisation avancée n’est recherchée à ce stade.

---

## 8. Sorties du PoC
Pour chaque dossier, l’agent produit :
- une **priorité suggérée** (Faible / Moyenne / Élevée),
- une **justification synthétique** expliquant les facteurs pris en compte,
- un **avertissement explicite** rappelant le caractère indicatif de la recommandation.

---

## 9. IA responsable — Principes appliqués

### Rôle de l’humain
Le système fonctionne exclusivement comme un **outil d’aide à la décision**.  
La validation, la correction et l’interprétation finale relèvent de l’agent humain.

### Transparence et explicabilité
Les règles de priorisation sont explicites et les justifications sont fournies pour chaque recommandation.

### Risques identifiés
- Surévaluation de l’urgence déclarée par certains usagers
- Biais liés au style d’écriture des descriptions
- Couverture incomplète des signaux textuels

### Mesures de mitigation
- Human-in-the-loop obligatoire
- Justification systématique des recommandations
- Absence de toute décision automatisée

---

## 10. Conclusion du PoC
Cette preuve de concept montre qu’il est possible de proposer une **priorisation indicative** de dossiers administratifs à partir de données simples, tout en respectant des **principes d’IA responsable**.

Le PoC constitue une base de réflexion utile pour :
- orienter l’attention humaine,
- améliorer la cohérence du traitement,
- explorer des usages de l’IA à faible risque.

**Décision PoC : poursuivre avec ajustements (GO conditionnel)**

---

## 11. Prochaines étapes possibles
- Enrichissement des données (historique, délais de traitement)
- Tests sur des cas réels anonymisés
- Analyse plus fine des biais
- Encadrement formel des usages et de la gouvernance
