---
title: IA dans les applications d’entreprise CX
description: Découvrez comment les applications CX Enterprise utilisent l’IA générative (GenAI), CX Enterprise Coworker, l’assistant d’IA, l’IA dédiée aux agences et les outils MCP.
TQID: 'https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds'
product_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
    internal-label: CX Enterprise Coworker
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
source-git-commit: a39c81f891a2bb1782f0531e210778f423a519a5
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 3%
---
# L’IA dans les applications CX Enterprise

Ce guide couvre les fonctionnalités de l’IA dans Adobe CX Enterprise : l’IA générative, CX Enterprise Coworker, l’assistant d’IA, Agent Orchestrator et MCP.

## Présentation des fonctionnalités de l’IA

Commencez ici pour une introduction sur l’endroit et la manière dont l’IA est utilisée dans CX Enterprise :

- [&#x200B; À propos de l’IA générative &#x200B;](./overview/generative-ai.md) décrit les applications CX Enterprise qui prennent en charge l’IA générative et l’assistant d’IA, et compare.
- [À propos de l’IA dédiée à l’agentic](./overview/agentic-ai.md) explique le fonctionnement de l’IA dédiée à l’agentic dans les applications CX Enterprise existantes et les applications dédiées à l’IA, et répertorie les agents disponibles dans chacun d’eux.
- [&#x200B; Surveillance de l’IA &#x200B;](./overview/monitoring.md) couvre les tableaux de bord qui suivent l’adoption, l’utilisation, les commentaires et la consommation de crédit de l’IA.
- [Consommation des crédits AI](./overview/ai-credit-consumption.md) explique comment les tâches de l’agent consomment les crédits AI, avec des taux de consommation estimés par agent et par type de tâche.
- [Transparence du contenu Generative AI](./content-transparency.md) explique comment Adobe joint automatiquement les métadonnées C2PA au contenu généré et modifié par GenAI dans les applications CX Enterprise.
- [CX Enterprise agentic tools](https://experienceleague.adobe.com/fr/docs/cx-enterprise-agentic-tools/using/overview) couvre les compétences et outils agentiques supplémentaires qui étendent les agents CX Enterprise (tutoriels vidéo).

## Coworker

Coworker est une évolution de l’IA Assistant orientée agent-first qui automatise l’expérience client et les workflows marketing, de sorte que votre équipe puisse se concentrer sur les objectifs commerciaux plutôt que sur l’exécution de routine. Au lieu de poser une question à la fois, vous décrivez un objectif. Un collègue planifie, exécute, valide et renvoie le travail terminé pour approbation. En savoir plus sur [&#128279;](https://business.adobe.com/products/cx-enterprise-coworker.html).

Le collaborateur comprend :

- **[Conversation avec un collègue](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)** : une interface de conversation permettant d’explorer vos données, de valider les audiences et les parcours, et d’effectuer des tâches en plusieurs étapes dans les applications CX Enterprise.
- **[Campagnes des collègues](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)** : une application native à l’IA qui regroupe l’information sur la campagne, la création d’audiences, la génération de contenu, la conception de parcours et la relecture dans une seule expérience de conversation. Il utilise des modèles intégrés, des bonnes pratiques et des conseils pour aider les petites équipes agiles à lancer rapidement des campagnes. En savoir plus sur [&#128279;](https://business.adobe.com/products/cx-enterprise-coworker/teams.html).
- **Projets de collègues** (bientôt disponible) : espace de travail unifié pour automatiser les workflows d’orchestration de l’expérience client de bout en bout, ce qui permet aux équipes de coordonner les tâches, les approbations et l’exécution afin d’obtenir des résultats de la stratégie à la diffusion. La documentation des projets sera bientôt disponible.

Les clients éligibles passent progressivement de l’assistant AI et des agents Experience Platform au chat des collègues. Lisez [Version d’évaluation des collaborateurs](./agents/trial.md) pour en savoir plus sur l’éligibilité des versions d’évaluation, l’utilisation du crédit AI et comment y accéder.

Pour voir le Module de conversation des collègues en action, [Module de conversation des collègues dans Playground](./coworker/playground-coworker-chat.md) ou lisez des cas d’utilisation réels tels que [Valider des données de migration d’AA vers CJA](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md), [valider vos données Experience Platform](./coworker/chat/use-cases/data-insights/data-validation-aep.md) et [Analyser des données CJA](./coworker/chat/use-cases/data-insights/analytics-chat.md).

Pour consulter la documentation complète du produit sur les conversations avec les collègues, les collègues pour les équipes (campagnes des collègues) et les projets, voir [Collègue](./coworker/overview.md). Pour la réplication d’objet de sandbox à sandbox, voir [Compétences de l’agent d’outils Sandbox](./agents/sandbox-tooling.md).

## Assistant IA

[AI Assistant](./ai-assistant/ai-assistant-ui.md) est un outil d’IA conversationnel et génératif disponible dans les applications Adobe Experience Platform. Utilisez-le pour acquérir des connaissances sur le produit, résoudre des problèmes, obtenir des informations opérationnelles et accéder aux agents Experience Platform, le tout via des invites en langage naturel dans une interface d’affichage plein écran ou par rail.

Pour savoir comment naviguer dans l’interface, lisez le guide de l’interface utilisateur de l’assistant [AI](./ai-assistant/ai-assistant-ui.md). Pour voir des exemples d’invites par agent, consultez la [bibliothèque d’invites](./ai-assistant/prompt-library.md).

## Agents Agent Orchestrator et Experience Platform

[&#128279;](./agents/agent-orchestrator.md) est la couche d’agent qui alimente les agents Experience Platform. Lorsque vous posez une question à l’assistant d’IA, Agent Orchestrator planifie le travail, fait appel aux agents spécialisés nécessaires pour y répondre et renvoie une réponse unifiée, le tout avec une supervision humaine.

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

Pour obtenir la liste complète des agents, les applications prises en charge par chacun et les conditions d’éligibilité, voir [IA dédiée aux agents dans CX Enterprise](./overview/agentic-ai.md).

## MCP

[La passerelle Adobe CX Coworker](./mcp/overview.md) est le point d’entrée MCP (Unified Model Context Protocol) pour CX Enterprise. Il offre aux clients compatibles avec MCP, tels que [!DNL Claude], [!DNL ChatGPT] et [!DNL Cursor], une connexion unique régie aux outils de produit que votre entreprise est autorisée à utiliser :

- [Outils Real-Time CDP](./mcp/rtcdp-mcp.md)
- [Outils Experience Platform](./mcp/aep-mcp.md)
- [Outils Journey Optimizer](./mcp/ajo-mcp.md)
- [Outils Customer Journey Analytics](./mcp/cja-mcp.md)
- [Outils Adobe Analytics](./mcp/analytics-mcp.md)
- Outils [!DNL Workfront], documentés dans le guide du serveur MCP [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/basics/workfront-mcp-server/workfront-mcp-server-overview)
- Outils [!DNL Target], présentés dans le guide [Guide du serveur MCP Target](https://experienceleague.adobe.com/en/docs/target/using/mcp/target-mcp)

Vous découvrez CX Coworker Gateway ? Voir [Accéder aux outils de la passerelle CX Coworker](./mcp/access.md) et [Installer la passerelle CX Coworker](./mcp/install.md) pour vous connecter. Une fois connecté, utilisez les [outils de contexte de session](./mcp/context-tools.md) pour définir l’organisation active, le sandbox et la vue de données avant d’appeler les outils du produit.

Avant d’utiliser ces outils, consultez [Avant de commencer](./overview/overview-ai-cxe.md#before-you-begin) pour en savoir plus sur les exigences d’accès, la confidentialité et la sécurité.

## Bonnes pratiques

Pour tirer le meilleur parti de votre expérience d’assistant d’IA ou de collègue, suivez ces bonnes pratiques :

- **Soyez précis** dans vos invites pour obtenir des informations ciblées et pertinentes.
- **Vérifier les réponses** en examinant les citations de la source et les explications du raisonnement fournies.
- **Utilisez le paramètre contextuel** pour vous assurer que les sources de données les plus pertinentes sont utilisées pour vos questions.
- **Fournissez des commentaires** pour améliorer les performances et la précision au fil du temps.
- **Combinez les informations** de plusieurs agents pour une analyse plus complète.

## Considérations juridiques

L’assistant AI prend actuellement en charge les réponses en anglais uniquement et les modèles de langue peuvent parfois faire des erreurs. Vérifiez toujours les informations fournies et utilisez les étapes de raisonnement incluses dans chaque réponse pour comprendre comment elles ont été générées. Pour plus de détails, lisez la [clause de non-responsabilité](./ai-assistant/legal-disclaimer.md).

Adobe joint automatiquement les métadonnées C2PA au contenu généré par GenAI et modifié par GenAI dans les applications CX Enterprise, afin de respecter les réglementations génératives en matière de transparence de l’IA. Pour plus d’informations, consultez la section [Transparence du contenu de Generative AI](./content-transparency.md).

