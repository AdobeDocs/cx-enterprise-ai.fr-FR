---
title: Consommation de crédit par l’IA
description: Découvrez la consommation des crédits d’IA dans les applications CX Enterprise.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
last-update: '2026-05-21T00:00:00.000Z'
last-substantial-update: 2026-19-2026
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
    internal-label: AI Tools
source-git-commit: 47f06af825995d14691816ff1fc3e5592ffd6250
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 7%
---
# Consommation des crédits AI

Découvrez la consommation des crédits d’IA dans les applications CX Enterprise.

## Crédits IA

Un _crédit d’IA_ est une mesure basée sur l’utilisation qui quantifie l’exécution d’actions ou de tâches.

## Services éligibles utilisant des crédits d’IA

* [CX Enterprise Coworker](#cx-enterprise-coworker-credit-rate)
* [Fonctionnalités de l’IA dédiée à CX Enterprise](#cx-enterprise-ai-capabilities)
* [Agents AEP](#aep-agents-credit-rate)

### taux de crédit CX Enterprise Coworker

Pendant une période d’introduction limitée, les entrées de collègues consomment des crédits AI à un taux de 25 crédits AI par entrée. Ce tarif est disponible pour une durée limitée uniquement et peut faire l’objet de modifications.

### Fonctionnalités de l’IA dédiée à CX Enterprise

| Fonctionnalité | Description | Applications prises en charge | Crédit IA |
| --- | --- | --- | --- |
| [Métadonnées Prenant En Compte La Marque](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/best-practices/brand-aware-metadata-best-practices) | Génération de métadonnées personnalisées sur la marque | Adobe Experience Manager [!DNL Assets] | 1 crédit IA (pour 10 générations de métadonnées) |
| Digital Rights Management | Extraction et gestion des droits d’utilisation | Adobe Experience Manager [!DNL Assets] | 6 crédits AI (par document traité) |

### Taux de crédit des agents AEP

Une _tâche d’agent_ est une série de tâches et d’actions qu’un agent AEP exécute pour obtenir un résultat spécifique, selon les instructions des clients.

À l’aide d’invites en langage naturel via l’assistant AI, vous pouvez demander à des agents d’effectuer des tâches spécifiques. En fonction de ces entrées, Agent Orchestrator coordonne les agents appropriés pour exécuter chaque étape dans les applications CX Enterprise appropriées.

L’utilisation du crédit de l’IA peut varier en fonction de la complexité et de la valeur de la tâche exécutée :

* Les tâches simples (souvent en une seule étape) consomment moins de crédits
* Les tâches complexes (souvent à plusieurs étapes) consomment davantage de crédits
* Les tâches impliquant un raisonnement avancé, la validation, la coordination multi-agent ou l&#39;intégration consomment plus de crédits

Pour connaître les agents AEP et les tâches d’agent disponibles dans vos applications CX Enterprise sous licence, consultez [Catalogue des fonctionnalités d’IA agentic CX Enterprise](https://agentic-capability-explorer.entapp.adproto.com/).

#### Taux estimés de crédit pour tâche de l&#39;agent

| Agent | Traitement | Applications prises en charge | Crédits IA estimés | Exemples d’invites |
| ------ | ----- | ------------------------ | ----------------------- | ----------------- |
| Agent Audience | Création d’audience/compte | <ul><li>Real-Time CDP (éditions B2B, B2C et B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li><em>Afficher les champs pour les acheteurs aisés</em></li><li><em>Rechercher tous les champs liés aux préférences du client</em></li></ul> |
| Agent Audience | Gestion des audiences/comptes | <ul><li>Real-Time CDP (éditions B2B, B2C et B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li><em>Y a-t-il des audiences en double ?</em></li><li><em>Afficher mes 5 audiences les plus importantes.</em></li><li><em>Afficher les audiences qui ne sont activées vers aucune destination</em></li><li><em>Répertorier toutes les audiences utilisées dans les parcours en direct</em></li></ul> |
| Agent Audience | Analyse des audiences/comptes | <ul><li>Real-Time CDP (éditions B2B, B2C et B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li><em>Quelles audiences ont augmenté leur taille de plus de 20 % au cours de la dernière semaine ?</em></li><li><em>Dans quelle mesure l’audience « Loyal Platinum » a-t-elle changé par rapport à la valeur il y a 30 jours ?</em></li><li><em>Quelle est mon audience qui croît le plus rapidement ?</em></li></ul> |
| Agent Audience | Idéation du groupe d&#39;achat | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li><em>Quels comptes indiquent leur intention pour ces produits ?</em></li><li><em>Afficher les personnes principales par intention de produit pour XYZ.</em></li><li><em>Quels groupes d&#39;achat comptent plus de 5 membres ?</em></li></ul> |
| Data Insights Agent | Analyse et visualisation des données | <ul><li>Customer Journey Analytics (éditions B2C et B2B)</li></ul> | 25 | <ul><li><em>Tendance des commandes en juillet</em></li><li><em>Afficher le chiffre d’affaires par région.</em></li><li><em>Afficher les commandes par genre, de mars à juin.</em></li><li><em>Quels étaient mes 10 principaux SKU par bénéfice en juin</em> ?</li><li><em>Proportion d&#39;achats par mois de l&#39;année</em></li><li><em>Part du chiffre d’affaires par catégorie de produits</em></li></ul> |
| Agent Journey | idéation du parcours | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li><em>Création d&#39;un parcours pour les comptes d&#39;espaces blancs avec l&#39;intention de ma solution, en se concentrant sur les personnes engagées avec le contenu sur le site web</em></li></ul> |
| Agent Journey | analyse de parcours | <ul><li>Adobe Journey Optimizer (éditions B2B et B2C)</li></ul> | 50 | <ul><li><em>Je souhaite analyser les abandons par nœud pour la campagne du 4 juillet par parcours.</em></li><li><em>Existe-t-il des conflits de planification pour le parcours X</em> ?</li><li><em>Afficher les conflits de chevauchement d&#39;audience pour le parcours X</em></li></ul> |
| Agent Journey | Gestion des parcours | <ul><li>Adobe Journey Optimizer (éditions B2B et B2C)</li></ul> | 25 | <ul><li><em>De combien de parcours en direct dispose-t-on ?</em></li><li><em>Répertorier tous les parcours utilisant l’audience X.</em></li><li><em>Répertorier tous les parcours actuellement en mode test</em></li></ul> |
| Agent du support technique du produit | Dépannage basé sur les connaissances | <ul><li>Real-Time CDP (éditions B2B, B2C et B2P)</li><li>Adobe Journey Optimizer (éditions B2C et B2B)</li><li>Customer Journey Analytics (éditions B2C et B2B)</li></ul> | 0 | <ul><li><em>Pourquoi mon nombre de profils diffère-t-il sur le tableau de bord d’utilisation de la licence et la page d’accueil d’Experience Platform ?</em></li><li><em>Quelles sont les raisons pour lesquelles un parcours ne se déclenche pas ?</em></li><li><em>Comment Adobe Experience Platform crée-t-il des expériences en temps réel ?</em></li><li><em>Comment configurer et utiliser les alertes dans Adobe Experience Platform ?</em></li><li><em>Quelle est la limite de richesse moyenne des profils dans l&#39;activation de Adobe Experience Platform ?</em></li></ul> |
| Agent du support technique du produit | Création et suivi des cas d’assistance | <ul><li>Real-Time CDP (éditions B2B, B2C et B2P)</li><li>Adobe Journey Optimizer (éditions B2C et B2B)</li><li>Customer Journey Analytics (éditions B2C et B2B)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li><em>Créer un nouveau ticket d’assistance pour ma tâche de segmentation ayant échoué</em></li><li><em>Quel est l&#39;état du ticket E-001772068 ?</em></li></ul> |
| Agent du gestionnaire de contenu | Découverte de contenu | <ul><li>Adobe Experience Manager</li></ul> | 5 | <ul><li><em>Afficher les fragments de contenu pour la création de la campagne d’offres WKND.</em></li><li><em>Rechercher des images PNG d&#39;emballage de produit.</em></li><li><em>Afficher les images balisées office dans le dossier WKND.</em></li><li><em>Le dossier WKND contient-il des fichiers SVG ?</em></li><li><em>Afficher tous les formulaires de demande de prêt.</em></li><li><em>Je recherche des formulaires d&#39;intégration des employés.</em></li></ul> |
| Agent du gestionnaire de contenu | <ul><li>Optimisation du contenu</li></ul> | <ul><li>Adobe Experience Manager Assets et Dynamic Media</li></ul> | 10 | <ul><li><em>Créez un rendu de 2 000 px en tant que JPEG avec une qualité de 80 %.</em></li><li><em>Créez un rendu pour une histoire Instagram.</em></li><li><em>Superposez l&#39;image avec des graphiques à 30 % de remise sur la bannière promotionnelle, en la plaçant à 100 px du centre.</em></li><li><em>Changer la couleur d&#39;arrière-plan du fichier PNG en #ff8932.</em></li></ul> |
| Agent de gouvernance de marque | <ul><li>Vérifications de la politique de marque</li></ul><ul><li>Autorisations avec Content Hub</li></ul><ul><li>Expiration des ressources</li></ul> | <ul><li>Adobe Experience Manager Sites (stratégies de marque)</li></ul><ul><li>Adobe Experience Manager Assets</li></ul> | 25 | <ul><li><em>Cette page correspond-elle à ma marque ? `https://www.website/en.html`</em></li><li><em>Afficher toutes les règles ABAC Content Hub existantes</em></li><li><em>Certaines de mes ressources expirent-elles bientôt ?</em></li></ul> |
| Brand Experience Agent | <ul><li>Mise à jour du contenu</li><li>Création de Forms</li><li>Dépannage du pipeline</li></ul> | <ul><li>Services cloud Adobe Experience Manager</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li><em>Le `URL`, mettez à jour le titre en Hello world</em></li><li><em>Créez un formulaire de contact avec des champs de nom, d&#39;e-mail et de message</em></li><li><em>Résolution des problèmes liés à l’échec de mon pipeline</em></li><li><em>Répertorier mes pipelines ayant échoué pour le programme principal.</em></li></ul> |
| Brand Experience Agent | Modernisation du site | Services cloud Adobe Experience Manager | 100 | <ul><li><em>Migrer la page `https://wknd-trendsetters.site`</em></li></ul> |

>[!NOTE]
>
>La consommation réelle de crédit de l’IA peut varier en fonction du nombre d’étapes exécutées et d’itérations par étape.

## Plus d’aide sur cette rubrique

* [GenAI dans CX Enterprise](generative-ai.md)
* [IA agentique dans CX Enterprise](agentic-ai.md)
* [Essai des agents Adobe Experience Platform lié à l’utilisation](https://experienceleague.adobe.com/fr/docs/cx-enterprise-ai/experience-cloud-ai/agents/trial)
