---
title: Compétences de l’agent d’outils Sandbox
description: Découvrez comment utiliser les compétences d’agent des outils Sandbox pour répliquer des métadonnées d’objet dans les environnements Sandbox.
source-git-commit: 5de0afec89309ab62bd50e0c2cb1d0e96890c57f
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---


# Compétences de l’agent d’outils Sandbox

>[!AVAILABILITY]
>
>Les compétences agent d’outils Sandbox sont disponibles pour tous les clients ayant accès à un collègue Adobe. Pour utiliser toutes les fonctionnalités disponibles, vous devez disposer des autorisations suivantes :
>
>**Gérer-sandbox** ou **Afficher-sandbox** : ces autorisations vous permettent d’utiliser les compétences de l’agent d’outils de sandbox pour afficher des sandbox directement dans Coworker.
>
>**Manage-package** : cette autorisation vous permet d’utiliser les compétences Agentic de l’outil Sandbox pour créer des packages directement dans Coworker.

>[!NOTE]
>
>Vous pouvez actuellement utiliser les compétences d’agent des outils Sandbox pour découvrir, compresser et migrer des objets de schéma et d’audience. La prise en charge de types d’objets supplémentaires sera ajoutée dans les prochaines versions.

Utilisez les compétences techniques des outils Sandbox pour déplacer les métadonnées d’objet (y compris les schémas et les audiences) dans les environnements Adobe Experience Platform en décrivant ce que vous souhaitez accomplir en langage naturel. Grâce à Coworker, vous pouvez découvrir les métadonnées requises, identifier automatiquement les dépendances, créer des packages de migration et migrer des objets par le biais d’une expérience de conversation.

## Conditions préalables {#prerequisites}

Avant de commencer, vérifiez que vous disposez des éléments suivants :

- L’accès à Adobe Experience Platform, ainsi qu’à l’organisation et au sandbox appropriés.
- Accès aux objets que vous souhaitez découvrir ou migrer.
- Plug-in Adobe CXO installé dans Coworker.

Pour obtenir des instructions sur l’installation de modules externes, consultez le [Guide de l’interface utilisateur de Coworker](https://experienceleague.adobe.com/fr/docs/cx-enterprise-coworker/content/chat/ui-guide).

## Utilisation des compétences d’agent pour les outils Sandbox {#use-sandbox-tooling-agentic-skills}

Interagissez avec les compétences Agentic des outils Sandbox via un collègue en utilisant le langage naturel. Décrivez votre objectif aussi clairement que possible. Les requêtes spécifiques produisent les meilleurs résultats, tandis que des invites vagues ou trop brèves peuvent renvoyer des résultats de moindre qualité ou ne pas appeler l&#39;agent.

Pour utiliser les compétences d’agent des outils Sandbox :

1. Accédez à **[!UICONTROL Collègue CX]**.
1. Saisissez une description claire de ce que vous souhaitez accomplir. Par exemple :

   *« Déplacez le schéma Loyalty Member Platinum du sandbox actuel vers le sandbox de démonstration Acme. »*

1. Consultez le tableau des résultats qui indique les sandbox source et cible. Lorsque vous êtes prêt à continuer, sélectionnez **[!UICONTROL Continuer]**, puis sélectionnez **[!UICONTROL Envoyer]** pour confirmer.

   ![Les résultats de la requête avec Continuer sélectionné, en surbrillance Envoyer.](./assets/sandbox-tooling/results-proceed.png)

1. Sélectionnez un ou plusieurs objets à migrer, puis sélectionnez **[!UICONTROL Envoyer]**.

   ![Page de sélection d’objets mettant en surbrillance Envoyer.](./assets/sandbox-tooling/object-selection.png)

1. Passez en revue les objets et les dépendances identifiés par l’agent et confirmez les actions d’opération : *Créer* ou *Utiliser existant*. Lorsque vous êtes prêt(e) à commencer la migration, sélectionnez **[!UICONTROL Continuer]**, puis **[!UICONTROL Envoyer]** pour confirmer. La migration peut prendre plusieurs minutes.

   ![Page Confirmer le plan d’action mettant en surbrillance Envoyer.](./assets/sandbox-tooling/action-plan.png)

1. Une fois la migration terminée, les objets sélectionnés sont disponibles dans le sandbox cible.

![Page Transfert terminé affichant le statut de la demande.](./assets/sandbox-tooling/transfer-complete.png)

Pour plus d’informations sur l’utilisation de Coworker, consultez le [Guide de l’interface utilisateur de Coworker](https://experienceleague.adobe.com/fr/docs/cx-enterprise-coworker/content/chat/ui-guide).

## Cas d’utilisation pris en charge {#supported-use-cases}

Explorez les méthodes courantes d’utilisation des outils Sandbox. Compétences des agents pour simplifier la gestion des sandbox et la migration des métadonnées.

### Déplacement de métadonnées d’objet entre des sandbox

En tant qu’administrateur de sandbox gérant plusieurs sandbox Adobe Experience Platform, vous pouvez migrer des métadonnées d’objet à l’aide de requêtes en langage naturel au lieu de parcourir manuellement l’interface utilisateur.

Grâce à Coworker, vous pouvez migrer des métadonnées d’objet (y compris des schémas, des audiences et des ressources de configuration associées) d’un sandbox à un autre en décrivant la migration en langage naturel. Sandbox Tooling Agentic Skills identifie et regroupe automatiquement les dépendances requises, contribuant ainsi à assurer une migration fiable.

Par exemple :

> « Déplacez le schéma Luma Loyalty Members Platinum du sandbox actuel vers le sandbox de production. »

### Promouvoir les audiences entre les sandbox

En tant qu’administrateur de sandbox, vous pouvez promouvoir des audiences entre des environnements sans les recréer ou les reconfigurer manuellement.

Par exemple :

> « Convertissez l’audience « Nom de l’audience » en sandbox d’évaluation. »

Les compétences Agentic (outils pour sandbox) identifient l’audience spécifiée, valident ses dépendances et migrent tous les objets requis vers la sandbox cible.

## Exemples d’invites {#example-prompts}

Utilisez les invites suivantes comme exemples lors de l’interaction avec les compétences Agentic d’outil Sandbox.

### Invites de schéma

Utilisez ces invites lorsque vous connaissez le nom du schéma et le sandbox de destination.

- « Déplacez le schéma « Nom du schéma » du sandbox actuel vers le sandbox de production. »

### Invites d’audience

Utilisez ces invites lorsque vous connaissez le nom de l&#39;audience.

- « Convertissez l’audience « Nom de l’audience » en sandbox d’évaluation. »

## Étapes suivantes {#next-steps}

Après avoir lu ce guide, vous devriez comprendre comment utiliser les compétences Agentic de l’outil Sandbox pour découvrir, regrouper et migrer les objets pris en charge entre les sandbox.

Pour plus d’informations sur l’outil Sandbox, consultez le [Guide de l’outil Sandbox](https://experienceleague.adobe.com/fr/docs/experience-platform/sandbox/ui/sandbox-tooling).
