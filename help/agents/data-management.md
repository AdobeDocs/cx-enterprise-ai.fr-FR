---
title: Agent de gestion des données pour Adobe Experience Platform
description: Découvrez comment utiliser l’agent de gestion des données dans CX Coworker pour rechercher et analyser les jeux de données Adobe Experience Platform et gérer les politiques de conservation du lac de données.
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# Agent de gestion des données

>[!AVAILABILITY]
>
>L’agent de gestion des données est disponible pour tous les clients ayant accès à Adobe CX Enterprise Coworker.

Pour comprendre et gérer la rétention du lac de données pour vos jeux de données d’événements d’expérience, utilisez l’agent de gestion des données dans CX Coworker. À mesure que les jeux de données d’événements d’expérience se développent dans votre lac de données Adobe Experience Platform, l’exécution des requêtes et des processus en aval peut prendre plus de temps, tandis que les exigences de conservation deviennent plus difficiles à gérer. Décrivez ce que vous souhaitez accomplir en langage naturel. L’agent de gestion des données trouve les jeux de données d’événements d’expérience pertinents, analyse l’activité de leur utilisation et modélise la quantité de données qu’une période de conservation proposée affecterait. Lorsque vous êtes prêt à agir, il vous aide à définir, modifier ou supprimer une politique de conservation et vous demande votre confirmation avant toute modification.

## Fonctionnement de Data Management Agent {#what-the-data-management-agent-can-do}

Data Management Agent offre quatre compétences.

>[!NOTE]
>
>Les compétences Répertorier les jeux de données, Analyser l’utilisation des jeux de données et Analyser la rétention des jeux de données sont en lecture seule. Seule la compétence Gérer la rétention des jeux de données peut modifier une politique de rétention du lac de données. Elle nécessite votre confirmation explicite avant d’appliquer toute modification.

| Compétence | Description |
|---|---|
| **Liste des jeux de données** | À utiliser lorsque vous décidez où commencer une révision de la rétention. Répertorie vos jeux de données d’événements d’expérience avec la taille de stockage, le nombre de lignes, les paramètres de rétention existants et l’activation du profil afin que vous puissiez rapidement identifier les jeux de données qui peuvent être candidats à une politique de rétention du lac de données |
| **Analyse de l’utilisation des jeux de données** | À utiliser avant de décider si un jeu de données est un bon candidat pour une politique de conservation de lac de données. Classe l’activité d’un jeu de données spécifique en fonction de signaux tels que l’ingestion récente, l’activité de requête et l’utilisation de l’application en aval. |
| **Analyser la rétention des jeux de données** | À utiliser avant de s’engager dans une période de conservation. Affiche les mesures de stockage d’un jeu de données et l’âge de ses données, puis utilise cette distribution d’âge pour estimer la quantité approximative de données qu’une période de conservation potentielle conserverait ou supprimerait. |
| **Gérer la conservation des jeux de données** | À utiliser lorsque vous êtes prêt à agir. Définit, modifie ou supprime une politique de rétention du lac de données sur un jeu de données, avec une prévisualisation de l’impact et une confirmation avant toute modification. |

## Portée : rétention du lac de données par rapport aux autres outils de gestion des données {#scope}

Utilisez l’agent de gestion des données lorsque vous devez rechercher et analyser des jeux de données d’événements d’expérience et définir, modifier ou supprimer une politique de conservation du lac de données.

Si vous ne savez pas si une politique de conservation du lac de données est la bonne option pour votre objectif, consultez [Choisir la fonctionnalité de gestion du cycle de vie des données appropriée](https://experienceleague.adobe.com/fr/docs/experience-platform/data-lifecycle/choose-a-capability) pour comparer les options de conservation et de suppression disponibles.

Ces compétences ne gèrent pas les fonctionnalités associées suivantes :

- **Politique de rétention du magasin de profils.** Pour gérer la durée pendant laquelle les événements d’expérience restent dans la banque de profils, configurez une politique d’expiration d’événement d’expérience sur les jeux de données d’événements d’expérience activés pour le profil. Voir [Expiration d’un événement d’expérience](https://experienceleague.adobe.com/fr/docs/experience-platform/profile/event-expirations).
- **Expiration des données de profil pseudonymes à l’échelle du sandbox.** Pour supprimer automatiquement les données de profil pseudonymes dans un sandbox une fois qu’elles remplissent les conditions configurées, consultez la section [Profils pseudonymes](https://experienceleague.adobe.com/fr/docs/experience-platform/profile/pseudonymous-profiles).
- **Expiration du jeu de données.** Pour planifier la suppression d’un jeu de données complet à une date ultérieure, voir [Expiration du jeu de données](https://experienceleague.adobe.com/fr/docs/experience-platform/data-lifecycle/ui/dataset-expiration).
- **Suppression d’enregistrement.** Pour supprimer des enregistrements de profil individuels pour des raisons de confidentialité ou d’hygiène, voir [Suppression d’enregistrements](https://experienceleague.adobe.com/fr/docs/experience-platform/data-lifecycle/ui/record-delete).

## Conditions préalables {#prerequisites}

Avant de commencer, vérifiez que vous disposez des éléments suivants :

- Accès à Adobe Experience Platform et au sandbox qui contient les jeux de données à vérifier.
- Les autorisations Adobe Experience Platform requises pour les jeux de données et les actions de conservation que vous souhaitez utiliser. L’agent de gestion des données utilise vos autorisations Experience Platform existantes et n’accorde pas d’accès supplémentaire. Consultez la [présentation du contrôle d’accès](https://experienceleague.adobe.com/fr/docs/experience-platform/access-control/home) pour en savoir plus sur le fonctionnement des autorisations et des rôles Adobe Experience Platform.
- Plug-in Adobe CXO installé dans CX Coworker.

Pour obtenir des instructions sur l’installation de modules externes, consultez le [Guide de l’interface utilisateur de Coworker](https://experienceleague.adobe.com/fr/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).

## Utilisation de l’agent Data Management {#use-the-data-management-agent}

Interagissez avec l’agent de gestion des données via CX Coworker à l’aide du langage naturel. Décrivez votre objectif, puis affinez les résultats avec des questions de suivi.

>[!NOTE]
>
>Avant de commencer, assurez-vous de travailler dans le sandbox qui contient les jeux de données à vérifier.

Pour utiliser l’agent de gestion des données :

1. Accédez à **&#x200B;**. Pour plus d’informations sur l’accès, consultez le [guide de l’interface utilisateur de Coworker](https://experienceleague.adobe.com/fr/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).
1. Saisissez une demande qui décrit ce que vous souhaitez accomplir.
1. Passez en revue les résultats et utilisez les questions de suivi pour poursuivre votre enquête.

Si une requête modifie une politique de rétention du lac de données, l’agent de gestion des données indique l’impact proposé et nécessite votre confirmation avant d’appliquer la modification.

Pour obtenir un workflow de bout en bout permettant d’identifier les jeux de données, d’analyser l’utilisation et l’impact de la rétention, ainsi que de gérer les politiques de rétention du lac de données, consultez [Gérer la rétention du lac de données](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

## Fonctionnement de Data Management Agent {#how-the-data-management-agent-works}

L’agent Data Management utilise des calculs déterministes pour analyser l’utilisation des jeux de données, de sorte que les mêmes entrées produisent le même niveau d’utilisation. Il calcule également l’impact de la rétention par programmation plutôt que sur des estimations générées par l’IA. L&#39;impact sur la rétention reste une approximation parce qu&#39;il est basé sur la distribution par âge des données. L’agent récupère les données directement à partir des services Adobe Experience Platform pour fournir des informations à jour sur vos jeux de données.

## Limites {#limitations}

L’agent de gestion des données peut identifier les jeux de données qui peuvent être de bons candidats pour une politique de conservation du lac de données, mais il ne décide pas si un jeu de données en nécessite un. Il n’applique, ne modifie ou ne supprime pas une politique de conservation sans votre confirmation explicite.

## Étapes suivantes {#next-steps}

Pour obtenir des conseils sur l’utilisation de chaque compétence pour rechercher, analyser et gérer la rétention du lac de données sur vos jeux de données d’événements d’expérience, voir [&#x200B; Gérer la rétention du lac de données &#x200B;](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

Pour plus d’informations sur le fonctionnement des politiques de rétention du lac de données dans Adobe Experience Platform, notamment le comportement et la configuration de la rétention, consultez le guide [Conservation des jeux de données d’événements d’expérience (TTL)](https://experienceleague.adobe.com/fr/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide).
