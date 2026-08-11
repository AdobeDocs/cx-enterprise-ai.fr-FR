---
title: Présentation de la passerelle du collègue Adobe CX
description: Adobe CX Coworker Gateway est le MCP unifié pour Adobe CX Enterprise, offrant aux clients MCP une connexion unique aux outils de produits pris en charge.
source-git-commit: 4bc180a76f3c1095a4d25ed7e07d804e4d5ff1a9
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 5%

---

# Passerelle de collègue Adobe CX {#mcp-overview}

La passerelle de collaboration Adobe CX est le protocole MCP (Unified Model Context Protocol) pour Adobe CX Enterprise. Avec une seule connexion, les clients compatibles avec MCP peuvent accéder aux outils de produit Adobe que votre organisation et votre compte sont autorisés à utiliser.

>[!IMPORTANT]
>
>Votre organisation Adobe doit être activée avant de pouvoir utiliser les outils **CX Coworker Gateway**.
>
>Si votre organisation n’y a pas encore accès, envoyez un e-mail à [](mailto:cx-coworker-gateway-support@adobe.com) pour demander l’activation de votre organisation.

Utilisez le point d’entrée CX Coworker Gateway pour toute la configuration du client MCP :

```
https://cx-coworker-gateway.adobe.io/mcp
```

Une fois que vous êtes connecté, le point d’entrée expose les outils disponibles pour votre organisation Adobe et vos informations d’identification. Les pages spécifiques à un produit de ce guide décrivent les tâches possibles de chaque outil de produit, les données auxquelles il peut accéder et les restrictions spécifiques à un produit.

## Qu’est-ce que le protocole de contexte de modèle ? {#mcp-what-is}

MCP (Model Context Protocol) est une norme open source permettant de connecter des applications d’IA à des systèmes externes. Les clients compatibles avec MCP tels que [!DNL Claude], [!DNL ChatGPT], [!DNL Cursor], [!DNL Claude Code], [!DNL Codex] et [!DNL VS Code] peuvent utiliser ces outils pour récupérer le contexte du produit, exécuter les opérations prises en charge et renvoyer les réponses en langage naturel.

La passerelle CX Coworker fournit un point d’entrée régi pour les outils de produit de la passerelle CX Coworker. Au lieu d’ajouter des serveurs de produit distincts, connectez-vous une fois au point d’entrée et utilisez les outils de produit affichés pour vos solutions autorisées.

## Outils de produit disponibles {#available-product-tools}

Les outils de produit suivants sont documentés dans ce guide :


| Outils de produit | Ce qu’il expose via le point d’entrée | Disponibilité | Documentation |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Real-Time CDP** | Audiences, destinations, sources, espaces de noms d’identité et intégrité de l’activation (lecture seule) | Beta | [Outils ](rtcdp-mcp.md) |
| **Experience Platform** | Schémas, jeux de données, gouvernance des données, Query Service et événements d’audit (lecture seule) | Beta | [Outils ](aep-mcp.md) |
| **Journey Optimizer** | Campagnes et configurations de canal (lecture seule) | Beta | [Outils ](ajo-mcp.md) |
| **Customer Journey Analytics** | Vues de données, dimensions, mesures, rapports, segments, périodes, projets et audiences (lecture et écriture) | Disponible | [Outils ](cja-mcp.md) |
| **Adobe Analytics** | Suites de rapports, dimensions, mesures, rapports, segments, périodes et projets Workspace (lecture et écriture pour les composants pris en charge) | Disponible | [Outils ](analytics-mcp.md) |
| **Workfront** | Outils de gestion du travail pour les projets, les tâches et les processus d&#39;approbation | Prévisualisation | [Serveur Workfront MCP](https://experienceleague.adobe.com/en/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview) |


>[!NOTE]
>
>La disponibilité des outils dépend de vos licences de produit, de l’activation de l’organisation, des autorisations de produit et des informations d’identification Adobe utilisées pour l’authentification. Le MCP ne fait apparaître que les outils auxquels votre organisation et votre compte utilisateur ont droit d’accès. Voir [Accéder aux outils de passerelle de collègue CX](access.md).



## Commencer {#mcp-get-started}

1. Consultez [Accéder aux outils de passerelle de collègue CX](access.md) pour confirmer la disponibilité, l’activation et les autorisations du produit.
2. Suivez [Installation d’Adobe pour la passerelle CX Coworker](install.md) pour connecter votre client MCP au point d’entrée .
3. Consultez la page produit pour chaque outil de produit que vous prévoyez d’utiliser.

