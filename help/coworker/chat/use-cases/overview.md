---
description: Parcourez les cas d’utilisation et les exemples d’invites de conversation des collègues, organisés par zone entre les informations sur les données, les audiences, les parcours et les opérations de la plateforme.
title: Cas D’Utilisation De La Conversation Avec Un Collègue
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 1284
ht-degree: 7%

---

# Cas d’utilisation de la conversation avec un collègue{#use-cases}

Le Chat Coworker vous permet d’interroger, d’analyser et d’agir sur vos données [!DNL Experience Platform] en utilisant un langage naturel au lieu de naviguer entre plusieurs interfaces utilisateur ou d’écrire des requêtes manuellement. Cette page répertorie les cas d’utilisation les plus utilisés par les utilisateurs et les utilisatrices, organisés par domaine de travail : informations sur les données, audiences, parcours, éléments fondamentaux et outils de sandbox. Chaque entrée comprend les compétences qu’elle appelle, les applications avec lesquelles elle fonctionne et des exemples d’invites que vous pouvez copier, adapter à vos propres données et affiner par la conversation.

## Informations sur les données

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| [Extraction des rapports et des mesures CJA](data-insights/analytics-chat.md) | Query CJA en temps réel pour extraire des mesures, des dimensions, des segments et des vues de données | `cja` | Customer Journey Analytics (CJA) | « Afficher les pages vues au cours des 30 derniers jours » · « Répertorier les segments principaux dans la vue de données principale » |
| Analyse comparative | Comparaison de mesures sur plusieurs canaux, périodes ou segments côte à côte | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | « Comparer le chiffre d’affaires par canal, mois après mois » · « À quoi ressemble la conversion entre appareils mobiles et ordinateurs de bureau ce trimestre ? » |
| Performances de la campagne | Mesurez les performances des campagnes, des canaux et des propriétés web sur une période donnée. | `cja`, `dx-api`, `knowledge-graph` | | « Quelles ont été les performances de nos campagnes web Acrobat le mois dernier ? » |
| Analyse funnel | Parcourez les entonnoirs de conversion à plusieurs étapes avec une restitution à chaque étape | `cja` | Customer Journey Analytics (CJA) | « Découvrez le funnel de passage en caisse » · « Afficher le funnel de conversion du PDP à l’achat » |
| Prévision | Prévision des valeurs des mesures futures en fonction des données CJA historiques | `cja` | Customer Journey Analytics (CJA) | « Sessions de prévision pour les 30 prochains jours » · « Sommes-nous sur la bonne voie pour atteindre notre objectif de revenus ? » |
| [Analyse de la cause première](data-insights/root-cause-analysis.md) | Découvrez pourquoi une mesure a changé : diagnostiquez les abandons, les pics et les anomalies | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | « Pourquoi les conversions ont-elles diminué la semaine dernière ? » · « Qu&#39;est-ce qui a provoqué la hausse des revenus le 15 janvier ? » |
| Résumés exécutifs et résumés des KPI | Produisez des résumés de performances prêts pour les parties prenantes, des recommandations normatives et des résumés de diapositives. | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | « Donnez-moi un résumé analytique du mois dernier » · « Créez un diaporama à partir des données de ce trimestre » |
| [Validation des données AA ↔ CJA](data-insights/data-validation-aa-cja.md) | Comparez, auditez et réconciliez les données entre Adobe Analytics et Customer Journey Analytics, en particulier lors de la mise à niveau d’Adobe Analytics vers Customer Journey Analytics | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | « Comparer ma suite de rapports AA à ma vue de données CJA » · « Valider les pages vues entre AA et CJA » |
| Séries chronologiques opérationnelles et analyse causale | Interroger et analyser les données historiques de séries temporelles pour les audiences, les jeux de données et les parcours avec attribution causale | `operational-stats-causal-analysis` | Toutes les applications éligibles | « Afficher les tendances de la taille de l’audience au cours des 90 derniers jours » · « Pourquoi ma ligne de jeu de données a-t-elle connu un pic le 3 mars ? » |
| Création de compétences CJA personnalisées | Transformer les modèles analytiques en compétences réutilisables et répétables qui persistent entre les sessions | `cja-skill-creator` | Customer Journey Analytics (CJA) | « Transformer cette analyse hebdomadaire du chiffre d’affaires en une compétence réutilisable » · « Enregistrer cette compétence en tant que compétence pour le compte rendu des performances mensuel de funnel » |

## Audiences

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| [Créer des audiences à partir du langage naturel](audiences/create-audience-from-natural-language.md) | Orchestrer la création d’audiences étape par étape avec l’approbation de l’utilisateur à chaque phase | `audience-creation-flow` | Real-Time CDP (RTCDP) | « Créer une audience d’utilisateurs qui ont acheté au cours des 30 derniers jours » · « Créer un segment pour les membres du programme de fidélité à forte valeur ajoutée en Californie » |
| Création de définitions PQL | Assembler les définitions d’audience à partir des propriétés XDM, des événements comportementaux ou des audiences existantes ; prendre en charge l’agrégation et les fenêtres temporelles | `segment-definition-assembly` | Real-Time CDP (RTCDP) | « Création d’un PQL pour les personnes qui ont consulté plus de 3 produits, mais ne les ont pas achetés » · « Ajout d’une période de 7 jours à ma condition d’événement » |
| Rechercher et trouver des audiences | Rechercher des audiences par identifiant, nom, recherche sémantique ; détecter les doublons et analyser les chevauchements | `audience-search` | Real-Time CDP (RTCDP) | « Rechercher toutes les audiences de fidélité » · « Existe-t-il un doublon de mon segment « Acheteurs de vacances » ? » |
| Estimer la taille de l’audience | Estimer la portée du profil pour une expression PQL à l’aide de l’API de prévisualisation Adobe Experience Platform avec interrogation | `audience-size-estimate` | Real-Time CDP (RTCDP) | « Quelle est la taille de cette audience ? » · « Estimer la portée de cette expression PQL » |
| Cascade de taille d’audience | Décomposer un PQL en sous-prédicats et montrer comment chaque condition contribue à la taille finale de l’audience | `audience-size-waterfall` | Real-Time CDP (RTCDP) | « Montrez-moi la cascade pour ce PQL » · « Déterminez comment chaque condition réduit l’audience » |
| Découvrir les champs XDM pour le ciblage | Rechercher des champs par nom, description ou valeur de données ; voir où ils vivent et où ils sont déjà utilisés | `field-discovery` | Real-Time CDP (RTCDP) | « Quels champs puis-je utiliser pour cibler les clients fidèles ? » · « Rechercher les champs liés à l&#39;historique des achats » |
| Publier/enregistrer des audiences | Conservez les définitions d’audience dans Experience Platform Segmentation Service avec les conventions de nommage et les contrôles de conformité. | `audience-publish` | Real-Time CDP (RTCDP) | « Enregistrer ceci en tant que brouillon » · « Publier l’audience nommée « Acheteurs de ventes printanières » » |

## Parcours

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| [Créer des parcours à partir du langage naturel](journeys/create-journey-from-natural-language.md) | Orchestrer la création de parcours dans AJO à partir d’une invite de texte ou d’une image/d’un diagramme de flux chargé | `journey-create` | Adobe Journey Optimizer (AJO) | « Création d’un parcours de bienvenue qui envoie un e-mail après l’inscription, attend 3 jours, puis envoie un suivi » · « Création d’un parcours à partir de cette image de diagramme de flux chargée » |
| Analyse des conflits de parcours | Détecter les chevauchements d’audience, les collisions planifiées et les problèmes de déduplication entre les parcours actifs | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | « Mon parcours d’abandon de panier est-il en conflit avec d’autres parcours ? » · « Vérifier le chevauchement des audiences entre mes parcours actifs » |
| Analyse des abandons de parcours | Identifiez où et pourquoi les clients abandonnent au cours d’un parcours et détectez les comportements générateurs de désengagement | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | « Où les gens décrochent-ils dans mon parcours de réengagement ? » · « Quels sont les nœuds du parcours X qui ont les retombées les plus importantes ? » |
| Analyse des erreurs d’action personnalisée | Identifiez le moment où les actions personnalisées échouent ou le pic des taux d’erreur dans un parcours, et diagnostiquez les causes profondes avant que les échecs ne se transforment en perturbations plus larges | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | « Pourquoi les actions personnalisées échouent-elles dans mon parcours d’inscription à la fidélité ? » · « Afficher le taux d’erreur de l’action personnalisée ExternalPush dans mon parcours de bienvenue ». |
| [Créer, modifier et gérer des défis de fidélité](journeys/create-loyalty-challenge.md) | Simplifier et accélérer la gestion des programmes de fidélité | `loyalty` | Adobe Journey Optimizer (AJO) | « Créez un défi pour encourager vos membres à essayer une nouvelle boisson saisonnière » · « Montrez-moi les défis de fidélité avec les taux de décrochage les plus élevés. » |

## Éléments fondamentaux

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Connaissances et documentation du produit | Répondez à des questions relatives à l’utilisation, à la conception, au dépannage et aux bonnes pratiques à partir de la documentation Adobe officielle | `product-knowledge` | Toutes les applications éligibles | « Comment configurer une destination de diffusion en streaming ? » · « Quelle est la différence entre la segmentation par lots et en flux continu ? » |
| Requête sur les entités Experience Platform / Journey Optimizer | Servir de point d’entrée principal pour les questions sur les entités de votre plateforme ; acheminer vers KG, la découverte de champs ou les API selon les besoins | `operational-insights` | Toutes les applications éligibles | « De combien de jeux de données dispose-t-on ? » · « Afficher tous les parcours actifs » · « Répertorier mes destinations » |
| Requêtes du graphique de connaissances | Nombre d’agrégats, jointures d’entités croisées, recherches de relations et exploration des métadonnées via des requêtes SQL uniques | `knowledge-graph` | Toutes les applications éligibles | « Quelles audiences utilisent ce jeu de données ? » · « Afficher les relations entre les schémas et les jeux de données » |
| Opérations de l’API Experience Platform / Journey Optimizer / Customer Journey Analytics | Fournir une passerelle d’API directe pour les mutations, les contrôles d’état en temps réel et les types d’entités qui ne figurent pas dans le graphique de connaissances | `cxo-api` | Toutes les applications éligibles | « Supprimer le jeu de données X » · « Vérifier le statut de mon traitement d’ingestion par lots » |
| Résolution d’entité et liaison | Utilisez la recherche sémantique et lexicale pour résoudre les mentions d’entité sur les entités Experience Platform réelles et découvrir les champs XDM. | `entity-linking` | Adobe Experience Platform | « Résoudre les « Acheteurs de vacances » sur une audience réelle » · « Me trouver des champs liés à l’historique des achats » |
| Gestion des compétences personnalisées | Enregistrer, modifier ou supprimer les compétences réutilisables détenues par l’utilisateur qui persistent entre les sessions | `manage-skill` | Toutes les applications éligibles | « Enregistrer ce workflow en tant que compétence » · « Supprimer ma compétence de rapport hebdomadaire » · « Transformer ceci en une compétence réutilisable » |

## Outil Sandbox

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| [Déplacement d’objets dans des sandbox](/help/agents/sandbox-tooling.md) | Migrez facilement les schémas, les audiences et d’autres configurations d’objet dans les sandbox, avec des dépendances résolues automatiquement | `sandbox-tooling-workflow` | Adobe Experience Platform | « Déplacer le schéma Luma Loyalty Members Platinum du sandbox actuel vers le sandbox de production » · « Promouvoir l’audience des membres du programme de fidélité Gold des États-Unis vers l’étape » |
