---
description: Parcourez les cas d’utilisation et les exemples d’invites de conversation des collègues, organisés par zone entre les informations sur les données, les audiences, les parcours et les opérations de la plateforme.
title: Cas D’Utilisation De La Conversation Avec Un Collègue
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 9975595370bff328ea990f07ec3dbb85c17ee23b
workflow-type: tm+mt
source-wordcount: 3308
ht-degree: 6%

---

# Cas d’utilisation de la conversation avec un collègue{#use-cases}

Le Module de conversation des collègues vous permet d’interroger, d’analyser et d’agir sur vos données [!DNL Experience Platform] en utilisant un langage naturel au lieu de parcourir plusieurs interfaces utilisateur ou d’écrire des requêtes manuellement. Cette page répertorie les cas d’utilisation les plus utilisés par les utilisateurs et les utilisatrices, organisés par domaine de travail : informations sur les données, audiences, parcours, éléments fondamentaux et outils de sandbox. Chaque entrée comprend les compétences qu’elle appelle, les applications avec lesquelles elle fonctionne et des exemples d’invites que vous pouvez copier, adapter à vos propres données et affiner par la conversation.

>[!NOTE]
>
>Prochainement :
>
>De nouvelles fonctionnalités d’agence AEM via CX Enterprise Coworker, conçues pour vous aider à en faire plus, plus rapidement.
>
>Tous les clients éligibles auront accès aux fonctionnalités de l’agence Adobe Experience Manager dans Coworker, de manière progressive.
>
>Consultez également la section [IA dans AEM - Présentation des fonctionnalités d’agent dans AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview).

## Expérience de marque

| Exemple d’utilisation | Description | Compétence(s) | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Mise à jour des pages AEM | Effectuez des actions telles que la mise à jour, la suppression, le remplacement ou l’ajout d’éléments de contenu pour que les expériences restent exactes et à jour. Les entrées peuvent être en langage naturel ou des annotations visuelles telles que des PDF ou des captures d’écran. | `aem-sites-pages-update` | Adobe Experience Manager (AEM) - AEM Sites | Le &lt;URL> mettez à jour le titre en Hello World<br><br>le &lt;URL> modifiez le bouton « Prenez notre quiz du café » en une version plus attrayante<br><br>Mettez à jour &lt;URL> en fonction du fichier joint<br><br>le &lt;URL> Je souhaite ajouter une nouvelle section teaser au bas de la page à propos d’une promotion que nous organisons au mois d’août qui consiste à acheter une machine à café et à obtenir 2 sacs de café gratuits. Retrouvez également l’image d’amis buvant du café et utilisez-la dans le teaser |
| Mise à jour d’AEM en bloc | exécuter des actions en bloc sur plusieurs pages en même temps, telles que la suppression, le remplacement ou l’ajout d’éléments de contenu, pour que les expériences restent exactes et à jour. | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) - AEM Sites | sur &lt;chemin aem>, mettez à jour toutes les pages qui contiennent la copie « MyBarista\ » vers « BrewPass ». |
| Passer de Figma au fragment de contenu visuel | Importez des conceptions directement de Figma dans Adobe Experience Manager à l’aide du langage naturel. Cette compétence crée automatiquement le modèle de contenu, le fragment de contenu, les ressources et le modèle de visualisation requis, ce qui permet aux utilisateurs professionnels de passer de la conception au contenu prêt pour le web en quelques minutes, sans configuration manuelle. | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) - AEM Sites | Importer depuis &lt;Image_URL> |

| Exemple d’utilisation | Description | Compétence(s) | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Créer un formulaire | Générez un nouveau formulaire adaptatif à partir d’une description en langage clair, d’un brief joint, d’une image ou d’un PDF | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) - AEM Forms | « Créer un formulaire d’intégration d’employé »<br><br>« Créez un formulaire à l’aide du brief ci-joint (image ou pdf)« <br><br>« Créez un &lt;type de formulaire> formulaire adaptatif » |
| Formulaire de modification/mise à jour | Modifier un formulaire existant — ajouter/modifier des champs, ajuster une disposition simple, configurer des actions d’envoi ou appliquer des modifications à partir d’un document de directives joint | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | « Ajouter le champ Deuxième prénom sous le champ Prénom »<br><br>« Placez les champs Prénom et Nom dans une disposition à 2 colonnes, 50/50 »<br><br>« Configurez le formulaire pour envoyer des données à un point d’entrée REST »<br><br>« Mettez à jour ce formulaire pour qu’il corresponde au document d’instructions joint »<br><br>« Ajoutez le champ &lt;nom du champ> sous le champ &lt;champ existant> » |
| Ajouter une logique commerciale | Créez des règles simples, par exemple pour afficher ou masquer un champ en fonction de la valeur d’un autre champ | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) - AEM Forms | « Afficher le champ Société uniquement lorsque le type d’employé est Sous-traitant »<br><br>« Afficher le champ &lt;champ> uniquement lorsque &lt;autre champ> est &lt;valeur> » |
| Formulaire intégré | Placez un formulaire existant ou nouvellement créé sur une page AEM Sites désignée (prise en charge sur les pages Edge Delivery Services uniquement). | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) - AEM Forms | « Incorporer ce formulaire dans la page d’accueil de notre site »<br><br>« Incorporer ce formulaire dans &lt;page path> » |

**Informations connexes**

* [Fonctionnalités d’agent dans AEM : Expérience de marque - Production d’expérience - Sites](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

* [Fonctionnalités d’agent dans AEM : Expérience de marque - Production d’expérience - Forms](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### Développement

| Exemple d’utilisation | Description | Compétence(s) | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Gestion des pipelines Cloud Manager | Créer, exécuter et surveiller les pipelines AEM Cloud Manager, y compris les journaux, les artefacts, les variables et les paramètres | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | « Répertorier les pipelines pour les 12345 de programme »<br><br>« Quel est l’état de mon dernier pipeline ? » |
| Gestion des environnements Cloud Manager | Création, configuration et maintenance des environnements AEM Cloud Manager, y compris les RDE, les variables d’environnement, les journaux et les sauvegardes | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | « Répertorier mes environnements pour les 12345 de programme »<br><br>« Réinitialiser mon RDE » |
| Gestion des programmes Cloud Manager | Répertorier, inspecter et supprimer des programmes AEM Cloud Manager, y compris leurs pipelines et environnements | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | « Répertorier mes programmes Cloud Manager« <br><br>« Obtenir des détails sur les 12345 du programme » |
| Gestion des plannings de mise à jour des versions d’AEM | Configurez des heures creuses quotidiennes et des périodes sans mise à jour pour une maintenance automatisée et affichez les fenêtres de gel de code globales d’Adobe. | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | « Quelle est ma fenêtre d’heures creuses actuelle ? »<br><br>« Planifiez une période sans mise à jour du 20 décembre au 2 janvier » |

**Informations connexes**

* [Fonctionnalités des agents dans AEM : Expérience de marque - Développement](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### Intégration

| Exemple d’utilisation | Description | Compétence(s) | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Intégration guidée de bout en bout | Orchestre le cycle de vie complet de l’intégration, la sélection du référentiel, la délégation au dossier, la balise, les métadonnées, l’importation et la recherche des sous-compétences, si vous ne connaissez pas la tâche d’intégration spécifique dont vous avez besoin. | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) - AEM Assets | « Intégration de notre équipe à AEM Assets »<br><br>« Découvrez comment intégrer la gestion des ressources numériques AEM » |
| Conception et création de hiérarchies de dossiers | Recommande et crée des structures de dossiers évolutives dans AEM Assets (sous `/content/dam`) en fonction des besoins de l’entreprise ou des entrées CSV. | `aem-folder-management` | Adobe Experience Manager (AEM) - AEM Assets | « Recommander une structure de dossiers pour vos ressources marketing liées à votre style de vie »<br><br>« Créer des dossiers basés sur ce fichier CSV » |
| Conception et création de balises | Conçoit et crée des vocabulaires de balises contrôlés sous `/content/cq:tags` : espaces de noms, balises hiérarchiques et opérations de balises par lots. | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) - AEM Assets | « Concevoir une taxonomie de balises avec des espaces de noms pour nos catégories de produits »<br><br>« Importer des balises à partir de ce fichier CSV »<br><br>« Créer ces balises hiérarchiques dans AEM » |
| Création et affectation de formulaires de métadonnées | Conçoit et crée des formulaires de métadonnées personnalisés que les auteurs de contenu de l’interface utilisateur de création utilisent à partir d’un fichier CSV, d’un tableau, d’un document d’exigences ou d’une description, puis les affecte éventuellement à des dossiers. | `aem-metadata-form` | Adobe Experience Manager (AEM) - AEM Assets | « Créer un formulaire de métadonnées à partir de cette liste de champs »<br><br>« Affecter ce formulaire au dossier `campaigns` » |

**Informations connexes**

* [Fonctionnalités d’agent dans AEM : expérience de marque - intégration](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## Conseiller d’accès

### Découverte de contenu

| Exemple d’utilisation | Description | Compétence(s) | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Recherche par thème sémantique | Recherchez des ressources par concept, humeur ou thème visuel à l’aide de la correspondance sémantique optimisée par l’IA. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | « Retrouvez-moi des images de style de vie du café du matin » |
| Recherche par métadonnées personnalisées | Filtrez les ressources en fonction de champs de métadonnées personnalisés (par exemple, mélange de café, marque, niveau de rôti). | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | « Rechercher les ressources où `Coffee Blend` est `Morning Muse`« <br><br>« Obtenez-moi les ressources dont la licence n’a pas expiré »<br><br>« Recherchez les ressources dont le nom de campagne n’est pas défini (la propriété doit être indexée pour obtenir les résultats appropriés). » |
| Rechercher par statut de validation | Filtrez les ressources en fonction du statut d’approbation. Par exemple, le statut approuvé, en cours de révision, rejeté ou manquant. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | « Afficher toutes les ressources approuvées dans le dossier `Campaign` » |
| Recherche par dossier/chemin d’accès | Identifiez les ressources en interprétant les invites en langage naturel qui font référence aux noms de dossier dans AEM. Vous pouvez simplement mentionner le dossier dans leur invite, sans avoir à parcourir manuellement le référentiel, ce qui réduit considérablement le nombre de clics nécessaires pour localiser le contenu approprié. | `aem-assets-discovery` | Adobe Experience Manager (AEM) - AEM Assets | « Y a-t-il des fichiers svg dans le dossier `WKND` » ?<br><br>« Afficher les ressources modifiées après le 1er novembre 2025 dans le dossier `WKND` » |

**Informations connexes**

* [Fonctionnalités d’agent dans AEM : conseiller d’accès - découverte de contenu](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### Optimisation du contenu

| Exemple d’utilisation | Description | Compétence(s) | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Création de rendus haute résolution et rendus optimisés pour les canaux | Générer de nouveaux rendus d’une ressource à une résolution et un niveau de qualité spécifiés, ce qui facilite la préparation de variations prêtes pour le canal sans modification manuelle. Vous pouvez également produire des rendus adaptés aux exigences spécifiques de la plateforme, telles que les histoires Instagram, en veillant à ce que les ressources respectent automatiquement les directives de format, de ratio et de qualité. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | « Créer un rendu `2000px` en tant que `JPEG` avec `80% quality` »<br><br>« Créer un rendu pour une histoire Instagram » |
| Recouvrements de marque et génération composite | Appliquez des graphiques promotionnels, des superpositions ou des badges à des ressources existantes avec un emplacement précis, ce qui permet de créer rapidement des composites prêts pour la campagne. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | « Recouvrez l’image avec des graphiques de remise `30%` sur la bannière promotionnelle, en la plaçant `100px` au centre. » |
| Améliorations des images, réglages des couleurs d’arrière-plan, transformations d’orientation | Appliquez des améliorations visuelles (accentuation de l’image), remplacez les couleurs d’arrière-plan et effectuez des transformations d’orientation. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) - AEM Assets | « Changer la couleur d’arrière-plan de l’`PNG` en `#ff8932`« <br><br>« Accentuer l’image »<br><br>« Mettre l’image en miroir horizontalement » |

**Informations connexes**

* [Fonctionnalités d’agent dans AEM : gestionnaire de contenu - Optimisation du contenu](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## Gouvernance de marque

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Règle et recherche de segment | Récupérer des instructions détaillées sur la marque, par segment, marché ou catégorie | enterprise-context | Adobe Experience Manager (AEM) | « Quelles sont les directives relatives au ton de la voix pour cette marque ?« <br>« Énumérez les catégories d&#39;allégations utilisées dans le volet santé » |
| Évaluer le contenu par rapport aux directives de la marque | Évaluez une page, un bloc de texte ou une image publié/créé par rapport aux contrôles de marque configurés. | aem-gouvernance | Adobe Experience Manager (AEM) | « Évaluez cette page de destination par rapport aux directives de SecurBank »<br>« Ce slogan est-il conforme à nos contrôles de la tonalité ? » |
| Déboguer les autorisations AEM | Déboguer/comprendre les politiques d’autorisation, les listes de contrôle d’accès et les règles d’héritage. | aem-gouvernance | Adobe Experience Manager (AEM) | « Pourquoi l’administrateur principal peut-il écrire des `/content/folder/us` sur `https://author/` ? »<br>« Pourquoi un exemple d’auteur ne peut-il pas écrire dans `/content/dam` sur `https://author` ? » |

**Informations connexes**

* [Fonctionnalités d’agent dans AEM : gouvernance de marque](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

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
| Surveillance de la capacité de diffusion en continu et des violations | Vérifiez l’utilisation, la capacité et le statut de violation du streaming actuel et historique sur les sandbox | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | « Quelle est ma capacité de diffusion en continu actuelle dans mon sandbox actuel ? » · « Mon sandbox actuel a-t-il dépassé les limites de capacité au cours de la dernière semaine ? » |
| [Afficher les résultats de l’évaluation du contrôle de l’intégrité](https://experienceleague.adobe.com/en/docs/experience-platform/run-and-operate/health-checks/overview) | Affichez la dernière évaluation du contrôle de l’intégrité de votre sandbox, explorez un contrôle ayant échoué et consultez les entités affectées | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | « Quel est le problème dans mon sandbox ? » · « Me parler de ma dernière évaluation du contrôle de l’intégrité » · « Quels sont les problèmes liés à la vérification de la description de l’espace de noms personnalisé ? » |
| Résoudre les problèmes de contrôle de l’intégrité | Correction des problèmes d’espace de noms d’identité, de politique de fusion et de schéma signalés directement dans le chat, avec votre approbation avant toute modification | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | « Correction des descriptions des espaces de noms d’identité » · « Correction des noms de politiques de fusion en double » · « Correction des schémas sans le groupe de champs d’audit » · « Correction des noms de politiques de fusion par défaut » |

## Outil Sandbox

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| [Déplacement d’objets dans des sandbox](/help/agents/sandbox-tooling.md) | Migrez facilement les schémas, les audiences et d’autres configurations d’objet dans les sandbox, avec des dépendances résolues automatiquement | `sandbox-tooling-workflow` | Adobe Experience Platform | « Déplacer le schéma Luma Loyalty Members Platinum du sandbox actuel vers le sandbox de production » · « Promouvoir l’audience des membres du programme de fidélité Gold des États-Unis vers l’étape » |

## Alertes clients

| Exemple d’utilisation | Description | Compétences | Application | Exemples d’invites |
| --- | --- | --- | --- | --- |
| Gestion des abonnements aux alertes | Affichez et gérez les abonnements aux alertes par le biais de conversations en langage naturel. | `alerts-subscribe` | Adobe Experience Platform | « À quelles alertes suis-je abonné ?« <br><br>« Abonnez-moi à cette alerte.« <br><br>« Supprimez mon abonnement à cette alerte. » |
| Vérifier l’activité d’alerte | Examinez le statut actuel de l’alerte et l’activité historique de l’alerte pour une période spécifiée. | `alerts-list` | Adobe Experience Platform | « Que s’est-il passé au cours des dernières 24 heures ? »<br><br>« Quelles alertes ont été déclenchées au cours des dernières 24 heures ? »<br><br>« Affichez les alertes actives des sept derniers jours. » |
| Identification des modèles d’alerte récurrents | Analysez l’historique des alertes pour identifier les types d’alerte fréquemment déclenchés et les tendances opérationnelles. | `alerts-list` | Adobe Experience Platform | « Affichez-moi les trois principaux types d’alerte déclenchés. »<br><br>« Quels types d’alerte se sont produits le plus souvent ce mois-ci ? »<br><br>« Quels modèles d’alerte voyez-vous au cours des sept derniers jours ? » |
| Se concentrer sur les questions hautement prioritaires | Filtrez l’activité d’alerte par gravité pour donner la priorité aux efforts d’enquête. | `alerts-list` | Adobe Experience Platform | « Afficher uniquement les alertes de gravité élevée. »<br><br>« Quelles alertes critiques ont été déclenchées cette semaine ? »<br><br>« Afficher les alertes critiques des 30 derniers jours. » |
| Comprendre le rayon d’impact des alertes | Identifiez les objets les plus affectés par les alertes et déterminez où l&#39;enquête doit commencer. | `alerts-list` | Adobe Experience Platform | « Quels sont les 5 objets les plus impactés ? »<br><br>« Quels objets sont associés aux alertes de gravité la plus élevée ? » |
| Connecter les types d’alerte aux objets concernés | Analysez les relations entre les types d’alerte et les ressources affectées. | `alerts-list` | Adobe Experience Platform | « Quels types d’alerte ont le plus souvent eu un impact sur ce jeu de données ? »<br><br>« Affichez la relation entre les types d’alerte et les objets concernés. »<br><br>« Quel type d’alerte a le plus souvent eu un impact sur l’objet le plus touché ? » |
| Concentrez-vous sur mes alertes | Analysez les alertes auxquelles vous êtes abonné et qui sont chargées de leur surveillance. | `alerts-list` | Adobe Experience Platform | « Montrez-moi les alertes de niveau de gravité élevé auxquelles je m’abonne. »<br><br>« Quelles alertes provenant de mes alertes ont été déclenchées cette semaine ? »<br><br>« Y a-t-il des alertes auxquelles je me suis abonné qui nécessitent une attention particulière ? » |
