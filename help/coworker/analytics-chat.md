---
title: Analyse des données Customer Journey Analytics avec la conversation des collègues
description: Découvrez comment utiliser le Module de conversation des collaborateurs d’entreprise Adobe CX pour analyser les données de Customer Journey Analytics, créer des entonnoirs et identifier les endroits où les clients abandonnent dans leur parcours.
source-git-commit: 6e3ab12f1d9ec706e745749b7ca47b91a09ff8b3
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 5%

---

# Analyse des données Customer Journey Analytics avec la conversation des collègues

>[!AVAILABILITY]
>
>La fonctionnalité décrite dans cet article se trouve dans la phase de test limité de la publication et peut ne pas encore être disponible dans votre environnement. Cette note sera supprimée lorsque la fonctionnalité sera disponible. Pour plus d’informations sur le processus de publication de Customer Journey Analytics, consultez [Versions des fonctionnalités de Customer Journey Analytics](https://experienceleague.adobe.com/fr/docs/analytics-platform/using/releases/latest).

Le Module de conversation des collaborateurs de l’entreprise Adobe CX peut effectuer une analyse avancée des données, auparavant uniquement possible dans Analysis Workspace. Le Module de conversation avec les collègues accède aux données à partir de vos vues de données Customer Journey Analytics, ce qui vous permet d’explorer ces données et d’obtenir des réponses aux invites en langage naturel.

Avant de commencer votre analyse, découvrez l’interface et les options de configuration du Module de conversation de Coworker, puis assurez-vous que Coworker est connecté à Customer Journey Analytics et à la vue de données contenant les données que vous souhaitez utiliser.

## Prise en main du chat des collègues

### Options d’interface et de configuration

Avant d’utiliser la discussion avec des collègues avec vos données Customer Journey Analytics, apprenez à vous connecter et à gérer les options de configuration pour les fonctionnalités suivantes :

* Entrées de conversation

* Conversations

* Marketplaces

* Serveurs MCP

* Mémoire

* Plug-ins

* Compétences

* Et en plus

Pour plus d’informations, consultez le [Guide de l’interface utilisateur de conversation des collègues](https://experienceleague.adobe.com/fr/docs/cx-enterprise-coworker/content/chat/ui-guide).

### Cas d’utilisation de Customer Journey Analytics

Vous pouvez voir des cas d’utilisation Customer Journey Analytics et des exemples d’invites que les utilisateurs utilisent dans le chat des collaborateurs en entreprise d’Adobe CX. Chaque invite est créée pour être copiée, adaptée à vos propres données et contexte et affinée par la conversation.

Pour plus d’informations, voir [Cas d’utilisation](https://experienceleague.adobe.com/fr/docs/cx-enterprise-coworker/content/chat/use-cases).

## Vérifier que la conversation avec un collègue est connectée à Customer Journey Analytics

1. Dans la conversation avec un collègue, vérifiez que celui-ci est connecté à Customer Journey Analytics :

1. Sélectionnez l’icône MCP dans le rail de gauche, puis assurez-vous que [!UICONTROL **cja-mcp**] est disponible dans la liste des serveurs MCP connectés.

   ![Icône MCP mise en surbrillance dans le rail de gauche de Coworker](assets/data-validation-aa-cja/coworker-mcp-cja.png)

1. (Conditionnel) Si [!UICONTROL **cja-mcp**] n’est pas encore connecté, sélectionnez [!UICONTROL **Ajouter le serveur MCP**], spécifiez cja dans le champ [!UICONTROL **Nom du serveur**] et sélectionnez-le lorsqu’il apparaît, puis sélectionnez [!UICONTROL **Ajouter le serveur**].

## Se connecter à la vue de données appropriée

Une vue de données est un conteneur dans Customer Journey Analytics qui détermine la manière dont les données sont interprétées.

Vous pouvez avoir accès à différentes vues de données dans Customer Journey Analytics, chacune contenant des dimensions et des mesures différentes que Coworker peut utiliser lors de l’analyse des données.

### Choix des vues de données à utiliser

Indiquez à votre collègue les types de questions auxquelles vous souhaitez obtenir une réponse et demandez-lui quelles vues de données auxquelles vous avez accès seraient les mieux placées pour fournir ces informations. Vous pouvez également [définir votre vue de données comme préférence en mémoire](#add-a-data-view-preference-in-memory).

**Vous:**

>[!BEGINSHADEBOX]

J&#39;aimerais savoir où les clients décrochent sur le parcours des clients. À quelles vues de données dans Customer Journey Analytics ai-je accès pour pouvoir répondre à cette question ?

>[!ENDSHADEBOX]

**Réponse du Chat des collègues :**

>[!BEGINSHADEBOX]

Vous avez accès à trois vues de données. La vue de données `Customer lifecycle` contient les dimensions et mesures suivantes, qui seraient les mieux adaptées pour répondre à votre question.

>[!ENDSHADEBOX]

**Vous:**

>[!BEGINSHADEBOX]

Très bien, utilisons cette vue de données.

>[!ENDSHADEBOX]

**Réponse du Chat des collègues :**

>[!BEGINSHADEBOX]

D’accord, j’utiliserai la vue de données `Customer lifecycle` pour répondre aux questions futures de cette session de conversation.

>[!ENDSHADEBOX]

### Ajout d’une préférence de vue de données en mémoire

Le Chat Coworker contient une fonctionnalité de mémoire qui vous permet de lui donner accès à des informations qui s’étendent sur toutes les conversations. Il est recommandé d’ajouter vos vues de données préférées en tant que préférences dans la mémoire du collègue.

1. Dans le volet de navigation de gauche de la discussion entre collègues, sélectionnez l’icône Mémoire .

1. Sur la page Mémoire, dans la section Préférences stockées , spécifiez une ou plusieurs vues de données que vous souhaitez que Chat des collaborateurs utilise dans vos conversations.

   ![Section Mémoire du rail de gauche](assets/data-validation-aa-cja/coworker-memory.png)

## Analyser dans Customer Journey Analytics

Une fois que Coworker a créé une visualisation, vous pouvez ouvrir la visualisation dans Analysis Workspace sous Customer Journey Analytics pour une analyse plus approfondie avec un contrôle plus granulaire. La visualisation s’ouvre dans un nouveau projet Analysis Workspace dans Customer Journey Analytics.

Pour ouvrir une visualisation dans un nouveau projet Analysis Workspace :

1. Sélectionnez [!UICONTROL **Analyser dans CJA**] en regard de toute visualisation créée dans Coworker.

1. Avec la visualisation ouverte dans Customer Journey Analytics, vous pouvez utiliser l’interface de navigateur glisser-déposer d’Analysis Workspace pour apporter des modifications, concevoir plus précisément votre analyse, créer une audience, et bien plus encore. Vous pouvez même partager votre projet Workspace avec toute personne de votre choix.

   Pour plus d’informations sur Analysis Workspace, consultez [Présentation d’Analysis Workspace](https://experienceleague.adobe.com/fr/docs/analytics-platform/using/cja-workspace/home).

## Exemple : Rechercher l’endroit où les clients repartent

Vous pouvez demander à Coworker Chat d’utiliser vos données pour analyser n’importe quelle question commerciale.

Par exemple, en tant que responsable marketing, marchandiseur ou responsable de croissance, vous pouvez vouloir comprendre où les clients abandonnent le chemin de l’achat, pourquoi ils l’ont fait et ce qui peut être fait pour augmenter les taux de conversion.

>[!NOTE]
>
>Les illustrations ci-dessous sont des exemples de données pour un retailer fictif, [!DNL TechPulse Electronics], utilisé pour montrer la forme de la conversation.

### Les types de questions que vous pouvez poser

Vous n’avez pas besoin de savoir ce qu’est une « visualisation des abandons » ou quelle mesure est utilisée dans quel emplacement. Décrivez plutôt le résultat qui vous tient à cœur en langage clair :

* « Où perdons-nous des gens sur le chemin de l&#39;achat ? »
* « Quel est mon funnel de conversion complet, de la consultation du produit au passage en caisse ? »
* « Quels canaux marketing présentent le plus de fuites entre le panier et l’achat ? »
* « L’abandon de panier est-il pire sur mobile ou poste de travail ? »
* « Les utilisateurs des réseaux sociaux payants se convertissent-ils différemment des utilisateurs des e-mails ? »

### La conversation

#### &#x200B;1. Commencez par la question commerciale

**Vous:**

>[!BEGINSHADEBOX]

Où perdons-nous des gens sur le chemin de l&#39;achat ?

>[!ENDSHADEBOX]

**Réponse du Chat des collègues :**

Notez que le Module de conversation des collègues sélectionne la visualisation appropriée, séquence les points de contact et ajoute même les étapes suivantes recommandées.

>[!BEGINSHADEBOX]

![Réponse du funnel de collègue](assets/data-validation-aa-cja/coworker-funnel-response.png)

Voici une question funnel : laissez-moi exécuter le funnel de conversion pour voir où se produit le déchargement sur le chemin d’accès à l’achat.

C&#39;est là que vous perdez des gens :

| Étape funnel | Nombre | Conversion en suivant | Abandon |
| --- | --- | --- | --- |
| Sessions | 137,476 | 45,0 % d’entre eux consultent un produit | 55 % quittent sans parcourir les produits |
| Consultations de produit | 61,845 | 55,0 % ajouter au panier | 45 % de navigation sans ajout |
| Ajouts au panier | 34,045 | Achat de 16,4 % | 83,6 % abandonnent le panier |
| Achats | 5,582 | — | — |

**La grande découverte : acheter un panier est votre plus grande fuite**

28 463 personnes ajoutent des articles à leur panier, mais ne terminent jamais l’achat. Il s&#39;agit d&#39;un taux de décrochage de 83,6 % du panier à l&#39;achat, soit de loin le point de défaillance le plus important.

En termes de dollars, la conversion de seulement 10 % de plus de ces ajouts au panier ajouterait environ 2 846 achats. À l&#39;échelle actuelle des données, il s&#39;agit d&#39;un revenu potentiellement important qui reste sur la table.

**Qu’est-ce que cela vous apprend sur les priorités**

| Priorité | Problème | Échelle des opportunités |
| --- | --- | --- |
| #1 | Abandon de panier à l’achat (baisse de 83,6 %) | 28 463 acheteurs perdus |
| #2 | Session pour consulter le produit (55 % ne parcourent jamais) | 75 631 sessions sans engagement produit |
| #3 | Consultations de produits du panier (45 % sans ajout) | 27 800 intéressés mais non engagés |

**Étapes suivantes recommandées :**

1. Ventilez les abandons de panier par canal marketing : certains canaux génèrent-ils un trafic de faible intention qui s’ajoute au panier mais n’achète jamais ?
1. Examiner l’abandon de panier par type d’appareil : le passage en caisse mobile détruit-il les conversions ?
1. Identifier les produits les plus abandonnés : problème de prix ? Surprise d&#39;expédition ?

**Dans laquelle de celles-ci voudriez-vous que je creuse ensuite ?** La répartition des canaux vous indiquerait directement quelles actions marketing vous amènent « quasi-acheteurs » par rapport aux acheteurs réels.

>[!ENDSHADEBOX]

#### &#x200B;2. Forer dans la fuite

**Vous:**

>[!BEGINSHADEBOX]

D’accord, répartissons par canal marketing

>[!ENDSHADEBOX]

**Réponse du Chat des collègues :**

>[!BEGINSHADEBOX]

![Réponse du funnel de collègue](assets/data-validation-aa-cja/coworker-funnel-response2.png)

Il existe une dimension **Canal marketing** personnalisée. Permettez-moi d’extraire le funnel par cela, puis de calculer les taux de conversion par canal et d’identifier où chaque canal fuit.

**Le verdict : la fuite n&#39;est pas spécifique à un canal**

C&#39;est une découverte très révélatrice. Voici la répartition funnel par canal :

| Canal | Sessions | À la vue du produit | Ajouter au panier | À acheter | Conversion globale | Chiffre d’affaires/session |
| --- | --- | --- | --- | --- | --- | --- |
| Recherche payante | 43,958 | 45.1% | 54.6% | 16.6% | 4.09% | $499.58 |
| Recherche organique | 31,492 | 44.9% | 54.9% | 16.9% | 4.17% | $494.76 |
| Direct | 25,661 | 43.6% | 55.4% | 15.8% | 3.82% | $497.29 |
| Email | 17,586 | 45.3% | 55.4% | 16.2% | 4.07% | $501.13 |
| Rémunération sociale | 12,684 | 45.4% | 55.7% | 16.0% | 4.03% | $512.17 |
| Affichage | 6,511 | 45.3% | 55.7% | 16.2% | 4.09% | $501.45 |

**Principaux points à retenir :**

1. Le taux de chute du panier à l’achat est uniformément mauvais sur tous les canaux (83 à 84 %). Cela signifie que le problème n&#39;est pas lié à la qualité du trafic - chaque canal fournit des visiteurs engagés similaires. La fuite se trouve dans votre expérience de passage en caisse elle-même, pas dans votre marketing.
1. Aucun canal n’est significativement meilleur ou pire lors de la conversion. Les taux de conversion globaux se regroupent étroitement entre 3,8 % et 4,2 %, et le chiffre d’affaires par session est presque identique (495 à 512 $).
1. Là où l’impact sur le volume est le plus important : le référencement payant perd le plus de monde en termes absolus (9 015 abandons de panier), suivi du référencement organique (6 449 perdus). Il s’agit des opportunités les plus importantes en termes de valeur monétaire, car elles génèrent le plus de trafic.

**Qu’est-ce que cela vous indique stratégiquement**

Les canaux marketing font leur travail : ils attirent tous les utilisateurs et les ajoutent au panier à des taux similaires. Le problème se situe en aval du marketing : votre caisse et votre flux de paiement sont là où l&#39;argent fuit.

**Prochaines investigations recommandées :**

1. Ventilez l’abandon du panier par type d’appareil : le passage en caisse mobile est-il rompu ou frustrant ?
1. Regardez quels produits sont abandonnés le plus souvent : y a-t-il une surprise de prix ou d&#39;expédition au passage en caisse ?
1. Vérifiez si la conversion de passage en caisse de la campagne « Holiday_flash_sale » est meilleure : les campagnes pilotées par l’urgence peuvent surmonter le conflit de passage en caisse.

**Quel angle souhaitez-vous explorer ensuite ?**

>[!ENDSHADEBOX]

#### &#x200B;3. Poursuivre l’enquête

**Vous:**

>[!BEGINSHADEBOX]

Intéressant. Essayons de ventiler par type d’appareil.

>[!ENDSHADEBOX]

**Réponse du Chat des collègues :**

>[!BEGINSHADEBOX]

![Réponse du funnel de collègue](assets/data-validation-aa-cja/coworker-funnel-response3.png)

**Trouvé : passage en caisse mobile rompu**

Le funnel est identique sur tous les appareils jusqu’au passage en caisse, puis le mobile tombe dans le précipice :

| Appareil | Sessions | À la vue du produit | Ajouter au panier | À acheter | Conversion globale |
| --- | --- | --- | --- | --- | --- |
| Bureau | 70,172 | 44.9% | 54.8% | 23.2% | 5.70% |
| Tablette | 14,149 | 44.7% | 55.6% | 14.3% | 3.56% |
| Mobile | 53,449 | 44.9% | 55.3% | 8.1% | 2.02% |

**Le pistolet fumant**

| Mesure | Bureau | Mobile | Écart |
| --- | --- | --- | --- |
| Taux panier à achat | 23.2% | 8.1% | 15 points de pourcentage |
| Le mobile est | — | 2,8 fois moins | — |
| Chariots abandonnés | 13,274 | 12,178 | Presque le même volume absolu |

L’expérience de navigation et d’ajout au panier est correcte sur mobile (taux de navigation identique de ~45 %, taux d’ajout au panier de ~55 %). Les gens sont tout aussi intéressés et engagés. Cependant, un élément du flux de passage en caisse mobile tue les conversions.

**L’opportunité de chiffre d’affaires**

Si le passage en caisse mobile était converti au même taux que le poste de travail, vous gagneriez environ 1 991 achats supplémentaires, soit une augmentation de 35 % du volume total d’achats résultant de la correction d’une expérience.

**Que se passe-t-il probablement**

Le modèle de données (engagement égal, passage en caisse catastrophique) est un signal classique pour :

* friction du formulaire de paiement sur de petits écrans (problèmes de remplissage automatique, mise en page du formulaire)
* Coûts inattendus révélés au passage en caisse (frais d&#39;expédition, taxes) provoquant un choc autocollant
* Passage en caisse des invités non disponible pour un mur de connexion sur mobile
* Problèmes de chargement de page ou de délai d’expiration lors du traitement des paiements sur mobile

**Étapes suivantes recommandées :**

1. Ventilez les abandons de panier mobile par catégorie de produits — est-ce pire pour les articles à prix élevé (qui suggèrent des problèmes de fiducie de paiement mobile) ?
1. Identifiez les canaux marketing qui génèrent le trafic mobile le plus important. Dépensez-vous des dollars de médias achetés pour envoyer des utilisateurs vers un funnel mobile endommagé ?
1. Vérifier s’il y a un signal de section de page ou de site — Peut-on voir quelles pages de passage en caisse les utilisateurs mobiles consultent en dernier avant d’abandonner ?

**Quelles sont les données que vous souhaitez explorer ou celles-ci sont-elles suffisantes pour être transmises à votre équipe d’expérience utilisateur et de passage en caisse ?**

>[!ENDSHADEBOX]

#### &#x200B;4. Transformez-la en décision

**Vous:**

>[!BEGINSHADEBOX]

Alors que dois-je faire ?

>[!ENDSHADEBOX]

**Réponse du Chat des collègues :**

>[!BEGINSHADEBOX]

D&#39;après ce que montrent les données, voici ce sur quoi je me concentrerais :

* **Corrigez le passage en caisse mobile, il ne s’agit pas d’un problème de canal.** Chaque canal convertit les utilisateurs en panier à un taux similaire et sain, de sorte que les dépenses publicitaires fonctionnent à tous les niveaux. Le chiffre d’affaires est perdu spécifiquement dans le flux de passage en caisse mobile, où se trouve le correctif.
* **Commencez par le paiement et la friction de formulaire.** Il s’agit des raisons les plus courantes pour lesquelles les acheteurs mobiles à forte intention abandonnent un panier. Offrir des options de porte-monnaie mobile et raccourcir le formulaire sont généralement les gains les plus rapides.
* **Vérifier à nouveau après le correctif.** Une fois que le passage en caisse a changé d’expédition, vérifiez si le taux de panier à l’achat de Mobile évolue vers le taux de poste de travail de 23,2 %.

Voulez-vous que j&#39;enregistre ceci en tant que projet afin que vous puissiez le suivre, ou définir une alerte si le panier mobile tombe en dessous d&#39;un seuil ?

>[!ENDSHADEBOX]

### Ce qui vient de se passer

Dans quatre questions en langage clair, Coworker nous a aidés :

* Créez un funnel de conversion à plusieurs étapes et signalez la fuite la plus importante, du panier à l’achat
* Excluez le canal marketing comme cause : chaque canal a fuité à un taux presque identique
* Isolez le vrai problème au passage en caisse mobile et quantifiez le correctif à un effet élévateur de 35 % dans les achats
* Partez avec un correctif spécifique à prioriser : le paiement mobile et la friction de formulaire. Il est comparé au taux de conversion de 23,2 % des ordinateurs de bureau

<!--

## Example #2: Find which marketing efforts drive revenue

You can ask Coworker Chat to use your data to analyze any business question.

For example, as a marketing manager, demand generation lead, or CMO, you might want to know which marketing efforts actually deserve credit for revenue so you can confidently decide where to put your marketing spend, rather than rewarding whichever channel happened to get the last click.

>[!NOTE]
>
>The figures below are illustrative sample data for a fictional retailer, [!DNL TechPulse Electronics], used to show the shape of the conversation.

### The types of questions you can ask

You don't need to know what an "attribution model" is, or how to configure an Attribution panel. Instead, describe the outcome you care about in plain language:

* "Which channels actually drive our revenue, not just the last click?"
* "If I change how I give credit for a sale, does my best channel change?"
* "Which campaigns start customer journeys versus close them?"
* "Am I over-investing in paid search because it always gets the last click?"
* "What role does email play in conversions it never gets credit for?"

### The conversation

#### 1. Start with the business question

**You:**

>[!BEGINSHADEBOX]

Which marketing channels actually drive our revenue?

>[!ENDSHADEBOX]

**Coworker Chat response:**

Notice that Coworker Chat picks the right analysis, starts with the model most reports default to, and immediately flags what that model can't tell you.

>[!BEGINSHADEBOX]

![Coworker Chat showing attributed revenue by marketing channel under a last-touch model](assets/data-validation-aa-cja/coworker-attribution-response.png)

This is an attribution question — let me attribute revenue to your marketing channels so you can see who's earning it.

I'll start with **last-touch attribution**, since that's what most out-of-the-box reports show. It gives all the credit for a sale to the last channel a person used before purchasing.

| Marketing channel | Attributed revenue (last touch) | Share |
| --- | --- | --- |
| Paid search | $948,000 | 34% |
| Organic search | $614,000 | 22% |
| Direct | $474,000 | 17% |
| Email | $307,000 | 11% |
| Paid social | $251,000 | 9% |
| Display | $195,000 | 7% |

**The headline: paid search looks like your hero**

Under last touch, paid search earns a third of all revenue — more than any other channel. If this were the only view you had, you'd likely pour more budget into paid search.

**One important caveat before you do that**

Last touch only tells you who *closed* the sale. It says nothing about who *started* the journey or *assisted* along the way. A channel that introduces people to your brand weeks before they buy gets zero credit here, even if the purchase never would've happened without it.

To know whether paid search is really driving revenue — or just harvesting demand other channels created — you need to compare attribution models.

**Recommended next step:**

Compare the same channels across first-touch, last-touch, and linear models. If paid search stays on top across all of them, it's a genuine driver. If it shrinks under first touch, it's a closer, not a creator.

**Want me to run that comparison?**

>[!ENDSHADEBOX]

#### 2. Compare attribution models

**You:**

>[!BEGINSHADEBOX]

Yes, compare it across models.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat comparing channel revenue share across first-touch, last-touch, and linear attribution models](assets/data-validation-aa-cja/coworker-attribution-response2.png)

Here's each channel's share of revenue under three models. First touch credits the channel that started the journey, last touch credits the one that closed it, and linear splits credit evenly across every touch.

| Marketing channel | First touch | Last touch | Linear |
| --- | --- | --- | --- |
| Paid search | 19% | 34% | 26% |
| Organic search | 20% | 22% | 21% |
| Direct | 9% | 17% | 13% |
| Email | 18% | 11% | 15% |
| Paid social | 21% | 9% | 15% |
| Display | 13% | 7% | 10% |

**The verdict: your "best" channel depends entirely on how you count**

This is the finding that changes budget decisions.

1. **Paid search closes far more than it starts.** It jumps from 19% of first touches to 34% of last touches. That's the signature of a *harvester* — it captures people who are already ready to buy, often after another channel introduced them. Valuable, but it's finishing journeys, not creating them.
1. **Paid social and email are badly undercredited by last touch.** Paid social starts 21% of journeys but gets credit for only 9% of sales. Email starts 18% but closes 11%. These channels are doing the expensive work at the top of the funnel and handing warm prospects to paid search.
1. **Organic search is your steady workhorse.** It sits around 20% across every model — it both starts and closes journeys reliably.

**Why this matters for budget**

If you cut paid social or email based on their weak last-touch numbers, you'd starve the top of your funnel — and paid search would have far fewer ready-to-buy people to close. You'd likely see paid search revenue fall too, even though you didn't touch its budget.

**Recommended next step:**

Look at the campaign level to see exactly which efforts start journeys versus close them. That's where you can act — trimming or protecting specific campaigns rather than whole channels.

**Want me to break this down by campaign?**

>[!ENDSHADEBOX]

#### 3. Keep investigating

**You:**

>[!BEGINSHADEBOX]

Let's break it down by campaign.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat showing top campaigns ranked by their role as initiators or closers of customer journeys](assets/data-validation-aa-cja/coworker-attribution-response3.png)

There's a **Campaign Name** dimension. Here are your highest-involvement campaigns, comparing the revenue they start (first touch) against the revenue they close (last touch).

| Campaign | Starts (first touch) | Closes (last touch) | Role |
| --- | --- | --- | --- |
| brand_awareness_q3 | $412,000 | $103,000 | Initiator |
| email_winback | $214,000 | $88,000 | Initiator |
| holiday_flash_sale | $268,000 | $249,000 | All-rounder |
| retargeting_dynamic | $71,000 | $339,000 | Closer |
| branded_search_always_on | $84,000 | $498,000 | Closer / harvester |

**The pattern: some of your "worst" campaigns are actually your best starters**

* **brand_awareness_q3** and **email_winback** start far more revenue than they close. On a last-touch ROI report, these look like underperformers you might cut. In reality, they're filling the top of your funnel — the journeys other campaigns finish.
* **retargeting_dynamic** and **branded_search_always_on** are the opposite. They close a lot but start almost nothing. They're efficient closers, but they can only close demand that already exists. Branded search, in particular, is largely capturing people who were going to search for you by name anyway.
* **holiday_flash_sale** does both — it introduces new shoppers and closes them, which is why urgency-driven promotions often look strong under any model.

**What this tells you strategically**

The campaigns you'd cut first on a last-touch report — the awareness and win-back efforts — are the ones creating the demand your closers depend on. Judge initiators on the journeys they start, and closers on the journeys they finish.

**Recommended next steps:**

1. Protect the initiator campaigns even though their last-touch ROI looks weak — they're feeding the funnel.
1. Right-size the branded search spend — test whether trimming it changes total revenue, since much of that demand may convert anyway.
1. Adopt a balanced model — like linear or a position-based model — as your default reporting view, so no channel gets systematically over- or under-rewarded.

**Want me to save this as a project, or is this enough to take into your budget planning?**

>[!ENDSHADEBOX]

#### 4. Turn it into a decision

**You:**

>[!BEGINSHADEBOX]

So how should I allocate budget?

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

Based on what the data shows, here's where I'd focus:

* **Stop judging upper-funnel channels on last touch alone.** Paid social and email start about 20% of your revenue each, but last touch credits them for less than half of that. Protect their budgets — they're creating the demand paid search closes.
* **Treat branded search as a harvester, not a driver.** It closes a lot but starts almost nothing. Test trimming it, since much of that demand may convert through other paths anyway.
* **Make a balanced model your default.** Reporting on linear or a position-based model instead of last touch will stop you from over-rewarding closers and under-funding the channels that start journeys.
* **Re-check after you rebalance.** Watch whether total revenue holds steady as you shift spend toward initiators — that's the signal your funnel is healthier, not just your last-touch report.

Want me to save this as a project so you can track it, or build a calculated metric that reports revenue on a balanced attribution model going forward?

>[!ENDSHADEBOX]

### What just happened

In four plain-language questions, Coworker helped us:

* Attribute revenue to marketing channels and flag that the default last-touch view tells only part of the story
* Compare attribution models and reveal that the "best" channel changes completely depending on how credit is counted
* Discover that paid social and email start far more revenue than they ever get credit for closing
* Identify which campaigns initiate journeys versus close them, and walk away with a budget direction: protect the initiators, right-size the harvesters, and report on a balanced model

-->
