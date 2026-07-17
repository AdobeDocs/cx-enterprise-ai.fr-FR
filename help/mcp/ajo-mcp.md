---
title: Outils Adobe Journey Optimizer dans la passerelle CX Coworker
description: Découvrez les outils Adobe Journey Optimizer disponibles via la passerelle CX Coworker.
source-git-commit: 30f4d593bdec8cb45d10c4c49fac3dce16e8ca03
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 3%

---

# Outils Adobe Journey Optimizer dans la passerelle CX Coworker {#ajo-mcp}

Utilisez les outils de produit Adobe Journey Optimizer pour inspecter les campagnes et les configurations de canal à partir d’un client compatible MCP. Ces outils sont disponibles via la passerelle [CX Coworker](overview.md) lorsque votre organisation est activée et que votre compte utilisateur dispose des autorisations Journey Optimizer requises.

>[!AVAILABILITY]
>
>Les outils du produit Journey Optimizer se trouvent dans Beta. L’accès se fait sur invitation uniquement et nécessite l’activation de l’organisation Adobe. Voir [Accéder aux outils de passerelle de collègue CX](access.md).

## Fonctionnalités principales {#mcp-capabilities}

Les outils Journey Optimizer fournissent une surface en lecture seule pour la révision de la configuration des campagnes et des canaux. Vous pouvez ainsi :

- Répertoriez les campagnes Journey Optimizer et filtrez par statut.
- Récupérez les détails de la campagne, y compris le ciblage, le planning, le canal et les métadonnées de configuration du contenu.
- Répertorier les configurations des canaux pour les canaux e-mail, SMS, push et WhatsApp.
- Examinez la configuration des campagnes et des canaux en langage naturel sans naviguer dans les écrans des produits.

>[!IMPORTANT]
>
>Tous les outils Journey Optimizer du Beta actuel sont en lecture seule. La création, la mise à jour, la suppression, le démarrage, l’arrêt ou la publication de campagnes n’est pas pris en charge.

## Outils disponibles {#mcp-tools}

| Outil | Description |
| --- | --- |
| `ajo_campaign_list` | Parcourez les campagnes marketing Journey Optimizer. Prend en charge le filtrage par statut, tel que `DRAFT`, `LIVE`, `STOPPED` et `COMPLETED`. |
| `ajo_campaign_get` | Récupérez les détails et la configuration d’une campagne spécifique par identifiant, y compris le ciblage de l’audience, le planning, le canal et les métadonnées des paramètres de contenu. |
| `ajo_channel_configuration_list`, `ajo_channel_configuration_get` | Affichez les paramètres prédéfinis de surface et les paramètres de branding pour les canaux e-mail, SMS, notification push ou [!DNL WhatsApp]. |

## Exemples d’invites {#mcp-use-cases}

| Objectif | Exemple d’invite |
| --- | --- |
| Vue d’ensemble de la campagne | « Afficher toutes mes campagnes Journey Optimizer. » |
| Audit de statut | « Quelles sont les campagnes actuellement actives ? » |
| Détails de la campagne | « Obtenez les détails complets des `[campaign ID]` de campagne. » |
| Public et ciblage | « Quelle audience est ciblée dans l’`[campaign ID]` de campagne ? » |
| Planning et minutage | « Quand l’exécution de la campagne est-elle planifiée `[campaign ID]` ? » |
| Dépannage | « Vérifiez la configuration des `[campaign ID]` de campagne et signalez les problèmes possibles. » |
| Configuration des canaux | « Quelles configurations de canal e-mail sont disponibles ? » |
| Audit de canal | « Quelles configurations de canal sont manquantes ou incomplètes ? » |

## Contexte et autorisations du produit {#mcp-context}

Votre compte utilisateur doit disposer des autorisations nécessaires pour afficher les campagnes Journey Optimizer et les configurations de canal sur lesquelles vous effectuez une requête. Le MCP ne contourne pas les autorisations de produit.

Si votre organisation utilise plusieurs sandbox, spécifiez le sandbox ou le contexte de l’environnement dans votre invite lorsque vous avez besoin des résultats d’un sandbox spécifique.

## Limites connues {#mcp-limitations}

| Limite | Description | Solution de contournement |
| --- | --- | --- |
| Surface en lecture seule | Les outils Journey Optimizer exposent uniquement les opérations de récupération. Vous ne pouvez pas créer, mettre à jour, supprimer, démarrer, arrêter ou publier de campagnes. | Utilisez l’interface utilisateur ou les API de Journey Optimizer pour les opérations d’écriture. |
| Aucune mesure d’engagement ou de performances | Les outils ne renvoient pas de données de rapport telles que les impressions, les taux de clic publicitaire, les conversions ou les statistiques de diffusion. | Utilisez les rapports Journey Optimizer, les outils Customer Journey Analytics ou les outils Adobe Analytics pour les mesures de performances. |
| La pagination de la liste des campagnes est limitée | La liste des campagnes renvoie la première page de résultats, avec un maximum de 50 campagnes triées par ordre alphabétique. Les valeurs de décalage et de limite ne sont pas appliquées. | Utilisez `Get Campaign` directement si l’identifiant de campagne est connu. Utilisez l’interface utilisateur de Journey Optimizer pour une navigation et un filtrage complets. |
| Aucun filtrage côté serveur par date, canal ou planning | Les listes Campaign prennent en charge le filtrage du statut, mais pas le filtrage par date de publication, date de planning, canal ou type de campagne. | Utilisez la liste des campagnes de l’interface utilisateur de Journey Optimizer pour le filtrage de date et de canal natif. |
| Récupération du contenu du message non disponible | Les outils actuels ne permettent pas de trouver des messages HTML, des objets, des jetons de personnalisation ni du contenu d’offre. | Affichez le contenu et la personnalisation des messages directement dans l’interface utilisateur de Journey Optimizer. |