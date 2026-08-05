---
title: IA dans les applications d’entreprise CX
description: Découvrez comment les applications d’entreprise CX utilisent l’IA générative (GenAI), l’assistant IA, l’IA dédiée aux agences, l’expérience client et les outils MCP.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: ca4515cb9010fb352489700108bbfe95396b0ad3
workflow-type: tm+mt
source-wordcount: 864
ht-degree: 4%

---

# IA dans CX Enterprise

Ce guide couvre les fonctionnalités d’IA d’Adobe CX Enterprise : IA générative, assistant d’IA, Agent Orchestrator, agents Experience Platform, collègue d’entreprise CX et MCP.

## Présentation des fonctionnalités de l’IA

Commencez ici pour une introduction sur où et comment l’IA est utilisée dans l’entreprise CX :

- [IA générative](./overview/generative-ai.md) décrit les applications d’entreprise CX qui prennent en charge l’IA générative et l’assistant d’IA, et compare.
- [Agentic AI](./overview/agentic-ai.md) explique le fonctionnement des agents Experience Platform à la fois dans les applications CX Enterprise et les applications AI-first existantes, et répertorie les agents disponibles dans chacune d’elles.
- [Surveillance de l’IA dédiée aux agents](./overview/monitoring.md) couvre les tableaux de bord qui suivent l’adoption, l’utilisation, les commentaires et la consommation de crédit de l’IA.
- [Tâches d’agent et consommation de crédits AI](./overview/ai-credit-consumption.md) explique comment les tâches d’agent consomment des crédits AI, avec des taux de consommation estimés par agent et type de tâche.
- [Outils d&#39;agentic CX Enterprise](https://experienceleague.adobe.com/fr/docs/cx-enterprise-agentic-tools/using/overview) couvrent les compétences et les outils agentic supplémentaires qui étendent les agents d&#39;agentic CX Enterprise (tutoriels vidéo).

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

Pour obtenir la liste complète des agents, les applications prises en charge par chacun et les conditions d’éligibilité, consultez [Agentic AI in CX Enterprise](./overview/agentic-ai.md).

## Collègue

Coworker est une évolution de l’IA Assistant orientée agent-first qui automatise l’expérience client et les workflows marketing, de sorte que votre équipe puisse se concentrer sur les objectifs commerciaux plutôt que sur l’exécution de routine. Au lieu de poser une question à la fois, vous décrivez un objectif. Un collègue planifie, exécute, valide et renvoie le travail terminé pour approbation. Le collaborateur comprend :

- **[Conversation avec un collègue](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)** : interface conversationnelle permettant d’explorer vos données, de valider les audiences et les parcours et d’effectuer des tâches en plusieurs étapes sur l’ensemble des applications d’entreprise CX.
- **[Campagnes des collègues](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)** : une application native à l’IA qui regroupe l’information sur la campagne, la création d’audiences, la génération de contenu, la conception de parcours et la relecture dans une seule expérience de conversation. Il utilise des modèles intégrés, des bonnes pratiques et des conseils pour aider les petites équipes agiles à lancer rapidement des campagnes.
- **Projets de collègues** (bientôt disponible) : espace de travail unifié pour automatiser les workflows d’orchestration de l’expérience client de bout en bout, ce qui permet aux équipes de coordonner les tâches, les approbations et l’exécution afin d’obtenir des résultats de la stratégie à la diffusion. La documentation des projets sera bientôt disponible.

Les clients éligibles passent progressivement de l’assistant AI et des agents Experience Platform au chat des collègues. Lisez [Version d’évaluation des collaborateurs](./agents/trial.md) pour en savoir plus sur l’éligibilité des versions d’évaluation, l’utilisation du crédit AI et comment y accéder.

Pour voir le Chat des collègues en action, [le Chat des collègues dans Playground](./coworker/playground-coworker-chat.md) ou lisez des cas d’utilisation réels tels que [Valider les données de migration d’AA vers CJA](./coworker/data-validation-aa-cja.md) et [Analyser les données CJA](./coworker/chat/analytics-chat.md).

Pour consulter la documentation complète sur les produits, les campagnes, les projets et le chat des collègues, voir [Collègue](./coworker/overview.md). Pour la réplication d’objet de sandbox à sandbox, voir [Compétences de l’agent d’outils Sandbox](./agents/sandbox-tooling.md).

## MCP

[Adobe CX Coworker Gateway](./mcp/overview.md) est le point d’entrée MCP (Model Context Protocol) unifié pour CX Enterprise. Il offre aux clients compatibles avec MCP, tels que [!DNL Claude], [!DNL ChatGPT] et [!DNL Cursor], une connexion unique régie aux outils de produit que votre entreprise est autorisée à utiliser. Ces outils comprennent [!DNL Real-Time CDP], [!DNL Experience Platform], [!DNL Journey Optimizer], [!DNL Customer Journey Analytics], [!DNL Adobe Analytics] et [!DNL Workfront].

Vous découvrez CX Coworker Gateway ? Voir [Accéder aux outils de la passerelle CX Coworker](./mcp/access.md) et [Installer la passerelle CX Coworker](./mcp/install.md) pour vous connecter.

## Commencer

### Exigences d’accès

Votre administrateur Adobe doit accorder les autorisations appropriées avant de pouvoir utiliser l’assistant AI et les agents Experience Platform. Les exigences varient selon l’application ; voir [Accès](./agents/agent-orchestrator.md#access) dans le guide d’Agent Orchestrator pour plus de détails.

### Confidentialité et sécurité

Les agents AI Assistant et Experience Platform donnent la priorité à la confidentialité, à la sécurité et à la gouvernance, y compris l’isolation des données spécifiques aux sandbox et vos politiques de contrôle d’accès existantes. Pour plus d’informations, lisez [Confidentialité, sécurité et gouvernance dans l’assistant AI](./ai-assistant/privacy.md).

## Bonnes pratiques

Pour tirer le meilleur parti de votre expérience d’assistant d’IA ou de collègue, suivez ces bonnes pratiques :

- **Soyez précis** dans vos invites pour obtenir des informations ciblées et pertinentes.
- **Vérifier les réponses** en examinant les citations de la source et les explications du raisonnement fournies.
- **Utilisez le paramètre contextuel** pour vous assurer que les sources de données les plus pertinentes sont utilisées pour vos questions.
- **Fournissez des commentaires** pour améliorer les performances et la précision au fil du temps.
- **Combinez les informations** de plusieurs agents pour une analyse plus complète.

## Considérations juridiques

L’assistant AI prend actuellement en charge les réponses en anglais uniquement et les modèles de langue peuvent parfois faire des erreurs. Vérifiez toujours les informations fournies et utilisez les étapes de raisonnement incluses dans chaque réponse pour comprendre comment elles ont été générées. Pour plus de détails, lisez la [clause de non-responsabilité](./ai-assistant/legal-disclaimer.md).

