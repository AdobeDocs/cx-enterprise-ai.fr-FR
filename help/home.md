---
title: IA dans les applications d’entreprise CX
description: Découvrez comment les applications CX Enterprise utilisent l’IA générative (GenAI), CX Enterprise Coworker, l’assistant d’IA, l’IA dédiée aux agences et les outils MCP.
TQID: 'https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds'
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: Coworker
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 9dab42a742d258dd7d3dea3ae555a6f8b3ecac9b
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 4%
---
# L’IA dans les applications CX Enterprise

Ce guide présente les fonctionnalités d’IA disponibles dans Adobe CX Enterprise : collègue, assistant d’IA et Agent Orchestrator avec les agents Experience Platform qu’il alimente. Commencez par la présentation ci-dessous pour comprendre la relation entre ces fonctionnalités, puis suivez les liens pour configurer l’accès, surveiller l’utilisation et tirer le meilleur parti de chacune d’elles.

- [À propos de l’IA générative](./overview/generative-ai.md) décrit quelles applications CX Enterprise prennent en charge l’IA générative et l’assistant d’IA, et comment elles se comparent.
- [À propos de l’IA dédiée aux agents](./overview/agentic-ai.md) explique le fonctionnement de l’IA dédiée aux agents dans les applications CX Enterprise existantes et les applications dédiées à l’IA, et répertorie les agents disponibles dans chacune d’elles.
- [La surveillance de l&#39;IA](./overview/monitoring.md) couvre les tableaux de bord de l&#39;assistant IA qui suivent l&#39;adoption, l&#39;utilisation, les commentaires et la consommation de crédit de l&#39;IA.
- [Consommation des crédits AI](./overview/ai-credit-consumption.md) explique comment les tâches de l&#39;agent consomment les crédits AI, avec des taux de consommation estimés par agent et type de tâche.
- [La transparence du contenu Generative AI](./content-transparency.md) explique comment Adobe joint automatiquement les métadonnées C2PA au contenu généré et modifié par GenAI dans les applications CX Enterprise.
- [Les outils agentic de CX Enterprise](https://experienceleague.adobe.com/fr/docs/cx-enterprise-agentic-tools/using/overview) couvrent les compétences et les outils agentic supplémentaires qui étendent les agents CX Enterprise (tutoriels vidéo).

## Coworker

Coworker est une évolution de l’IA Assistant orientée agent-first qui automatise l’expérience client et les workflows marketing, de sorte que votre équipe puisse se concentrer sur les objectifs commerciaux plutôt que sur l’exécution de routine. Au lieu de poser une question à la fois, vous décrivez un objectif. Un collègue planifie, exécute, valide et renvoie le travail terminé pour approbation. En savoir plus sur [Adobe for Business](https://business.adobe.com/fr/products/cx-enterprise-coworker.html).

Le collaborateur comprend :

- **[Conversation avec un collègue](https://experienceleague.adobe.com/fr/docs/coworker/content/chat/overview)** : une interface de conversation pour explorer vos données, valider les audiences et les parcours et effectuer des tâches en plusieurs étapes dans les applications CX Enterprise.
- **[Collègue pour les équipes](https://experienceleague.adobe.com/fr/docs/coworker/content/campaigns/overview)** : application native de l’IA qui regroupe les informations sur la campagne, la création d’audiences, la génération de contenu, la conception de parcours et la relecture dans une seule expérience de conversation. Il utilise des modèles intégrés, des bonnes pratiques et des conseils pour aider les petites équipes agiles à lancer rapidement des campagnes. En savoir plus sur [Adobe for Business](https://business.adobe.com/fr/products/cx-enterprise-coworker/teams.html).
- **Projets collaborateurs** (bientôt disponible) : espace de travail unifié pour automatiser les workflows d’orchestration de l’expérience client de bout en bout, aidant les équipes à coordonner les tâches, les approbations et l’exécution afin d’obtenir des résultats de la stratégie à la diffusion. La documentation des projets sera bientôt disponible.

Les clients éligibles passent progressivement de l’assistant AI et des agents Experience Platform au chat des collègues.

### Ressources du collègue

- Lisez la [version d’essai de vos collaborateurs](./agents/trial.md) pour en savoir plus sur l’éligibilité de la version d’essai, l’utilisation du crédit AI et comment y accéder.
- Voir la page d’accueil d’aide de [Coworker](https://experienceleague.adobe.com/fr/docs/coworker/content/home) pour tout le contenu de Coworker.
- Pour la réplication d’objet sandbox à sandbox, voir [Compétences en agent pour les outils sandbox](https://experienceleague.adobe.com/fr/docs/coworker/content/chat/use-cases/sandbox-tooling/sandbox-tooling).

## Assistant IA

[L’assistant AI](./ai-assistant/ai-assistant-ui.md) est un outil d’IA conversationnel et génératif disponible dans les applications Adobe Experience Platform. Utilisez-le pour acquérir des connaissances sur le produit, résoudre des problèmes, obtenir des informations opérationnelles et accéder aux agents Experience Platform, le tout via des invites en langage naturel dans une interface d’affichage plein écran ou par rail.

Pour savoir comment naviguer dans l’interface, lisez le [guide de l’interface utilisateur de l’assistant AI](./ai-assistant/ai-assistant-ui.md). Pour voir des exemples d’invites par agent, consultez la [bibliothèque d’invites](./ai-assistant/prompt-library.md).

## Agents Agent Orchestrator et Experience Platform

[Agent Orchestrator](./agents/agent-orchestrator.md) est la couche d’agent qui alimente les agents Experience Platform. Lorsque vous posez une question à l’assistant d’IA, Agent Orchestrator planifie le travail, fait appel aux agents spécialisés nécessaires pour y répondre et renvoie une réponse unifiée, le tout avec une supervision humaine.

Les agents Experience Platform suivants sont documentés dans ce guide :

- [Agent Audience](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Agent Experimentation](./agents/agent-experiment.md)
- [Agent de découverte de champ](./agents/field-discovery-agent.md)
- [Agent Journey](./agents/ajo-agent.md)
- [Agent de notifications](./agents/notifications.md)
- [Agent du support technique du produit](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [Valider vos données](./agents/data-validation.md)

Pour obtenir la liste complète des agents, les applications prises en charge par chacun et les conditions d’éligibilité, consultez [IA dédiée aux agents dans CX Enterprise](./overview/agentic-ai.md).

<!--
## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md) is the unified Model Context Protocol (MCP) endpoint for CX Enterprise. It gives MCP-compatible clients, such as [!DNL Claude], [!DNL ChatGPT], and [!DNL Cursor], a single governed connection to the product tools your organization is entitled to use:

- [Real-Time CDP tools](./mcp/rtcdp-mcp.md)
- [Experience Platform tools](./mcp/aep-mcp.md)
- [Journey Optimizer tools](./mcp/ajo-mcp.md)
- [Customer Journey Analytics tools](./mcp/cja-mcp.md)
- [Adobe Analytics tools](./mcp/analytics-mcp.md)
- [!DNL Workfront] tools, documented in the [Workfront MCP server guide](https://experienceleague.adobe.com/fr/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)
- [!DNL Target] tools, documented in the [Target MCP server guide](https://experienceleague.adobe.com/fr/docs/target/using/mcp/target-mcp)

New to CX Coworker Gateway? See [Access CX Coworker Gateway tools](./mcp/access.md) and [Install CX Coworker Gateway](./mcp/install.md) to get connected. Once connected, use the [session context tools](./mcp/context-tools.md) to set the active organization, sandbox, and data view before calling product tools.

Before you use any of these tools, see [Before you begin](./overview/overview-ai-cxe.md#before-you-begin) for access requirements and privacy and security considerations.
-->

## Bonnes pratiques

Pour tirer le meilleur parti de votre expérience d’assistant d’IA ou de collègue, suivez ces bonnes pratiques :

- **Soyez spécifique** dans vos invites pour obtenir des informations ciblées et pertinentes.
- **Vérifiez les réponses** en examinant les citations sources et les explications de raisonnement fournies.
- **Utilisez le paramètre de contexte** pour vous assurer que les sources de données les plus pertinentes sont utilisées pour vos questions.
- **Fournissez des commentaires** pour améliorer les performances et la précision au fil du temps.
- **Combinez les informations** provenant de plusieurs agents pour une analyse plus complète.

## Considérations juridiques

L’assistant AI prend actuellement en charge les réponses en anglais uniquement et les modèles de langue peuvent parfois faire des erreurs. Vérifiez toujours les informations fournies et utilisez les étapes de raisonnement incluses dans chaque réponse pour comprendre comment elles ont été générées. Pour plus d&#39;informations, lisez la [clause de non-responsabilité](./ai-assistant/legal-disclaimer.md).

Adobe joint automatiquement les métadonnées C2PA au contenu généré par GenAI et modifié par GenAI dans les applications CX Enterprise, afin de respecter les réglementations génératives en matière de transparence de l’IA. Pour plus d’informations, lisez [Transparence du contenu de Generative AI](./content-transparency.md).

